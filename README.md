# ipu6-camera-bins

This repository supports MIPI cameras through the IPU6 on Intel Tiger Lake and
Alder Lake platforms. There are 4 repositories that provide the complete setup:

- https://github.com/intel/ipu6-drivers - kernel drivers for the IPU and sensors
- https://github.com/intel/ipu6-camera-hal - HAL for processing of images in userspace
- https://github.com/intel/ipu6-camera-bins - IPU firmware and proprietary image processing libraries
- https://github.com/intel/icamerasrc (branch:icamerasrc_slim_api) - Gstreamer src plugin

## Content of this repository:
- IPU6 firmware
- IPU6ep firmware
- Library binary dependencies for IPU6 HAL
- Header files for those libraries

## Deployment
ipu6-camera-bins should be copied to build server and target
```shell
cp -r ipu6-camera-bins/<IPU_VER>/include/* /usr/include/
cp -r ipu6-camera-bins/<IPU_VER>/lib/* /usr/lib/
```
