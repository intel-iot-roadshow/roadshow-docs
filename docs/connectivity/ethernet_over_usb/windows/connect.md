---
layout: default
title: Getting Started
---

<div id="toc" markdown="1">
* [Add static IPv4 address »](#add-static-ipv4-address)
* [Share your computer's WiFi connection (optional) »](#share-your-computers-wifi-connection-optional)
</div>

# Set Up Ethernet over USB - Windows

When you are in a busy or restricted network environment, connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB". Ethernet over USB uses the RNDIS protocol.

This document will guide you through obtaining an IP address for the Intel® Edison in order to program your board offline using the Intel® IoT Developer Kit IDEs.

<!-- <div id="related-videos" class="callout video">
[Ethernet over USB - Intel Edison - Windows (preview)](https://drive.google.com/open?id=0B2ywC78pxngCUWJxZXJiYngycU0&authuser=0)
</div> -->

## Add static IPv4 address

<div class="tldr" markdown="1">
If you have the Intel® Edison Drivers installed, update your computer's Network Adapter configuration with a static IP address to use Ethernet over USB. 
</div>

[![Animated gif: adding static IPv4 address in Windows](){: .animated data-still="images/ipv4_windows-sampleframe.jpg" data-animated="images/ipv4_windows-animated.gif"}](details-ipv4_address.html)

[View detailed instructions »](details-ipv4_address.html){: .link-button .centered }


## Share your computer's WiFi connection (optional)

<div class="tldr" markdown="1">
Turn on Internet Connection Sharing (ICS) to cut down on Wi-Fi traffic in a crowded room. Sharing your computer's internet connection also means that you can log into networks that have HTML password pages and then share the connection with the Intel® Edison. Internet sharing is an optional step but is highly recommended if you are at a hackathon. 
</div>

[View detailed instructions »](details-share_internet.html){: .link-button .centered }


<div class="callout done" markdown="1">
See what you can do [once connected »](../shared/once_connected.html)
</div>


<div id="next-steps" class="note" markdown="1">
### Next Steps

Based on your programming language preference, install an IDE for Intel® IoT development:

* **For C/C++:** [Set Up IoT Dev Kit Eclipse »](../../../ide_setup/eclipse/setup.html)
* **For JavaScript:** [Set Up Intel XDK for IoT »](../../../ide_setup/xdk/setup.html)
* **For Arduino:** [Set Up Arduino IDE »](../../../ide_setup/arduino/setup.html)
</div>