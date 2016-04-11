# gradle-android-javadoc-plugin

[![Build Status](https://travis-ci.org/vanniktech/gradle-android-javadoc-plugin.svg?branch=master)](https://travis-ci.org/vanniktech/gradle-android-javadoc-plugin?branch=master)
[![Codecov](https://codecov.io/github/vanniktech/gradle-android-javadoc-plugin/coverage.svg?branch=master)](https://codecov.io/github/vanniktech/gradle-android-javadoc-plugin?branch=master)
[![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
![Java 8 required](https://img.shields.io/badge/java-8-brightgreen.svg)

Gradle plugin that generates Java Documentation from an Android Gradle project.

Works with the latest Gradle Android Tools version 1.3.1. This plugin is compiled using Java 8 hence you also need Java 8 in order to use it.

# Set up

**app/build.gradle or library/build.gradle**

```groovy
buildscript {
    repositories {
        mavenCentral()
    }
    dependencies {
        classpath 'com.vanniktech:gradle-android-javadoc-plugin:0.2.1'
    }
}

apply plugin: 'com.vanniktech.android.javadoc'
```

Information: [This plugin is also available on Gradle plugins](https://plugins.gradle.org/plugin/com.vanniktech.android.javadoc)

### Snapshots

Can be found [here](https://oss.sonatype.org/#nexus-search;quick~gradle-android-javadoc-plugin). Current one is:

```groovy
classpath 'com.vanniktech:gradle-android-javadoc-plugin:0.2.2-SNAPSHOT'
```

## Get Javadoc

```groovy
./gradlew generateDebugJavadoc
./gradlew generateReleaseJavadoc
```

**HTML reports**

```
<subproject>/javaDoc/debug/index.html
<subproject>/javaDoc/release/index.html
```

# License

Copyright (C) 2015 Vanniktech - Niklas Baudy

Licensed under the Apache License, Version 2.0