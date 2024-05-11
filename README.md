Yocto Image for Raspberry Pi 3B+:

This project uses poky to build a linux image for raspberry pi 3b+ machine.

Follow these setps:
1. Source “oe-init-build-env” script
  $ source poky/oe-init-build-env my_build
2. Replace the configuration files local.conf and bblayes.conf in my_build/conf/ with the files from repo rpi_build/conf/
3. Run below bitbake command to build the x11 image.
  $ bitbake core-image-x11
4. To build the qt5 toolchain for application development run below command.
  $ bitbake meta-toolchain-qt5
