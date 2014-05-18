---
title: RaspberryPi Install
tags: 
categories: 
published: True
layout: default
js: index
---

##**Installing EmonHub to Raspberry Pi**

-----------------------------------

####***Prerequisites***
There are numerous ways to set-up and configure a Pi to run emonHub so before installing emonhub it's worth weighing up the best approach, if emonhub is going to be running 24/7 to give continuous reporting thats alot of data points and the life of an SD card can be significantly reduced by constantly writing to it. Therefore the recommendation is to either protect the SD card by configuring it to be "Read-Only" or to use a harddrive in place of the SD card.

#### Configure as ReadOnly

#### Add a hardrive

Installing emonHub to a RaspberryPi using the Debian Package Installer is really quite straight forward. After adding the location of the software, just tell it to install, the installer asks you some questions and in many cases offers default values, then once it has the info confirmed it will prepare everything for you.

----------

##{% include step/add-repo.md dist="wheezy"%}

----

##{% include step/add-deb.md pack="emonhub"%}

---

Follow the set-up screens

-----------------------------

Adding a RFM2Pi

Create a RO image

#### [Set up RaspberryPi hdd]({{site.page}}install/raspberrypi/hdd)

#### [Set up RaspberryPi hdd]({%include page/rpi-hdd%})





