_this code has been forked from https://github.com/AtlasScientific/Raspberry-Pi-sample-code and is now maintained separately, optimised for Whitebox carrier boards_ 

# Preparing the Raspberry Pi #
### Install the latest Raspberry Pi OS
Follow the instructions on this page to get Raspberry Pi OS running
https://www.raspberrypi.org/downloads/raspberry-pi-os/

### Expand file system
    
Expand file system by following this:
https://www.raspberrypi.org/documentation/configuration/raspi-config.md

### Update and Upgrade Packages 
    
    sudo apt-get update
    sudo apt-get upgrade

# Download sample code.
    
    cd ~
    git clone https://github.com/whitebox-labs/whitebox-raspberry-ezo.git


# I2C MODE #

### Enable I2C bus on the Raspberry Pi ###

Enable I2C bus on the Raspberry Pi by following this:

https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup/configuring-i2c

You can confirm that the setup worked and sensors are present with the `sudo i2cdetect -y 1` command.

### Test Sensor ###
    
Run the sample code below:
    
    cd ~/Raspberry-Pi-sample-code
    sudo python i2c.py

When the code starts up a list of commands will be shown.

For more details on the commands & responses, please refer to the Datasheets of the Atlas Scientific Sensors.
 
Note that it may be a different ttyAMA depending on your setup

