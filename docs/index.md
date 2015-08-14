---
layout: default
title: Getting Started
---

![Arduino Expansion Board with Intel® Edison](images/arduino_expansion_board_with_edison.png)

# How to go from Zero to Blinking Light Hero

_Instructions for **Intel® Edison** installed on an **Arduino-compatible expansion board** using the Intel® IoT Developer Kit **(C/C++, JavaScript or Arduino development workflow)**_


## 1. Get Started with Intel® Edison

Find out what hardware is included with your Intel® IoT Developer Kit ("dev kit"). And review important assembly and cable hook up instructions.

[Assemble your Arduino expansion board »](assembly/arduino_expansion_board/index.html){: .link-button .centered}


## 2. Set Up Your Computer

Install software and drivers specifically for your computer's operating system. 

**Mac or Linux user?** You have no special setup. Skip to Step 3.

<div class="link-button-container" markdown="1">
<span class="link-button-container-title">**Windows user?** Install software and drivers for Windows.</span>
[Install on Windows »](computer_setup/windows/index.html){: .link-button}
</div>


## 3. Flash Edison Firmware

Some Edison boards have older firmware images on them. You **_may_** need to update the firmware to a newer version to get access to important features.

<div class="link-button-container" markdown="1">
<span class="link-button-container-title">Install the Flashing Tool for:</span>
[Windows »](flash_firmware/windows/index.html){: .link-button}
[Mac »](flash_firmware/mac/index.html){: .link-button}
[Linux »](flash_firmware/linux/index.html){: .link-button}
</div>


## 4. Shell Access

Gain command line access of your IoT board. Execute special Linux commands to configure your IoT board such as setting up Wi-Fi.

* [Windows »](shell_access/windows/serial_connection.html)
* [Mac »](shell_access/mac/serial_connection.html)
* [Linux »](shell_access/linux/serial_connection.html)


## 5. Get Your IoT Board Online

Get your board online in order to turn your IoT board into a true "Internet of Things" device. You also need the IP address of your IoT board to program it using the dev kit IDEs.
  
**Connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB":**
  
  * [Windows »](connectivity/ethernet_over_usb/windows/connect.html)
  * [Linux »](connectivity/ethernet_over_usb/linux/connect.html)
  * Note: At this time, Ethernet over USB on Mac is not officially supported.

**At home? Have a dependable Wi-Fi connection?**

  * [Connect Your Intel Edison to Wi-Fi »](connectivity/wifi/connect.html)


## 6. Install an IDE

Based on your programming language preference, install an IDE for Intel® IoT development:

* **For JavaScript:** [Set Up Intel XDK for IoT »](ide_setup/xdk/setup.html)
* **For C/C++:** [Set Up IoT Dev Kit Eclipse »](ide_setup/eclipse/setup.html)
* **For Arduino:** [Set Up Arduino IDE »](ide_setup/arduino/setup.html)

## 7. Sensor Tutorials

Experiment with sample code supplied for available sensors and actuators.

* **[Grove Starter Kit - Intro »](sensor_examples/grove_starter_kit/index.html)**
  * [JavaScript »](sensor_examples/grove_starter_kit/javascript/samples.html)
  * [C++ »](https://software.intel.com/en-us/working-with-sensors-in-eclipse)

Also search for your component on [software.intel.com/en-us/iot/sensors](http://software.intel.com/en-us/iot/sensors).


## Now make your own creation!

Take pictures along the way. Create your own guide and post them to [Instructables.com](http://instructables.com/id/intel).


## Running into issues?

Search for answers and post your questions to the [Intel® Edison Support Community](https://communities.intel.com/community/tech/edison).


## Resources

* [Intel® Edison Product Brief](http://www.intel.com/support/edison/sb/CS-035277.htm) (Specs)
* [Intel® Edison Arduino Expansion Board Hardware Guide](http://www.intel.com/support/edison/sb/CS-035275.htm)
  * For pinout listing, see page 7
* [Intel® Edison Mini Breakout Board Hardware Guide](http://www.intel.com/support/edison/sb/CS-035252.htm)
  * For pinout listing, see page 9 
* [Yocto Project: Foundation for the Internet of Things](https://www.youtube.com/watch?v=ztsnQ3p59jA&list=PLg-UKERBljNw254jnyMNZiu8yqF8pPq0m&index=24) (Introduction to Yocto video)
* [Intel® IoT Developer Kit Cloud-based Analytics User Guide](https://software.intel.com/en-us/intel-iot-developer-kit-cloud-based-analytics-user-guide) 
* [Seeed Studio Sketchbook Starter Kit](https://github.com/Seeed-Studio/Sketchbook_Starter_Kit_V2.0) (Sensor sample code for Arduino IDE)
