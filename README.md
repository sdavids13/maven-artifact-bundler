Maven Artifact Bundler
==========

This project allows clients provide a maven artifact via the `artifact` system or gradle property
 and produces a zip file in a maven directory structure containing the given artifact and all
 dependencies. The motivation is to easily zip the desired artifact and dependencies for easy import
 into a stand-alone maven server.

## Execution
Example execution: `./gradlew -Partifact=com.netflix.nebula:gradle-ospackage-plugin:2.2.6 bundle`
this produces an output `com.netflix.nebula:gradle-ospackage-plugin:2.2.6-maven-bundle.zip` in the `build` directory.

Note: the `artifact` syntax is in the format of `<group id>:<artifact id>:<version>`