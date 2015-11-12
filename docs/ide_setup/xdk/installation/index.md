---
layout: default
title: Intel® XDK IoT Edition - Standalone Installation
---

<div id="toc" markdown="1">
* [Install Intel® XDK IoT Edition »](#install-intel-xdk-iot-edition)
  * [Windows only: Install Bonjour »](#windows-only-install-bonjour)
* [Launch and sign into Intel® XDK »](#launch-and-sign-into-intel-xdk)
</div>

# Set Up Intel® XDK IoT Edition - Standalone Installation

The [Intel® XDK IoT Edition](https://software.intel.com/en-us/html5/xdk-iot) lets you create and test applications on Intel® IoT platforms. It uses NodeJS to communicate with all the GPIOs, libraries, and packages. The IoT edition also provides NodeJS templates for creating new applications that interact with sensors and actuators, enabling you to get a quick start on developing for the Internet of Things. 

This document will guide you through installing the Intel® XDK IoT Edition IDE for Intel® Edison development.

## Install Intel® XDK IoT Edition

<div class="tldr" markdown="1">
Get the latest Intel® XDK IoT Edition installer from <span class="icon folder">downloads</span> → <span class="icon folder">[your OS]</span> → <span class="icon folder">edison_media</span>. Simply run the installer and follow the prompts.
</div>

<figure markdown="1">
[![Animated gif: installing the Intel® XDK](){: .animated data-still="images/install_xdk-sampleframe.jpg" data-animated="images/install_xdk-animated.gif"}](details-install_xdk.html)
<figcaption>Example installation on Mac OSX</figcaption>
</figure>

<div class="link-button-container" markdown="1">
<span class="link-button-container-title">View detailed instructions for your operating system:</span>
[Windows »](details-install_xdk-windows.html){: .link-button}
[Mac »](details-install_xdk-mac.html){: .link-button}
[Linux »](details-install_xdk-linux.html){: .link-button}
</div>

### Windows only: Install Bonjour

<div class="tldr" markdown="1">
[Bonjour](http://support.apple.com/kb/DL999) (or zeroconf) is a service that enables the Intel® XDK to auto detect Intel® IoT devices on your network. This service is already available on Mac and Linux; only Windows users need to install an additional Bonjour service. 
</div>

[![Animated gif: installing Bonjour](){: .animated data-still="images/install_bonjour-sampleframe.jpg" data-animated="images/install_bonjour-animated.gif"}](details-install_bonjour.html)

[View detailed instructions for Windows »](details-install_bonjour.html){: .link-button .centered}


## Launch and sign into Intel® XDK

<div class="tldr" markdown="1">
Before you can use the Intel® XDK, you must sign up for an Intel® XDK account or log in to a pre-existing account. 
</div>

[![Animated gif: launching Intel® XDK for the first time](){: .animated data-still="images/launch_xdk-sampleframe.jpg" data-animated="images/launch_xdk-animated.gif"}](details-launch_xdk.html)

[View detailed instructions »](details-launch_xdk.html){: .link-button .centered}


<div id="next-steps" class="callout goto" markdown="1">
You should now have the Intel® XDK IoT Edition installed. Next, create and run a Hello Word project (blinking the onboard LED) on the Intel® Edison.

[Run a Sample Intel® XDK for IoT Project »](../sample_project/index.html){: .link-button .centered}
</div>
