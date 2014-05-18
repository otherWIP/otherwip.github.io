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

Pre-install considerations......

You should consider whether to [install to SD card or to HDD]({{site.page}}install/raspberrypi/sd_or_hdd) as it is highly recommended that emonHub is installed to a hardrive unless the SD card is configured as Read-Only.



Installing emonHub to a Raspberry Pi using the Debian Package Installer is really quite straight forward. After adding the location of the software, just tell it to install, the installer asks you some questions and in many cases offers default values, then once it has the info confirmed it will prepare everything for you.

----------

##{% include step/add-repo.md dist="wheezy"%}

----

##{% include step/add-deb.md pack="emonhub"%}

---

Follow the set-up screens

-----------------------------

Adding a RFM2Pi

