# Common-Gradle

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
![Build](https://github.com/TheRandomLabs/Common-Gradle/workflows/Build/badge.svg?branch=master)
[![Dependabot](https://badgen.net/dependabot/TheRandomLabs/Common-Gradle/?icon=dependabot)](https://dependabot.com/)

A common Gradle buildscript for my projects.

```groovy
ext {
	commonGradleBranch = "master"
	javaVersion = 11
	useSpotBugs = false
	testing = true //true by default
	defaultCompileDependencies = false //Guava and SLF4J.
	autoUpdateLicenses = false
	mainClass = "com.test.Main"
	jacocoMinimumInstructionCoverage = 0.1
	jacocoExcludes = ["com.test.*"]
	registerDefaultMavenPublication = false
}

group = "com.test"
version = "1.0.0"

apply from: "https://raw.githubusercontent.com/TheRandomLabs/Common-Gradle/${project.commonGradleBranch}/build.gradle"
```
