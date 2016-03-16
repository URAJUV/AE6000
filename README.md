## How to use this driver ##

* Unzip and cd AE6000-master

* run the following commands

1. Unplug Wifi dongle from USB

2. update your sources and upgrade if any
   sudo apt-get update
   sudo apt-get upgrade

3. install gnu compiler collection
   sudo apt-get install build-essential

4. lets install git

   sudo apt-get install git

5. get sources
   git clone https://github.com/URAJUV/AE6000.git

5.1 - if you have cloned already
   cd AE6000-master
   git pull

6. build driver

   cd AE6000-master
   make clean
   make
   sudo make install


There should not be any errors in last commands

7. After the last command connect your USB Wifi adapter to any USB port. Now it must have listed all visible wifi signals(SSIDs). Connect to internet
8. open a browser and test internet !!
```

Connect Linksys AE6000 Wifi Dongle to your PC / Laptop.. You will notice the led blinking.

For other chipsets some files need modification including the following

* Makefile
* os/linux/config.mk
* common/rtusb_dev_id.c
