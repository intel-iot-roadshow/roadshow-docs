---
layout: default
title: Getting Started
---

# Shell Access - Linux

![computer icon with command prompt](../images/icon-computer_shell.png)

If you need to configure your IoT board, you will need to remotely connect to the Intel® Edison or Intel® Galileo. Once connected to your Intel® IoT board, you have access to the Linux-based Yocto operating system running on the board. 

You can then execute special Linux commands such: changing the hostname and password, setting up Wi-Fi, or flashing new firmware.

<div id="toc" class="box" markdown="1">
* [Install a shell session manager (Screen) »](#install-a-shell-session-manager-screen)
* [Establish a serial connection »](#establish-a-serial-connection)
</div>

## Install a shell session manager (Screen)

<div class="tldr" markdown="1">
Your computer may not have come with a pre-installed shell session manager. Download and install the GNU Screen utility using `sudo apt-get install screen`. 

[View detailed instructions »](details-install_screen.html)
</div>

## Establish a serial connection

<div class="tldr" markdown="1">
Use the Screen utility that you installed in the previous section to gain command line access of your IoT board. For example: `sudo screen /dev/ttyUSB0 115200`. 

[View detailed instructions »](details-screen_connection.html)
</div>

<br>

<div class="callout done" markdown="1">
You are now logged into your IoT board and can run shell commands. For example, to output the version number of the firmware running on your board:

```
cat /etc/version
```

![example output after running cat command](../images/firmware_version_output.png)

The firmware version is in YYYYMMDDHHMM format so, in this case, Sept 3, 2014.
</div>

<div class="callout goto" markdown="1">
For more info on using Screen such as quitting, read [Using Screen »](../mac-and-linux/using_screen.html)
</div>

<div id="next-steps" class="note" markdown="1">
### Next Steps

Get your board online in order to turn your IoT board into a true "Internet of Things" device. You also need the IP address of your IoT board to program it using the dev kit IDEs.


**At a hackathon? On a busy or restricted Wi-Fi network?**

Connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB":

* [Linux »](../../connectivity/ethernet_over_usb/linux/connect.html)

**At home? Have a dependable Wi-Fi connection?**

* [Get Your Edison Board Online »](../../connectivity/wifi/connect.html)
</div>