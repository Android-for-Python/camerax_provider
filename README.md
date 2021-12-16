camerax_provider
================

An Android camera provider for Camera4Kivy.

# Install

Camera4Kivy depends on the 'master' version of Buildozer. Currently `1.2.0.dev0`

`pip3 install git+https://github.com/kivy/buildozer.git`

To add a camera provider and a recipe to an Android project that uses Camera4Kivy:

`cd <project directory>`

`git clone https://github.com/Android-for-Python/camerax_provider.git`

`rm -rf camerax_provider/.git`


# Contents

`gradle_options.py` sets

`android.enable_androidx = True`
`android.gradle_dependencies = ` as required for camerax

`recipes/camera4kivy/` contains the camerax implementation