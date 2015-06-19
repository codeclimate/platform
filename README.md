# Code Climate Engine

This repository contains the definition of the Code Climate Engine specification. This includes technical details about how to implement a static analysis engine compatible with the Code Climate ecosystem of tools, including the ability to run it locally as well as on [CodeClimate.com](https://codeclimate.com/). See [SPEC.md](SPEC.md) for the actual specification.

## What is a Code Climate Engine?

A _Code Climate Engine_ is a static analysis module. Static analysis refers to the
act of deriving data from code without actually executing it. Code Climate Engines
have been created to produce data about code quality, security, style, performance and bug risk across a variety of programming languages.

### What is the Code Climate Engine spec?

The Code Climate Engine spec describes a simple contract that must be followed to
ensure compatability with the rest of the tools in the Code Climate static analysis
ecosystem. It defines several aspects of Engine operation including input, outputs, packaging, as well as performance and security restrictions.

## What is the promise of the Code Climate Engine spec?

Defining a simple specification that any static analysis tool can easily conform
to makes it possible to integrate them all into a clear, unified workflow for developers. Engines can be run locally at any time on developers' laptops on the command line, but can also be set up to run on CodeClimate.com (which is free for open source) automatically after every commit and Pull Request.

## What are some implementations of the spec?

The most mature implementations of the spec are:

* codeclimate-rubocop
* codeclimate-govet
* codeclimate-golint
* codeclimate-gofmt
* codeclimate-watson
* codecliamte-rubymotion
* codecliamte-coffeelint
* codeclimate-csslint

## Working with the spec

To get started implementing an Engine, first install the **[Code Climate CLI](https://github.com/codeclimate/codeclimate)**. Once that is installed, build your Engine as a Docker image (see the Packaging section of the SPEC). When you are ready to test it locally, run:

    $ TODO
