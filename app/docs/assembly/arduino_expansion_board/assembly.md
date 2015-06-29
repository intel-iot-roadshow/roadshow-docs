---
layout: default
title: Getting Started
---

# Unboxing and Assembly

Find out what is in your Intel® Edison Kit for Arduino box. Some assembly is required. ;)

<div class="toc" markdown="1">
**Table of contents**

* [Look in the Intel® Edison Kit for Arduino box »](#look-in-the-intel-edison-kit-for-arduino-box)
* [Quick Start Assembly Instructions »](#quick-start-assembly-instructions)
  * [Install the Intel® Edison module »](#install-the-intel-edison-module)
  * [Install the plastic spacers »](#install-the-plastic-spacers)
* [Example of a full development setup »](#example-of-a-full-development-setup)
</div>

<div class="related-videos" markdown="1">
**Related video**

[![Intel Edison Kit for Arduino: Unboxing and Assembly - screenshot](images/video_screenshot-unboxing_assembly.png)](https://software.intel.com/en-us/videos/intel-edison-kit-for-arduino-unboxing-and-assembly)
</div>

## Look in the Intel® Edison Kit for Arduino box

![Closed Intel® Edison retail box](images/retail_box.png)

![Unpacked Intel® Edison retail box](images/retail_box-unpacked.png)

* **Intel® Edison compute module**
  
  Refer to the [product brief](http://www.intel.com/support/edison/sb/CS-035277.htm) for specs. 

* **Intel® Edison kit for Arduino expansion board.**
  
  Software and hardware pin-compatible with Arduino Uno R3 shields. Refer to the [hardware guide](http://www.intel.com/support/edison/sb/CS-035275.htm) for specs.

* **Small hex nuts (x2)**
  
  For attaching the Intel® Edison module to the expansion board.

* **Screws (x4) & plastic spacers (x4)**
  
  To keep the expansion board stable and lifted off of surfaces.


## Quick Start Assembly Instructions


### Install the Intel® Edison module

<div class="tldr" markdown="1">
The Intel® Edison module is meant to be used with breakout boards or custom PCBs. You will need to secure your Intel® Edison module to the Arduino expansion board before you can use it. [View detailed instructions »](details-install_module.html)
</div>

![Animated gif: installing the Intel® Edison module](images/module_install-animated.gif)


### Install the plastic spacers

<div class="tldr" markdown="1">
To add stability to the expansion board and to help avoid accidental short circuits, attach the four plastic spacers supplied in your Intel® Edison box to act as "legs" for the expansion board. [View detailed instructions »](details-install_spacers.html)
</div>

![Animated gif: installing the plastic spacers](images/spacer_install-animated.gif)


## Example of a full development setup

While plugging in every cable is not required at this very moment, a development setup with serial communication for shell access would look like this:

1. **microswitch** in "USB device mode" (i.e. toggled **_down_** towards the micro-USB ports)

2. **device mode micro-USB cable** plugged into your computer

3. **UART/serial micro-USB cable** plugged into your computer

The Arduino expansion board for Intel® Edison can be powered via the DC power jack, the device mode micro-USB port, or both. This setup uses only a micro-USB cable for power.

![Cable and microswitch setup for Intel® Edison development](images/cables-full_dev_setup.png)

<div class="next-steps" markdown="1">
### Next Steps

Explore when and how to use all the cables ports on the Intel® Edison kit for Arduino: [Connecting Cables »](connecting_cables.html)
</div>

<div class="footnote">
* The Arduino name, logo and the graphics design of its boards are a protected trademark of Arduino and its partners.
</div>