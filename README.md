# raspberrypi

## installation of a wifi dongle on raspberry pi model B

dongle model : TP-Link TL-WN823N
if dongle is not detected :

    $ iwconfig  
    lo        no wireless extensions.  
    eth0      no wireless extensions.

    $ lsusb
    <doesn't give any results>

That means you need to install the driver :
https://raspberrypi.stackexchange.com/questions/54716/raspberry-1-no-wifi-dongle-detected-tp-link-tl-wn823n

You can download from the constructor, but you'll need to compile it, and so you need the linux kernels to do that. 
One usefull command is rpi-source

https://www.raspberrypi.org/forums/viewtopic.php?t=148389

https://www.raspberrypi.org/forums/viewtopic.php?f=29&t=76261

    sudo wget https://raw.githubusercontent.com/notro/rpi-source/master/rpi-source -O /usr/bin/rpi-source && sudo chmod +x /usr/bin/rpi-source && /usr/bin/rpi-source -q --tag-update
https://github.com/notro/rpi-source/wiki
