# Yocto Image for Raspberry Pi 3B+

This project utilizes Poky to build a Linux image for Raspberry Pi 3B+.

## Steps to Build the Image:

**1. Source  to `oe-init-build-env` script:**
  $ source poky/oe-init-build-env my_build

**2. Replace the configuration files local.conf and bblayes.conf in my_build/conf/ with the files from repo rpi_build/conf/**

**3. Run below bitbake command to build the x11 image.**
  $ bitbake core-image-x11
  This will generate image file in my_build/tmp/image/
  
**4. To build the qt5 toolchain for application development run below command.**
  $ bitbake meta-toolchain-qt5
This will generate tookit installer under the path my_build/tmp/sdk/
