## TensorFlow Android Camera Demo
This folder contains an example application utilizing TensorFlow for Android
devices.
### Description
The demos in this folder are designed to give straightforward samples of using
TensorFlow in mobile applications.

Inference is done using the [TensorFlow Android Inference Interface](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/examples/android),
which may be built separately if you want a standalone library to drop into your
existing application. Object tracking and YUV -> RGB conversion is handled by
libtensorflow_demo.so.

A device running Android 5.0 (API 21) or higher is required to run the demo due
to the use of the camera2 API, although the native libraries themselves can run
on API >= 14 devices.
### Building from Source
Pick your preferred approach below. At the moment, we have full support for
Bazel, and partial support for gradle, cmake, make, and Android Studio.

As a first step for all build types, clone the TensorFlow repo with:
```
git clone https://github.com/i25ffz/tf-demos.git
gradle downloadJar
gradle installDebug
```
