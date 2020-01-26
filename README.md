# Common-Gradle

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Dependabot](https://badgen.net/dependabot/TheRandomLabs/Common-Gradle/?icon=dependabot)](https://dependabot.com/)

A common Gradle buildscript for my projects.

```groovy
ext {
	//testing = false
	disableDefaultCompileDependencies = true //Guava and SLF4J.
	mainClass = "com.test.Main"
	jacocoMinimumInstructionCoverage = 0.1
	jacocoExcludes = ["com.test.*"]
}

group = "com.test"
version = "1.0.0"

apply from: "https://raw.githubusercontent.com/TheRandomLabs/Common-Gradle/master/build.gradle"
```
