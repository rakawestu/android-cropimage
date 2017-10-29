# Android CropImage

<img src="https://cdn.rawgit.com/lvillani/android-cropimage/f55253d2be3e6c28a06dd8bdd1e45aa7fd0b22a1/logo.svg" align="right" width="200" height="200"/>

[![License](http://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat)](http://choosealicense.com/licenses/apache-2.0/)

--------------------------------------------------------------------------------

The `CropImage` activity extracted from `Gallery.apk` (AOSP 4.4.4). Compatible
with Android API Level 15 and up.

--------------------------------------------------------------------------------

## :warning: Not Maintained

This project is not maintained anymore. Starting January 2018 the source code will be replaced with
a deprecation notice. This repository will be decommissioned in June 2018. Both source and binary
artifact may become unavailable after that point.

--------------------------------------------------------------------------------

## :warning: Maven Repository URL Changed

The Maven repository has been moved to <http://lvillani.github.io/android-cropimage/>. Please see
the updated documentation and the [example](./CropImageRepo) for more details.

The old repository URL may become unavailable starting January 2018.

--------------------------------------------------------------------------------

## Android Studio and Gradle

The project was created with Android Studio and uses the Gradle build system.


## Intent-based API

The `CropImage` activity is controlled by an Intent-based API. Please use the wrapper class
[CropImageIntentBuilder](CropImage/src/main/java/com/android/camera/CropImageIntentBuilder.java)
for a type-safe interface.


## Example Project

It is contained inside the `CropImageExample` module.


## Gradle Repository

There's a [Gradle repository](http://lvillani.github.io/android-cropimage/) available at
<http://lvillani.github.io/android-cropimage/>.

In your top-level `build.gradle` add the address of the Maven repository to the `repositories`
section so that it looks like:

```groovy
repositories {
    mavenCentral()

    maven {
        url 'http://lvillani.github.io/android-cropimage/'
    }
}
```

Then add the dependency to your `dependencies` section:

```groovy
compile 'me.villani.lorenzo.android:android-cropimage:1.1.+'
```

For more information see the `CropImageRepo` example (the project doesn't do anything, it only shows
how to pull the dependency through Gradle).
