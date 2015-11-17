---
layout: default
title: Connecting cables
parentUrl: index.html
parentTitle: Unboxing and Assembly
---

<div id="toc" markdown="1">
* [Device mode vs host mode »](#device-mode-vs-host-mode)
* [Device mode micro-USB cable »](#device-mode-micro-usb-cable)
* [UART/serial micro-USB cable »](#uartserial-micro-usb-cable)
* [DC power supply »](#dc-power-supply)
* [Host mode USB cable »](#host-mode-usb-cable)
</div>

# Connecting cables

Explore when and how to use all the cables ports on the Intel® Edison kit for Arduino. 

## Device mode vs host mode

The hardware slider on the Arduino expansion board switches between USB _host mode_ and USB _device mode_. 

**Device mode:** The switch is toggled down and a micro-USB cable can be used to turn the Intel® Edison into a computer peripheral. Device mode allows you to do such things as: program the board over USB, or mount the onboard flash memory like a disk drive. Refer to [Device mode micro-USB cable »](#device-mode-micro-usb-cable)

![Microswitch toggled down for device mode](images/microswitch-device_mode-zoom_in.png)

**Host mode:** The switch is toggled up and USB peripherals with a standard-sized USB cable (such as mice, keyboards, etc) can be plugged into the Intel® Edison. USB host mode requires the use of an external power adapter. Refer to [Host mode USB cable  »](#host-mode-usb-cable)

![Microswitch toggled up for host mode](images/microswitch-host_mode-zoom_in.png)


## Device mode micro-USB cable

<div class="tldr" markdown="1">
Use the top micro-USB port in USB device mode for:

* 5V power, 
* programming the Intel® Edison using the Arduino IDE, 
* programming the Intel® Edison using the Intel® XDK or Eclipse IDE included in the Intel® IoT Developer Kit via Ethernet over USB (not Wi-Fi), and
* writing to the onboard flash memory from your computer.
</div>

[![Animated gif: using device mode](){: .animated data-still="images/device_mode-sampleframe.jpg" data-animated="images/device_mode-animated.gif"}](details-device_mode_cable.html)

[View detailed instructions for the device mode cable »](details-device_mode_cable.html){: .link-button .centered}


## UART/serial micro-USB cable

<div class="tldr" markdown="1">
Use the bottom micro-USB port to send serial commands to your Intel® Edison via Terminal or PuTTY. Use these commands to flash firmware, configure Wi-Fi, or identify the board's IP address. 
</div>

[![Animated gif: using UART/serial cable](){: .animated data-still="images/serial-sampleframe.jpg" data-animated="images/serial-animated.gif"}](details-serial_cable.html)

[View detailed instructions for the serial cable »](details-serial_cable.html){: .link-button .centered}


## DC power supply

<div class="tldr" markdown="1">
The Arduino expansion board for Intel® Edison can be powered via the DC power jack, the device mode micro-USB port, or both. If you are going to use more power intensive features such as Wi-Fi, a servo motor, or an Arduino shield, use a DC power supply in addition to the device mode micro-USB cable. 
</div>

[![Animated gif: using power barrel connector](){: .animated data-still="images/power_barrel-firstframe.jpg" data-animated="images/power_barrel-animated.gif"}](details-power_barrel.html)

[View detailed instructions for the power supply cable»](details-power_barrel.html){: .link-button .centered}


## Host mode USB cable

<div class="tldr" markdown="1">
Use the standard-sized USB port in USB host mode to allow the Intel® Edison to accept USB peripherals such as mice, keyboards, etc. 
</div>

[![Animated gif: using host mode](){: .animated data-still="images/host_mode-sampleframe.jpg" data-animated="images/host_mode-animated.gif"}](details-host_mode_cable.html)

[View detailed instructions for the host mode cable »](details-host_mode_cable.html){: .link-button .centered}

