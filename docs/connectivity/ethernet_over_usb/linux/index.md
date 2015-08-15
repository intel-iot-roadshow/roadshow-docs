---
layout: default
title: Getting Started
---

<div id="toc" markdown="1">
* [Forward usb0 connection »](#forward-usb0-connection)
* [Share your computer's WiFi connection (optional) »](#share-your-computers-wifi-connection-optional)
</div>

# Set Up Ethernet over USB - Linux

When you are in a busy or restricted network environment, connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB". Ethernet over USB uses the RNDIS protocol.

This document will guide you through obtaining an IP address for the Intel® Edison in order to program your board offline using the Intel® IoT Developer Kit IDEs.

## Forward usb0 connection

<div class="tldr" markdown="1">
Use Terminal and the `ifconfig` command to forward connections to the IP address 192.168.2.2 through "usb0" which should be the USB cable. 
</div>

[View detailed instructions »](details-forward_usb0.html){: .link-button .centered}


## Share your computer's WiFi connection (optional)

<div class="tldr" markdown="1">
Turn on Internet Sharing to cut down on Wi-Fi traffic in a crowded room. Sharing your computer's internet connection also means that you can log into networks that have HTML password pages and then share the connection with the Intel® Edison. Internet sharing is an optional step but is highly recommended if you are at a hackathon. 
</div>

[View detailed instructions »](details-share_internet.html){: .link-button .centered}


<div class="callout done" markdown="1">
See what you can do [once connected »](../shared/once_connected.html)
</div>


<div id="next-steps" class="note" markdown="1">
### Next Steps

Based on your programming language preference, install an IDE for Intel® IoT development:

* **For C/C++:** [Set Up IoT Dev Kit Eclipse »](../../../ide_setup/eclipse/index.html){: .link-button}
* **For JavaScript:** [Set Up Intel XDK for IoT »](../../../ide_setup/xdk/index.html){: .link-button}
* **For Arduino:** [Set Up Arduino IDE »](../../../ide_setup/arduino/index.html){: .link-button}
</div>
