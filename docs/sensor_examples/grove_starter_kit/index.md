---
layout: default
title: Getting Started
---

<div id="toc" markdown="1">
* [Inside the Grove Starter Kit box »](#inside-the-grove-starter-kit-box)
* [Install the Grove Base Shield »](#install-the-grove-base-shield)
* [Connect a Grove component »](#connect-a-grove-component)
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


<div id="next-steps" class="note" markdown="1">
### Next Steps

<div class="link-button-container" markdown="1">
<span class="link-button-container-title">Try code samples:</span>
[Arduino »](arduino/index.html){: .link-button}
[JavaScript »](javascript/index.html){: .link-button}
[C++ »](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities#_Toc4){: .link-button}
</div>

</div>

<div class="callout goto" markdown="1">
### Additional resources

* Article: [Using MRAA to Abstract Platform I/O Capabilities](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities) 

* For PWM hardware configuration on the Arduino expansion board, refer to section 3.2 "Intel® Edison kit for Arduino* PWM swizzler" in the [Intel® Edison Kit for Arduino* Hardware Guide](http://www.intel.com/support/edison/sb/CS-035275.htm).
</div>