---
layout: default
title: Getting Started
---

# JavaScript samples for the Grove Starter Kit

To follow the instructions in this guide, you should have already completed the [Set Up Intel XDK for IoT](/docs/ide_setup/xdk/setup.html) guide, and you can successfully [blink the onboard LED](/docs/ide_setup/xdk/create_project.html) on your Intel® Edison or Intel® Galileo.


<div class="toc" markdown="1">
**Table of contents**

* [Grove component types »](#grove-component-types)
  * [Digital outputs »](#digital-outputs)
  * [Digital inputs »](#digital-inputs)
  * [Analog inputs »](#analog-inputs)
  * [Analog outputs »](#analog-outputs)
  * [I2C »](#i2c)
</div>

<div class="related-videos" markdown="1">
**Related video**

* [Create Intel® IoT projects with the Grove Starter Kit - Part 2: JavaScript (preview)](https://drive.google.com/open?id=0B6gHgawzKtxCZU56NmJfei1GX00&authuser=0)
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
var mraa = require('mraa');

var led = new mraa.Gpio(6);  // set up digital read on digital pin #6
led.dir(mraa.DIR_OUT);  // set the GPIO direction to output

led.write(1);  // set the digital pin to high (1)
```

**Higher level UPM example:**

```
var groveSensor = require('jsupm_grove');

var led = new groveSensor.GroveLed(6); // set up digital output on digital pin #6

led.on();                              // set the digital pin to high
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
var mraa = require('mraa');

var button = new mraa.Gpio(5);     // set up digital read on digital pin #5
button.dir(mraa.DIR_IN);           // set the GPIO direction to input

var buttonState = button.read();   // read the value of the digital pin
console.log(buttonState);          // write the value to the console for debugging
```

**Higher level UPM example:**

```
var groveSensor = require('jsupm_grove');

var button = new groveSensor.GroveButton(5); // set up digital input on pin #5

var buttonState = button.value();  // read the value of the digital pin
console.log(buttonState);          // write the value to the console for debugging
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
var mraa = require('mraa');

var light = new mraa.Aio(0);     // set up analog input on analog pin #0 (A0)

var lightValue = light.read();   // read the value of the analog pin
console.log(lightValue);         // write the value to the console for debugging
```

**Higher level UPM example:**

```
var groveSensor = require('jsupm_grove');

var light = new groveSensor.GroveLight(0); // set up analog input on pin #0 (A0)

var lightValueRaw = light.raw_value();     // read the raw value of the analog pin
var lightValue = light.value();            // read the converted value of the pin
console.log(lightValueRaw, lightValue);    // write values to console for debugging
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
var mraa = require("mraa");

var led = new mraa.Pwm(3);  // initialize PWM on digital pin #3

led.write(0.5);             // make LED half brightness

///--- below example: fade over time ---

var brightness = 1;
var fadeInterval;

function fade(){
  led.write(brightness);
  brightness -= 0.01;
  if (brightness < 0) clearInterval(fadeInterval);
}

fadeInterval = setInterval(fade, 100);
```

**Higher level UPM example:**

Please see: [https://github.com/intel-iot-devkit/upm/blob/master/examples/javascript/es08a.js](https://github.com/intel-iot-devkit/upm/blob/master/examples/javascript/es08a.js)


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
var jsUpmI2cLcd  = require ('jsupm_i2clcd');
 
var lcd = new jsUpmI2cLcd.Jhd1313m1(6, 0x3E, 0x62); // Initialize the LCD

lcd.setCursor(0,1); // go to the 1st row, 2nd column (0-indexed)
lcd.write("hello"); // print characters to the LCD screen
```

---

### Next Steps

You're done! Now make your own creation. 

Return back to [START HERE »](/docs/arduino_expansion_board.html#now-make-your-own-creation)