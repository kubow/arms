[How to burn .iso to USB drive - Linux.com](https://www.linux.com/training-tutorials/how-burn-iso-usb-drive/)
[RPi Easy SD Card Setup - eLinux.org](https://elinux.org/RPi_Easy_SD_Card_Setup)

- preparing OS to
	- SD card
	- Solid State Drive
	- internal FLASH (not all devices have this option)
## Apps

- [balenaEtcher - Flash OS images to SD cards & USB drives](https://www.balena.io/etcher)
- [Rufus - Create bootable USB drives the easy way](https://rufus.ie/en/) (win only)
- Win32DiskImager - very slow (win only) 
- imagewriter @ [openSUSE Software](https://software.opensuse.org/package/imagewriter)
- [Tools for OSForensics - ImageUSB - Write an image to multiple USB Flash Drives](https://www.osforensics.com/tools/write-usb-images.html)
- SuseStudio - a lot r/w errors
- [SD Memory Card Formatter | SD Association](https://www.sdcard.org/downloads/formatter/)
- [UNetbootin - Homepage and Downloads](http://unetbootin.github.io/)

## Linux way

```shell
cat /proc/partitions  # list available partitions  
sudo fdisk -l (df -h)  # show all connected devices  
fdisk /dev/sdx  
card=/dev/sdx  # assign variable from previous command  
sudo dd if=/dev/zero of=${card} bs=1024 seek=544 count=128  # clean the card  
sudo dd if=<file>.img/raw of=$card bs=1024 seek=8  # write SD card  
sync  # before unmount
```


## win way

- WIN+R --> cmd  
```cmd
Diskpart  
List disk  
Select disk #  
List partition  
Select partition #  
Delete partition  
Create partition primary
```
  - Computer management -> Storage -> Disk Management  
  - [SDB:Create a Live USB stick using Windows - openSUSE Wiki](https://en.opensuse.org/SDB:Create_a_Live_USB_stick_using_Windows)

## fdisk

```shell
# fdisk help  
# m - help  
# p - for partitions  
# d - delete partition(s)  
# choose number  
# n - new partition  
# w - write changes and quit
```


### Quality

Repair SD card [http://superuser.com/questions/485756/how-do-i-repartition-an-sdhc-card-in-windows](http://superuser.com/questions/485756/how-do-i-repartition-an-sdhc-card-in-windows)  
[http://ubuntuforums.org/showthread.php?t=2305402](http://ubuntuforums.org/showthread.php?t=2305402)  


Testing SD Card integrity [https://www.youtube.com/watch?v=qnezKfCTO7E](https://www.youtube.com/watch?v=qnezKfCTO7E)  
h2testw - windows only - [https://fightflashfraud.wordpress.com/2008/11/24/h2testw-gold-standard-in-detecting-fake-capacity-flash/](https://fightflashfraud.wordpress.com/2008/11/24/h2testw-gold-standard-in-detecting-fake-capacity-flash/)  
Detect USB problems [https://sosfakeflash.wordpress.com/2008/09/02/h2testw-14-gold-standard-in-detecting-usb-counterfeit-drives/comment-page-3/#comment-9861](https://sosfakeflash.wordpress.com/2008/09/02/h2testw-14-gold-standard-in-detecting-usb-counterfeit-drives/comment-page-3/#comment-9861)  
- [f3 - Fight Flash Fraud — f3 8.0 documentation](https://fight-flash-fraud.readthedocs.io/en/latest/introduction.html)
  
Create bootable SD for cubietruck [https://blog.night-shade.org.uk/2013/12/create-a-bootable-sd-for-a-cubietruck/](https://blog.night-shade.org.uk/2013/12/create-a-bootable-sd-for-a-cubietruck/)


### Flashing

[Tutorial: Manually installing Android ADB USB Driver](https://visualgdb.com/KB/usbdebug-manual/)
Livesuit cubieboard install guide [http://docs.cubieboard.org/tutorials/common/livesuit_installation_guide](http://docs.cubieboard.org/tutorials/common/livesuit_installation_guide)  
LiveSuit on Fedora [http://linux-sunxi.org/LiveSuit](http://linux-sunxi.org/LiveSuit)  
Proper drivers install [http://www.slatedroid.com/topic/53170-correct-installation-phoenixsuit-usb-drivers-in-win-8/](http://www.slatedroid.com/topic/53170-correct-installation-phoenixsuit-usb-drivers-in-win-8/)  
