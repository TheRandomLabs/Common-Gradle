# Common-Gradle

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Dependabot](https://badgen.net/dependabot/TheRandomLabs/Common-Gradle/?icon=dependabot)](https://dependabot.com/)

A common Gradle buildscript for my projects.

```groovy
apply from: "https://raw.githubusercontent.com/TheRandomLabs/Common-Gradle/master/build.gradle"
```

Without dependencies:

```groovy
apply from: "https://raw.githubusercontent.com/TheRandomLabs/Common-Gradle/master/no-dependencies/build.gradle"
```

Fat runnable jar:

```groovy
ext.mainClass = "${group}.Main"

apply from: "https://raw.githubusercontent.com/TheRandomLabs/Common-Gradle/master/runnable/build.gradle"
```
