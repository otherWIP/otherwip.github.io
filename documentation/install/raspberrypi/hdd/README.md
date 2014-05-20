 sudo nano /media/hdd/etc/inittab
 
 
 NEW SCRIPT
Boot up Pi with the hdd connected but without any other drives connected


    sudo tune2fs -U random -L hdd  /dev/sda2
    sudo mkdir /media/hdd
    sudo mount /dev/sda2 /media/hdd
    sudo mv /media/hdd/etc/fstab /media/hdd/etc/fstab.orig
    sudo sh -c "echo 'proc            /proc           proc    defaults              0    0' >> /media/hdd/etc/fstab"
    sudo sh -c "echo '/dev/mmcblk0p1  /boot           vfat    defaults              0    2' >> /media/hdd/etc/fstab"
    sudo sh -c "echo '/dev/sda2       /               ext4    defaults,noatime      0    1' >> /media/hdd/etc/fstab"
    sudo sh -c "echo '# a swapfile is not a swap partition, so no using swapon|off from here on, use  dphys-swapfile swap[on|off]  for that' >> /media/hdd/etc/fstab"
    sudo sh -c "echo ' ' >> /media/hdd/etc/fstab"
    sudo sh -c 'echo "dwc_otg.lpm_enable=0 console=tty1 root=/dev/sda2 rootfstype=ext4 elevator=deadline rootwait" > /boot/cmdline.txt'
    
Then *(sort /etc/inittab)* restart

    sudo shutdown -r now


    sudo apt-get update
    sudo apt-get upgrade -y


would be nice to have 

a) a script to add hdd using raspbian on hdd + single script

b) a script to add hdd using wget

c) a ro + hdd script in one command

d) a ro emonhub image with "add hdd" facilities
