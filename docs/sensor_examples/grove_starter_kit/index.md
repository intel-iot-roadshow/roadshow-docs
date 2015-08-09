---
layout: default
title: Getting Started
---

<div id="toc" markdown="1">
* [Inside the Grove Starter Kit box »](#inside-the-grove-starter-kit-box)
* [Install the Grove Base Shield »](#install-the-grove-base-shield)
* [Connect a Grove component »](#connect-a-grove-component)
* [Programming Grove components »](#programming-grove-components)
  * [Install code libraries »](#install-code-libraries)
    * [MRAA »](#mraa)
    * [UPM »](#upm)
* [Find code samples »](#find-code-samples)
</div>

# Create Intel® IoT projects with the Grove Starter Kit

The Grove System is an easy to use group of modules that minimise the effort required to get started with microcontroller-based experimentation and learning. Intel® has partnered with [Seeed](http://seeedstudio.com), the creators of Grove, to distribute the [Grove Starter Kit Plus - Intel IoT Edition](http://www.seeedstudio.com/depot/Grove-starter-kit-plus-Intel-IoT-Edition-for-Intel-Galileo-Gen-2-and-Edison-p-1978.html) which contains essential sensor and actuator modules to jump start your IoT prototyping.

![The components in the Grove Starter Kit](images/components_in_huddle.png)

This guide will demonstrate how you can use the Grove Starter Kit with any Intel® IoT board to go beyond blinking the onboard LED.

<!-- <div id="related-videos" class="callout video">
* [Create Intel® IoT projects with the Grove Starter Kit - Part 1 (preview)](https://drive.google.com/open?id=0B6gHgawzKtxCNEhfNms3ai0zM1k&authuser=0)
</div> -->

## Inside the Grove Starter Kit box

The sensors and actuators in the Grove Starter Kit Plus – Intel® IoT Edition for Intel® Galileo Gen 2 work with both the Intel® Galileo and the Intel® Edison.

**Located in the plastic tray inside the green box:**

* Base Shield v2 (look underneath LCD)
* Grove LCD RGB Backlight
* Grove Buzzer
* Grove Sound Sensor
* Grove Touch Sensor
* Grove Temperature
* Grove Light Sensor
* Grove Rotary Angle
* Grove Button
* Grove LED Socket Kit
* Grove Smart Relay

**Look underneath the plastic tray:**

* Grove Servo Motor
* 26AWG Grove Cable (× 10)
* 9V to Barrel Jack Adapter - 126mm
* Red, green, and blue 3mm LEDs
* Grove Starter Kit manual

**Look elsewhere in the cardboard Grove box:**

* Micro-USB Cable
* Ethernet Cable
* 3.3V FTDI USB-to-Serial Cable
* 8GB microSD Card with an SD Card Adapter


## Install the Grove Base Shield

Arduino "shields" are add-ons that plug into standard Arduino header pin configurations. The use of shields allow for additional functionality without having to use an additional prototyping area such as a breadboard.

1. Unplug the Arduino expansion board from all power sources.

2. Line up the male header pins of the Grove Base Shield with the female pins on the Arduino expansion board. 

    Pin configurations of Arduino shields will only fit the Arduino expansion board in one direction so do not force the pins if they do not line up.

3. Push down firmly and evenly on both sides of the Grove Base Shield until the shield is securely installed.

4. Check the voltage toggle (marked VCC, next to A0) on the Grove Base Shield. It should be set to 5V. 

5. Power the expansion board back on. Allow 1 minute for your Intel® Edison or Intel® Galileo to finish booting up.


## Connect a Grove component 

All components in the Grove System use a 4-pin cable with JST connectors. This allows you to prototype without having to individually learn how to wire up each unique component.

1. Choose a component from the Grove System.

    See [Programming Grove components](#programming-grove-components) to help choose a component from the Grove Starter Kit.

2. Use a 4-pin Grove Cable and connect one end of the cable to the component.

    The cable connectors only fit in one direction so you can be confident that the wiring is correct.

3. For the other end of the cable, refer to the the Grove Shield labels for the correct pin to connect to.

    * Digital pins (D2-D8)
    * Analog pins (A0-A3)
    * I2C (bottom row)
    * UART (top right)


## Programming Grove components

### Install code libraries 

<div class="callout warning" style="margin-top: 1em;" markdown="1">
**Is your board online?** Your board must have an internet connection to install the code libraries with the following commands.
</div>

#### MRAA

Libmraa (pronounced "em-raah") is a C/C++ library (with bindings to JavaScript and Python) to interface with the GPIO pins on the Intel® Galileo, Intel® Edison, and other platforms. 

Intel® maintains the [MRAA library on Github](https://github.com/intel-iot-devkit/mraa). 

[C/C++ API documentation](http://iotdk.intel.com/docs/master/mraa/) and [JavaScript API documentation](http://iotdk.intel.com/docs/master/mraa/node/modules/mraa.html) can be found on intel.com.

1. Establish an SSH or serial connection to your Intel® Galileo or Intel® Edison. {% strip %}{% include shell_access.md %}{% endstrip %}

2. Run the following commands on your board. The first command will edit the mraa-upm config file on the board. The last two commands use the board's built-in Opkg package manager to download and update the missing library.

```
echo "src mraa-upm http://iotdk.intel.com/repos/1.1/intelgalactic" > /etc/opkg/mraa-upm.conf
```
```
opkg update
```
```
opkg install libmraa0
```

#### UPM

UPM is a higher level library that leverages libmraa for controlling more complex sensors or actuators. A supported sensor will have its own class file that needs to be imported into your project and instantiated. 

Intel® maintains the [UPM library on Github](https://github.com/intel-iot-devkit/upm). 

For code samples, look for your specific component on [software.intel.com/iot/hardware/sensors](http://software.intel.com/iot/hardware/sensors) or in the [examples](https://github.com/intel-iot-devkit/upm/tree/master/examples/) folder in the UPM Github repo.

1. Establish a serial connection to your Intel® IoT board, if you're not already connected.

2. Run the following command to use the board's built-in Opkg package manager to download and update the UPM library.

    ```
    opkg install upm
    ```


### Find code samples

1. To find code samples for your component, start by visiting the hardware sensors page at [software.intel.com/en-us/iot/hardware/sensors](https://software.intel.com/en-us/iot/hardware/sensors).

    1. Browse for supported components by paging through the list. Filter the results using the drop down menus on the page.

    2. Click on a component to view additional information and view code samples in C/C++, JavaScript, and Python (when available).

2. Alternatively, to find the most up-to-date UPM code samples, browse the UPM "examples" folder at [github.com/intel-iot-devkit/upm/tree/master/examples](https://github.com/intel-iot-devkit/upm/tree/master/examples).

    1. Go into the "c++", "javascript", or "python" folder and look for your component by model or part name.

## Grove component types

The simpler components in the Grove Starter Kit fall into 2 categories: input or output. These two categories further subdivide into digital or analog. 

Other components in the Grove Starter Kit may use more complex communications protocols such as UART or I2C.

Identifying which category a component falls under is required in order to correctly attach the component to the Grove Base Shield and to understand what code library and commands are needed to control the component.

<div id="next-steps" class="note" markdown="1">
### Next Steps

Try code samples in JavaScript or C++:

* [JavaScript »](javascript/samples.html)
* [C++ »](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities#_Toc4)
</div>

<div class="callout goto" markdown="1">
### Additional resources

* Article: [Using MRAA to Abstract Platform I/O Capabilities](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities) 

* For PWM hardware configuration on the Arduino expansion board, refer to section 3.2 "Intel® Edison kit for Arduino* PWM swizzler" in the Intel® Edison Kit for Arduino* Hardware Guide: http://www.intel.com/support/edison/sb/CS-035275.htm

* Sensor sample code for Arduino IDE: [Seeed Studio Sketchbook Starter Kit](https://github.com/Seeed-Studio/Sketchbook_Starter_Kit_V2.0)
</div>