camerax_provider
================

An Android camera provider for Camera4Kivy.

**2023-11-13 This repository is archived.**

Camera4Kivy depends on the 'master' version of Buildozer. Currently `1.2.0.dev0`

`pip3 install git+https://github.com/kivy/buildozer.git`

The current version is 0.0.3

# Install

To add a camera provider to an Android project that uses Camera4Kivy:

`cd <project directory>`

`git clone https://github.com/Android-for-Python/camerax_provider.git`

`rm -rf camerax_provider/.git`

Then in buildozer.spec set

`p4a.hook = camerax_provider` 

No other camera specific buildozer.spec changes are required.

Note: The implementation of the gradle dependencies is architecture specific, an app built for armeabi-v7a will crash on an arm64-v8a device.

# Behavior

This hook adds the following buildozer.spec options to the build:

`android.enable_androidx = True`

`android.permissions = CAMERA, RECORD_AUDIO`

`android.gradle_dependencies = ` as required for camerax

`android.add_src = camerax_provider/camerax_src`



