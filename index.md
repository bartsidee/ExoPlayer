---
layout: default
title: Home
---

ExoPlayer is an application level media player for Android. It provides an alternative to Android’s
MediaPlayer API for playing audio and video both locally and over the Internet. ExoPlayer supports
features not currently supported by Android’s MediaPlayer API (as of KitKat), including DASH and
SmoothStreaming adaptive playbacks, persistent caching and custom renderers. Unlike the MediaPlayer
API, ExoPlayer is easy to customize and extend, and can be updated through Play Store application
updates.

### Blog ###

Read news, hints and tips in the ExoPlayer [blog]({{ site.baseurl }}/blog.html).

### Developer guide ###

The [ExoPlayer developer guide]({{ site.baseurl }}/guide.html) provides a wealth of information to
help you get started.

### Reference documentation ###

ExoPlayer's [class reference pages]({{ site.baseurl }}/doc/reference) document the ExoPlayer library
classes.

### Project branches ###

  * The [master][] branch holds the most recent minor release.
  * Most development work happens on the [dev][] branch.
  * Additional development branches may be established for major features.

[master]: https://github.com/google/ExoPlayer/tree/master
[dev]: https://github.com/google/ExoPlayer/tree/dev

### Using Eclipse ###

The repository includes Eclipse projects for both the ExoPlayer library and its
accompanying demo application. To get started:

  1. Install Eclipse and setup the [Android SDK][].

  1. Open Eclipse and navigate to File->Import->General->Existing Projects into
     Workspace.

  1. Select the root directory of the repository.

  1. Import the ExoPlayerDemo and ExoPlayerLib projects.

[Android SDK]: http://developer.android.com/sdk/index.html

### Using Gradle ###

ExoPlayer can also be built using Gradle. You can include it as a dependent project and build from
source. e.g.

```
// settings.gradle
include ':app', ':..:ExoPlayer:library'

// app/build.gradle
dependencies {
    compile project(':..:ExoPlayer:library')
}
```

If you want to use ExoPlayer as a jar, run:

```
./gradlew jarRelease
```

and copy library.jar to the libs-folder of your new project.