# [WIP]obs-asio
ASIO is a trademark and software of Steinberg Media Technologies GmbH

This is a third-party plugin to extend OBS's native support of common audio drivers to include ASIO enabled devices. 
This software is subject to no warranty or garuntee. Use at your own risk.

To Build:
Follow instructions on https://github.com/jp9000/obs-studio/wiki/Install-Instructions

With minor changes, namely:

```
git clone --recursive https://github.com/andersama/obs-studio.git
```

Checkout the `asio-support` branch, this repo will be included as a submodule in the plugins directory.
It also has modifications to the CMakeLists.txt to add the plugin as a build option, be sure to check that option using cmake.

In command-line for you linux and mac lovers~:
```
cmake ... -D BUILD_ASIO_SUPPORT=yes
```

Given the license terms of the SDK, I can't distribute it, however you may download it yourself to build the working plugin

[https://www.steinberg.net/en/company/developers.html](https://www.steinberg.net/en/company/developers.html)

Extract the files to .../obs-asio/asiosdk2.3
