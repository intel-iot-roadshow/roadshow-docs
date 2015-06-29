---
layout: default
title: Getting Started
---

# Set Up Ethernet over USB - Linux

When you are in a busy or restricted network environment, connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB". Ethernet over USB uses the RNDIS protocol.

This document will guide you through obtaining an IP address for the Intel® Edison in order to program your board offline using the Intel® IoT Developer Kit IDEs.


<div class="toc" markdown="1">
**Table of contents**

* [Forward usb0 connection »](#forward-usb0-connection)
* [Share your computer's WiFi connection (optional) »](#share-your-computers-wifi-connection-optional)
</div>

## Forward usb0 connection

Use Terminal and the `ifconfig` command to forward connections to the IP address 192.168.2.2 through "usb0" which should be the USB cable. [View detailed instructions »](details-forward_usb0.html)


## Share your computer's WiFi connection (optional)

Turn on Internet Sharing to cut down on Wi-Fi traffic in a crowded room. Sharing your computer's internet connection also means that you can log into networks that have HTML password pages and then share the connection with the Intel® Edison. Internet sharing is an optional step but is highly recommended if you are at a hackathon. [View detailed instructions »](details-share_internet.html)


### Additional Resources

See what you can do [once connected »](/docs/connectivity/ethernet_over_usb/shared/once_connected.html)

---

### Next Steps

Based on your programming language preference, install an IDE for Intel® IoT development:

* **For C/C++:**
  * [Set Up IoT Dev Kit Eclipse »](/docs/ide_setup/eclipse/)

* **For JavaScript:**
  * [Set Up Intel XDK for IoT »](/docs/ide_setup/xdk/)
