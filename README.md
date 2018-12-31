# led_device_driver
device driver for led

## Demonstration
https://www.youtube.com/watch?v=9zPbc1hHtWc&feature=youtu.be

## Requirements
* Raspberry Pi 3 Model B+
 * Raspbian

* Linux Kernel Source
 * download kernel source into /user/src/linux
 * kernel build scripts : https://github.com/ryuichiueda/raspberry_pi_kernel_build_scripts.git
 
* 2 LEDs
 * connected with 23 and 24 pins
 
## Usage
* cd led_device_driver
* make
* sudo insmod myled.ko
* sudo chmod 666 /dev/myled0
* echo 1 > /dev/myled0 //flash
* echo 0 > /dev/myled0 //solid
* echo 2 > /dev/myled0 //flash
* sudo rm /dev/myled0
* sudo rmmod myled

## Licence
This repository is licensed under the GPLv3 license
