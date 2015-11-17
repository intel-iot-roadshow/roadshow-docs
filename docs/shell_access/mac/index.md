---
layout: default
title: Shell Access - Mac
---

<div id="toc" markdown="1">
* [Identify the "usbserial" device name »](#identify-the-usbserial-device-name)
* [Establish a serial connection »](#establish-a-serial-connection)
</div>

# Shell Access - Mac 

![computer icon with command prompt](../images/icon-computer_shell.png)

If you need to configure your IoT board, you will need to remotely connect to the Intel® Edison or Intel® Galileo. Once connected to your Intel® IoT board, you have access to the Linux-based Yocto operating system running on the board. 

You can then execute special Linux commands such: changing the hostname and password, setting up Wi-Fi, or flashing new firmware.


## Identify the "usbserial" device name 

<div class="tldr" markdown="1">
Use the `ls /dev/tty.*` command in Terminal to find the device name of the "**usbserial**" connection. You will need the exact device name for use in <span class="icon bookmark">Establish a serial connection</span> next. 
</div>

[![Animated gif: using Terminal to find the USB device name](){: .animated data-still="images/identify_usbserial-sampleframe.jpg" data-animated="images/identify_usbserial-animated.gif"}](details-identify_usbserial.html)

[View detailed instructions »](details-identify_usbserial.html){: .link-button .centered}


## Establish a serial connection

<div class="tldr" markdown="1">
Use the Screen utility in Terminal to gain command line access of your IoT board. For example: `screen /dev/tty.usbserial-A102GW3T 115200`. 
</div>

[![Animated gif: using Screen utility to connect to IoT board](){: .animated data-still="images/screen_connection-sampleframe.jpg" data-animated="images/screen_connection-animated.gif"}](details-screen_connection.html)

[View detailed instructions »](details-screen_connection.html){: .link-button .centered}


<div class="callout done" markdown="1">
You are now logged into your IoT board and can run shell commands. For example, try:

```
configure_edison --help
```
</div>


<div id="next-steps" class="callout done" markdown="1">
You should now be able to gain command line access to the Intel® Edison.

[Continue to the next step in the START HERE guide »](../../index.html#done-shell-access){: .link-button .centered}
</div>