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

There are numerous ways to set-up and configure a Pi to run emonHub so before installing emonhub it's worth weighing up the best approach, if emonhub is going to be running 24/7 to give continuous reporting that's a lot of data points and the life of an SD card can be significantly reduced by constantly writing to it. Therefore the recommendation is to either protect the SD card by configuring it to be "Read-Only" or to use a hard drive in place of the SD card.

##### **Configure SD card as Read Only**

This method basically locks down the SD card so nothing can be written to it, all the processing and temporary files are stored in the RAM. Ideally suited to a situation where the Pi is forwarding data to a remote emonCMS server. The hardware remains compact as there is no additional hardrive and it's simple, reliable and cheap. A read-only solution cannot store data or host emonCMS, emonHub will however buffer data in the Pi's relatively small memory so that short interval network interruptions and server outages do not cause loss of data. All data in the buffer is lost if the Pi losses power.

##### **Use a HDD in place of SD card**

Installing to a hard drive greatly improves the Pi's ability to store and access data, this is definitely the best option if you intend to install an emonCMS server and database to the Pi.

Installing emonHub to a Raspberry Pi using the Debian Package Installer is really quite straight forward. After adding the location of the software, just tell it to install, the installer asks you some questions and in many cases offers default values, then once it has the info confirmed it will prepare everything for you.

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





