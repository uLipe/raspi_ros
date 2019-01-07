raspi_ros
============

This is a collection of core recipes to allow building a embedded linux distro which
supports ROS, the idea is to make simple the building of ROS powered devices which 
are intended to execute on constrained devices, embedded systems.

# Disclaimer:
This is a WIP project and it can break suddenly, check support section below.

# Dependencies:
- Yocto typical dependencies see here: https://www.yoctoproject.org/docs/1.8/ref-manual/ref-manual.html
- Tested on UBUNTU 18-04 variant;
- This image was flashed in a raspberry pi 3 model B

# How to build
 - Clone this repository;
 - Cd to the repository root folder;
 - type:

 ```
 $ source poky/oe-init-build-env
 ```
 - You will appear inside a build folder, there are bblayers and local.conf files;
 - Navigate on top level folder to find the template of this files and override the generated;
 - Edit the paths but not the metas used;
 - Go back to the terminal, inside of build folder type:

 ```
 $ bitbake rpi-test-image
 ```
- Go to spend a day doing some interesting stuff :D ; 
- The built artifacts will appear in build/tmp/deploy/image/raspberryxxx
- flash the image on SDCARD, use this reference: https://www.lynxbee.com/flashing-rpi-yocto-images-to-sd-card-using-dd-making-sd-card-ready-to-boot-yocto-images-for-raspberry-pi/

- Enjoy to use ROS inside of raspberry.

# Support:
 - If you want some help with this work give a star and contact me: ryukokki.felipe@gmail.com