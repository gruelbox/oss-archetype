# oss-archetype
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

TODO

## Enable Travis build

TODO

## Publish to Maven Central

TODO
