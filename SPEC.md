# Code Climate Engine Specification

## Abstract

This specification describes the contract that must be followed by an engine to ensure compatability with the rest of the tools in the Code Climate static analysis ecosystem. It defines several aspects of Engine operation including input, outputs, packaging, as well as performance and security restrictions.

## Status of this document

The current version of this specification is [in the repository](https://github.com/codeclimate/spec/blob/master/VERSION).  This specification is versioned using [Semantic Versioning](http://semver.org/).

Engines declare the version of the specification they are compatible with in the engine specification file, described below.

We welcome your participation and appreciate your patience as we finalize the platform.

## Table of contents

- [Overview](#overview)
- [Engine execution](#engine-execution)
    - [Input](#input)
        - [Which files to analyze](#which-files-to-analyze)
    - [Output](#output)
    - [Resource restrictions](#resource-restrictions)
    - [Security restrictions](#security-restrictions)
- [Engine specification file](#engine-specification-file)
- [Data types](#data-types)
    - [Issues](#issues)
        - [Descriptions](#descriptions)
        - [Categories](#categories)
        - [Remediation points](#remediation-points)
    - [Locations](#locations)
        - [Positions](#positions)
    - [Other Locations](#other-locations)
    - [Contents](#contents)
    - [Source code traces](#source-code-traces)
- [Packaging](#packaging)
- [Naming convention](#naming-convention)

## Overview

A Code Climate engine is a standalone program which accepts a configuration and source code, and returns static analysis results. It can be implemented in any programming language, and is distributed as a Docker image.

## Engine execution

### Input

The Engine Docker container is provided the source code to analyze at `/code`, which is mounted as a read-only volume.

* `/code`, a directory containing the files to analyze (read-only)

Engines accept a configuration in JSON format passed as a read-only file mounted at `/config.json`.

Engines can define their own appropriate configuration keys and values, based on
their needs. A developer invoking a Code Climate engine stores their configuration
for all engines in a single `.codeclimate.yml` file. The Code Climate CLI (and other tools compatible with Code Climate Engines) parse and interpret the YAML file to produce a single, simple JSON config object for each engine.

The `include_paths` key will always be present in `config.json`, and must be used by engines to limit which files they will analyze. Details of this key are below.

#### Which files to analyze

`include_paths` in `/config.json` contains an array of file paths and directory paths (relative to the `/code` directory) that defines the range of files that the engine can analyze. Directories will end with a trailing slash. For example:

```json
{
  "include_paths":[
    ".gitignore",
    "app/",
    "test/"
  ]
}
```

`include_paths` may include paths to files that are irrelevant to the analysis (i.e., `.gitignore` if the engine only analyzes JavaScript). Engines are responsible for filtering out irrelevant files.

### Output

* Engines must stream [Issues](#issues) to `STDOUT` in JSON format.
* When possible, results should be emitted as soon as they are computed (streamed, not buffered).
* Each issue must be terminated by the [null character][null] (`\0` in most programming languages), but can additionally be separated by newlines.
* Unstructured information can be printed on `STDERR` for the purposes of aiding debugging.
  * *Note that `STDERR` output will only be displayed in console output when there is a failure, unless `codeclimate analyze` is run with the `CODECLIMATE_DEBUG` environment variable, e.g. `CODECLIMATE_DEBUG=1 codeclimate analyze`
* Engines must exit with a zero exit code unless a fatal error in the process occurs.
  * *Note that an engine finding and emitting issues is expected, and not a fatal error - this means that if your engine finds issues, it should still in all cases exit with code zero.*
  * *Note that all results will be discard and the analysis failed if an engine exits with a non-zero exit code.*



### Resource restrictions

In order to ensure analysis runs reliably across a variety of systems, Engines
must conform to some basic resource restrictions:

* The Docker image for an Engine must not exceed 512MB, including all layers.
* The combined total RSS memory usage by all processes within the Docker container must not exceed 1GB at any time.
* All Engines must complete and exit within 10 minutes.

### Security restrictions

Engines run in a secured runtime environment, within container-based virtualization
provided by Docker.

* The `/code` directory, containing the files to analyze, & `/config.json`, containing configuration for the engine to use, are mounted read-only.
* Engines run with no network access (`--net=none` in Docker). They must not rely on making any external network calls.
* Engines run with the minimal set of Linux capabilities (`--cap-drop all` in Docker)
* Engines are always run as a user `app` with UID and GID of 9000, and never `root`.

## Engine specification file

All engines must include an `engine.json` file at `/engine.json`. This file includes information that is necessary for the analysis runtime and metadata about the engine. Here is an example specification:

```json
{
  "name": "govet",
  "description": "govet was created by the Go team at Google, and examines Go source code and reports suspicious constructs, and potential bugs.",
  "maintainer": {
    "name": "Michael R. Bernstein",
    "email": "mrb@codeclimate.com"
  },
  "languages" : ["Go"],
  "version": "da5a2077",
  "spec_version": "0.0.1"
}
```

The following fields are declared in the specification file, and all are required:

* `name` (`String`) - the name of the package
* `description` (`String`) - a description of the engine
* `maintainer` (`Object`) - data about the engine maintainer
  * `name` (`String`) - the name of the maintainer
  * `email` (`String`) - the email address of the maintainer
* `languages` (`[String]`) - an array of programming languages that this engine is meant to analyze. **See note about possible values for `languages` below**
* `version` (`String`) - engine version, an arbitrary string maintained by the engine maintainer
* `spec_version` (`String`) - the version of the specification which this engine supports

The `languages` key can have the following values:
- `*` - all possible languages, for language agnostic analysis engines
- Any language listed as keys in the `github/linguist` repository's data file, which [can be found here](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml).
- Note that we follow these spellings exactly, so while [`JavaScript` is a valid spelling of that language](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml#L1642), `javascript` is not.
- Some commonly used languages spelled properly are: `CSS, Clojure, CoffeeScript, Go, Haskell, Java, JavaScript, PHP, Python, Ruby, SCSS, Scala, Shell`

## Data Types

### Issues

An `issue` represents a single instance of a real or potential code problem, detected by a static analysis Engine.

```json
{
  "type": "issue",
  "check_name": "Bug Risk/Unused Variable",
  "description": "Unused local variable `foo`",
  "content": Content,
  "categories": ["Complexity"],
  "location": Location,
  "other_locations": [Location],
  "remediation_points": 50000,
  "severity": Severity,
  "fingerprint": "abcd1234"
}
```

* `type` -- **Required**. Must always be "issue".
* `check_name` -- **Required**. A unique name representing the static analysis check that emitted this issue.
* `description` -- **Required**. A string explaining the issue that was detected.
* `content` -- **Optional**. A markdown snippet describing the issue, including deeper explanations and links to other resources.
* `categories` -- **Required**. At least one category indicating the nature of the issue being reported.
* `location` -- **Required**. A `Location` object representing the place in the source code where the issue was discovered.
* `trace` -- **Optional.** A `Trace` object representing other interesting source code locations related to this issue.
* `remediation_points` -- **Optional**. An integer indicating a rough estimate of how long it would take to resolve the reported issue.
* `severity` -- **Optional**. A `Severity` string (`info`, `minor`, `major`, `critical`, or `blocker`) describing the potential impact of the issue found.
* `fingerprint` -- **Optional**. A unique, deterministic identifier for the specific issue being reported to allow a user to exclude it from future analyses.

#### Descriptions

Descriptions must be a single line of text (no newlines), with no HTML formatting contained within. Ideally, descriptions should be fewer than 70 characters long, but this is not a requirement.

Descriptions support one type of basic Markdown formatting, which is the use of backticks to produce inline &lt;code&gt; tags that are rendered in a fixed width font. Identifiers like class, method and variable names should be wrapped within backticks whenever possible for optimal rendering by tools that consume Engines data.

#### Categories

Issues must be associated with one or more categories. Valid issue `categories` are:

- `Bug Risk` -- TODO describe me
- `Clarity` -- TODO describe me
- `Compatibility` -- TODO describe me
- `Complexity` -- TODO describe me
- `Duplication` -- TODO describe me
- `Performance` -- TODO describe me
- `Security` -- TODO describe me
- `Style` -- TODO describe me

#### Remediation points

Remediation points are an abstract, relative scale to express the estimated time it would take for a developer to resolve an issue. They are abstract because they do not map directly to absolute time durations like minutes and hours. Providing remediation points is optional, but they can be useful to certain tools that consume Engines data and generate reports related to the level of effort required to improve a codebase (like CodeClimate.com).

Here are some guidelines to compute appropriate remediation points values for an Issue:

* The more local an issue is, generally the easier it is to fix. For example, issues that only require consideration of a single line tend to be easier to fix than issues that potentially affect an entire function, class, module, or program.
* TODO more

The baseline remediation points value is 50,000, which is the time it takes to fix a trivial code style issue like a missing semicolon on a single line, including the time for the developer to open the code, make the change, and confidently commit the fix. All other remediation points values are expressed in multiples of that Basic Remediation Point Value.

### Locations

Locations refer to ranges of a source code file. A Location contains a `path` and a source range, (expressed as `lines` or `positions`). Here's an example location:

```json
{
  "path": "path/to/file.css",
  "lines": {
    "begin": 13,
    "end": 14
  }
}
```
And another:

```json
{
  "path": "path/to/file.css",
  "positions": {
    "begin": {
      "line": 3,
      "column": 10
    },
    "end": {
      "line": 4,
      "column": 12
    }
  }
}
```

All Locations require a `path` property, which is the file path relative to `/code`.

Locations of the first form (_line-based_ locations) emit a beginning and end line number for the issue, which form a range. Line numbers are 1-based, so the first line of a file would be represented by `1`. Line ranges are evaluated inclusively, so a range of `{"begin": 9, "end": 11}` would represent lines 9, 10 and 11.

Locations in the second form (_position-based_ locations) allow more precision by including references to the specific characters that form the source code range representing the issue.

#### Positions

Positions refer to specific characters within a source file, and can be expressed in two ways:

1. Line and column coordinates. (You can roughly think of these as X/Y axis.)
2. Absolute character offsets, for the _entire source buffer_.

For example:

```json
{
  "line": 3,
  "column": 10
}
```

Or:

```json
{
  "offset": 4
}
```

Line and column numbers are 1-based. Therefore,
a Position of `{ "line": 2, "column": 3 }` represents the third character on the second
line of the file.

Offsets, however are 0-based. A Position of `{ "offset": 4 }` represents the _fifth_ character in the file. Importantly, the `offset` is from the beginning of the file, not the beginning of a line. Newline characters (and all characters) count when computing an offset.

### Other Locations

Other locations is an optional array of [Location](#locations) objects:

```json
"other_locations": [
  {
    "path": "foo.rb",
    "lines": { "begin": 25, "end": 55 }
  },
  {
    "path": "bar.rb",
    "lines": { "begin": 20, "end": 50 }
  }
]
```

### Contents

Content gives more information about the issue's check, including a description of the issue, how to fix it, and relevant links. They are expressed as a hash with a `body` key. The value of this key should be a [Markdown](http://daringfireball.net/projects/markdown/) document. For example:

```json
{
  "body": "This cop checks that the ABC size of methods is not higher than the configured maximum. The ABC size is based on assignments, branches (method calls), and conditions. See [this page](http://c2.com/cgi/wiki?AbcMetric) for more information on ABC size."
}
```
### Source code traces

Some engines require the ability to refer to other source locations in describing an issue. For this reason, an `Issue` object can have an associated `Trace`, a data structure meant to represent ordered or unordered lists of source code locations. A `Trace` has the following fields:

* `locations` -- **[Location] - Required**. An array of [Location](#locations) objects.
* `stacktrace` -- **Boolean - Optional **. *Default: false* When `true`, this `Trace` object will be treated like an ordered stacktrace by the CLI and the Code Climate UI.

An example trace:

```json
"trace": {
  "locations": [{
    "path": "path/to/file.css",
      "lines": {
        "begin": 13,
        "end": 14
      }
    },
    {
      "path": "path/to/file.css",
      "lines": {
        "begin": 19,
        "end": 20
      }
    }],
  "stacktrace": true
}

```


## Packaging

Engines are packaged and distributed as Docker images, which allows them to be
easily portable between systems, regardless of the programming language they are
implemented in. We recommend Engine implementors use a `Dockerfile` to automate
the builds of these images. The `Dockerfile` must follow these specifications:

* The image must specify a `maintainer` `LABEL`:
* The `/code` must be declared as a `VOLUME`.
* The `WORKDIR` must be specified as `/code`
* A non-root user named `app` must be created with UID and GID 9000 and declared
  using the `USER` directive.
* A default command (`CMD`) must be declared so that the engine can be invoked without specifying a command
* The image must not include any `EXPOSE` directives
* The image must not include any `ONBUILD` directives

Here is an example of a `Dockerfile` that follows the specifications for an engine written in Node.js:

```
FROM node:7.7-alpine

LABEL maintainer "Your Name <hello@example.com>"

WORKDIR /usr/src/app
COPY package.json /usr/src/app/

RUN npm install

RUN adduser -u 9000 -D app
COPY . /usr/src/app
RUN chown -R app:app /usr/src/app

USER app

VOLUME /code
WORKDIR /code

CMD ["/usr/src/app/bin/your-engine"]
```

## Naming convention

Your `Docker` image must be built with the name `codeclimate/codeclimate-YOURENGINENAME`.


[null]: http://en.wikipedia.org/wiki/Null_character

