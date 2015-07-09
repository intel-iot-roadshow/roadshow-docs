---
layout: default
title: Getting Started
---

# C++ samples for the Grove Starter Kit

To follow the instructions in this guide, should have already completed the [Set Up IoT Dev Kit Eclipse »](/docs/ide_setup/eclipse/setup.html) guide, and you can successfully [blink the onboard LED](/docs/ide_setup/eclipse/create_project.html) on your Intel® Edison or Intel® Galileo.

<div class="toc" markdown="1">
**Table of contents**

* [Grove component types »](#grove-component-types)
  * [Digital outputs »](#digital-outputs)
  * [Digital inputs »](#digital-inputs)
  * [Analog inputs »](#analog-inputs)
  * [Analog outputs »](#analog-outputs)
  * [I2C »](#i2c)
</div>

## Grove component types

The simpler components in the Grove Starter Kit fall into 2 categories: input or output. These two categories further subdivide into digital or analog. 

Other components in the Grove Starter Kit may use more complex communications protocols such as UART or I2C.

Identifying which category a component falls under is required in order to correctly attach the component to the Grove Base Shield and to understand what code library and commands are needed to control the component.


### Digital outputs

A digital output can write a value of either on (1) or off (0).

Connect to any pin labelled "D" (for "digital") on the Grove Base Shield such as D2 to D8.

<table>
  <tr>
    <td>Grove LED Socket Kit</td>
    <td>Grove Smart Relay</td>
  </tr>
  <tr>
    <td>UPM sample code</td>
    <td>UPM sample code</td>
  </tr>
  <tr>
    <td>require('jsupm_grove')</td>
    <td>require('jsupm_grove')</td>
  </tr>
</table>

**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

```

```

If you want to make the LED turn on and off, add a setTimeout() or setInterval() to toggle between writing 1 or 0 to the digital pin.  

### Digital inputs

A digital input can read a value as either on (1) or off (0).

Connect to any pin labelled "D" (for "digital") such as D2 to D8 on the Grove Base Shield.

<table>
  <tr>
    <td>Grove Button</td>
    <td>Grove Touch Sensor (TTP223)</td>
  </tr>
  <tr>
    <td>UPM code samples</td>
    <td>UPM code samples</td>
  </tr>
  <tr>
    <td>require('jsupm_grove')</td>
    <td>require('jsupm_ttp223')</td>
  </tr>
</table>

**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

```

```

To react to button press beyond application startup, add a `setTimeout()` or `setInterval()` to periodically poll the pin state.

### Analog inputs

An analog input will read a value as between 0 and 1024.

Connect to any pin labelled "A" (for "analog") on the Grove Base Shield such as A0 to A3.

<table>
  <tr>
    <td>Grove Light Sensor</td>
    <td>Grove Rotary Angle</td>
    <td>Grove Temperature</td>
    <td>Grove Sound Sensor</td>
  </tr>
  <tr>
    <td>UPM code samples</td>
    <td>UPM code samples</td>
    <td>UPM code samples</td>
    <td>UPM code samples</td>
  </tr>
  <tr>
    <td>require('jsupm_grove')</td>
    <td>require('jsupm_grove')</td>
    <td>require('jsupm_grove')</td>
    <td>require("jsupm_mic")</td>
  </tr>
</table>


**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

```

```

To react to changes in light beyond application startup, add a `setTimeout()` or `setInterval()` to periodically poll the sensor value.

### Analog outputs

An analog output is a digital output in disguise. Intel® IoT boards are digital microcontrollers that can pretend to be analog using a concept called Pulse Width Modulation (PWM). 

Analog outputs will accept a floating-point value representing a duty cycle percentage between 0 (always off), 1.0 (always on). For example, a value of 0.5 will rapidly pulse equally between on and off.

Components will only work when connected to PWM-enabled pins! By factory default, these PWM pins are D3, D5, and D6. (Digital pin #9 is also available on the Arduino expansion board via the standard female header pin.)

<table>
  <tr>
    <td>Grove LED Socket Kit</td>
    <td>Grove Buzzer</td>
    <td>Grove Servo Motor (ES08A)</td>
  </tr>
  <tr>
    <td>(no UPM sample)</td>
    <td>UPM sample code</td>
    <td>UPM sample code</td>
  </tr>
  <tr>
    <td></td>
    <td>require("jsupm_buzzer")</td>
    <td>require("jsupm_servo")</td>
  </tr>
</table>


**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

Please see: [https://github.com/intel-iot-devkit/upm/blob/master/examples/c++/es08a.js](https://github.com/intel-iot-devkit/upm/blob/master/examples/c++/es08a.js)


### I2C

I²C (Inter-Integrated Circuit), pronounced both "I-two-C" or "I-squared-C", is a multi-master, multi-slave, single-ended, serial computer bus used for attaching lower-speed peripherals to processors on computer motherboards and embedded systems.

<table>
  <tr>
    <td>Grove LCD RGB Backlight (JHD1313M1)</td>
  </tr>
  <tr>
    <td>UPM code samples</td>
  </tr>
  <tr>
    <td>require ('jsupm_i2clcd')</td>
  </tr>
</table>

**Higher level UPM example:**

```

```

---

### Next Steps

You're done! Now make your own creation. 

Return back to [START HERE »](/docs/arduino_expansion_board.html#now-make-your-own-creation)
