---
layout: default
title: Getting Started
---

# C++ samples for the Grove Starter Kit

To follow the instructions in this guide, you should have already completed the [Set Up IoT Dev Kit Eclipse »](/docs/ide_setup/eclipse/setup.html) guide, and you can successfully [blink the onboard LED](/docs/ide_setup/eclipse/create_project.html) on your Intel® Edison or Intel® Galileo.

<div id="toc" class="box" markdown="1">
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

<div class="tldr" markdown="1">
A digital output can write a value of either on (`1`) or off (`0`).

Connect to any pin labeled "D" (for "digital") on the Grove Base Shield such as D2 to D8.
</div>

**Example components:**

* Grove LED Socket Kit
* Grove Smart Relay

**Low level MRAA-only example:**

```
#include "mraa.hpp"

int main()
{
  // set up GPIO digital pin #6
  mraa::Gpio* led = new mraa::Gpio(6, true, false);

  // set the GPIO direction to output
  led->dir(mraa::DIR_OUT);

  // set the digital pin to high (1)
  led->write(1);

  return MRAA_SUCCESS;
}
```

**Higher level UPM example:**

```
#include "grove.h"

int main()
{
  // use GroveLed class to set up GPIO digital pin #6
  // (internally sets direction to output)
  upm::GroveLed* led = new upm::GroveLed(6);

  // set the digital pin to high
  led->on();

  return MRAA_SUCCESS;
}
```

If you want to make the LED turn on and off, add a `for` loop to toggle between writing `1` or `0` to the digital pin. For example:

```
// loop forever to toggle the on board LED every second
for (;;) {
  led->write(1);
  sleep(1);
  led->write(0);
  sleep(1);
}
```  

### Digital inputs

<div class="tldr" markdown="1">
A digital input can read a value as either on (`1`) or off (`0`).

Connect to any pin labeled "D" (for "digital") such as D2 to D8 on the Grove Base Shield.
</div>

**Example components:**

* Grove Button
* Grove Touch Sensor (TTP223)

**Low level MRAA-only example:**

```
#include "mraa.hpp"
#include <stdio.h>

int main()
{
  // set up digital read on digital pin #5
  mraa::Gpio* button = new mraa::Gpio(5, true, false);

  // set the GPIO direction to input
  button->dir(mraa::DIR_IN);

  // read the value of the digital pin
  int button_state = button->read();

  // write the value to the console for debugging
  printf("%d \n", button_state);

  return MRAA_SUCCESS;
}
```

To react to a button press beyond application startup, add a `while` or `for` loop with a delay to periodically poll the pin state. For example, this loop reads the button and waits for 500ms before checking the button state again:

```
// poll for changes in input state
for (;;) {
  int button_state = button->read();
  printf("%d \n", button_state);
  usleep(500*1000);
}
```

To implement a non-blocking way of detecting changes in input values, use [`mraa_gpio_isr()` as an interrupt handler](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities#_Toc4.2) instead of a loop.

**Higher level UPM example:**

```
#include "grove.h"
#include <stdio.h>

int main()
{
  // use GroveButton class to set up GPIO digital pin #5
  // (internally sets direction to input)
  upm::GroveButton* button = new upm::GroveButton(5);

  // poll for changes in input state
  for(;;) {
    // read the value of the digital pin
    int button_state = button->value();

    // write the value to the console for debugging
    printf("%d \n", button_state);
    
    // 500ms delay
    usleep(500 * 1000);
  }

  // Delete the button object
  delete button;

  return MRAA_SUCCESS;
}
```

### Analog inputs

<div class="tldr" markdown="1">
An analog input will read a value as between `0` and `1024`.

Connect to any pin labeled "A" (for "analog") on the Grove Base Shield such as A0 to A3.
</div>

**Example components:**

* Grove Light Sensor
* Grove Rotary Angle
* Grove Temperature
* Grove Sound Sensor

**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

```

```

To implement a non-blocking way of detecting changes in input values, use [`mraa_gpio_isr()` as an interrupt handler](https://software.intel.com/en-us/articles/internet-of-things-using-mraa-to-abstract-platform-io-capabilities#_Toc4.2) instead of a loop.

### Analog outputs

<div class="tldr" markdown="1">
An analog output is a digital output in disguise. Intel® IoT boards are digital microcontrollers that can pretend to be analog using a concept called Pulse Width Modulation (PWM). 

Analog outputs will accept a floating-point value representing a duty cycle percentage between `0` (always off), `1.0` (always on). For example, a value of `0.5` will rapidly pulse equally between on and off.

Components will only work when connected to PWM-enabled pins! By factory default, these PWM pins are D3, D5, and D6. (Digital pin #9 is also available on the Arduino expansion board via the standard female header pin.)
</div>

**Example components:**

* Grove LED Socket Kit
* Grove Buzzer
* Grove Servo Motor (ES08A)

**Low level MRAA-only example:**

```

```

**Higher level UPM example:**

Please see: [https://github.com/intel-iot-devkit/upm/blob/master/examples/c++/es08a.js](https://github.com/intel-iot-devkit/upm/blob/master/examples/c++/es08a.js)


### I2C

<div class="tldr" markdown="1">
I²C (Inter-Integrated Circuit), pronounced both "I-two-C" or "I-squared-C", is a multi-master, multi-slave, single-ended, serial computer bus used for attaching lower-speed peripherals to processors on computer motherboards and embedded systems.
</div>

**Example components:**

* Grove LCD RGB Backlight (JHD1313M1)

**Higher level UPM example:**

```

```

<div id="next-steps" class="note" markdown="1">
### Next Steps

You're done! Now make your own creation. 

Return back to [START HERE »](/docs/index.html#now-make-your-own-creation)
</div>
