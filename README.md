# oss-archetype

[![Build Status](https://travis-ci.org/gruelbox/oss-archetype.svg?branch=master)](https://travis-ci.org/gruelbox/oss-archetype)

An opinionated archetype designed to set up a new open source library. Includes:

  - JUnit
  - Mockito
  - Hamcrest
  - Checkstyle
  - Findbugs
  - JaCoCo

Along with all configuration in place and instructions for setting up:

  - Publishing to Maven Central via OSSRH (including sources, Javadoc etc)
  - Build, test and deploy to OSSRH automatically from Travis CI
  - Source code analysis on Sonarcloud

And a README chock-full of lovely badges covering everything from test coverage to build status to Javadocs.

# Usage

## Create the project

To create your project, clone this repo, then:

```
mvn install
cd ..
mvn archetype:generate -DarchetypeGroupId=com.gruelbox -DarchetypeArtifactId=oss-archetype -DarchetypeVersion=0.0.2-SNAPSHOT
```

You can now open the project in your IDE and push it to GitHub.

## Connect to Sonar

TODO detail

  - Add to account
  - Create key
  - Encrypt with `travis` ruby tool
  - Add to POM

## Enable Travis build

TODO detail

  - Add to Travis
  - SHould just work

## Publish to Maven Central

TODO, referencing https://www.phillip-kruger.com/post/continuous_integration_to_maven_central/

# Credit

Large parts of this build heavily on the Travis script and POM in Alfa Systems [Morf](https://github.com/alfasoftware/morf) by Venushka Perera, which uses a toolset I am familiar with and use for all my projects.  It in turn leans heavily on the approach in [this great post](https://www.phillip-kruger.com/post/continuous_integration_to_maven_central/) by Phillip Krüger.
