http://www.raspberrypi.org/forums/viewtopic.php?f=29&t=22596

https://wiki.debian.org/ReadonlyRoot


To undo these changes and revert to the original set up run
    
    sudo mount -o remount,rw /dev/mmcblk0p2  /
    sudo mv /etc/default/rcS.orig /etc/default/rcS
    sudo mv /etc/fstab.orig /etc/fstab
    sudo mv /etc/mtab.orig /etc/mtab
    sudo rm /usr/bin/rpi-ro
    sudo rm /usr/bin/rpi-rw
    sudo shutdown -r now
