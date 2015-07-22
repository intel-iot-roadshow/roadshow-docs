---
layout: default
title: Getting Started
---

# Connecting cables

Explore when and how to use all the cables ports on the Intel® Edison kit for Arduino. 

<div id="toc" class="box" markdown="1">
* [Device mode vs host mode »](#device-mode-vs-host-mode)
* [Device mode micro-USB cable »](#device-mode-micro-usb-cable)
* [UART/serial micro-USB cable »](#uartserial-micro-usb-cable)
* [DC power supply »](#dc-power-supply)
* [Host mode USB cable »](#host-mode-usb-cable)
</div>

<!-- <div id="related-videos" class="callout video">
  <object id="flashObj" width="565" height="367" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,47,0"><param name="movie" value="http://c.brightcove.com/services/viewer/federated_f9?isVid=1" /><param name="bgcolor" value="#FFFFFF" /><param name="flashVars" value="videoId=4117768692001&playerID=741496470001&playerKey=AQ~~,AAAArH1stHk~,LuRqJUw7MaeYQkat5frTpWWPINh71g7p&domain=embed&dynamicStreaming=true" /><param name="base" value="http://admin.brightcove.com" /><param name="seamlesstabbing" value="false" /><param name="allowFullScreen" value="true" /><param name="swLiveConnect" value="true" /><param name="allowScriptAccess" value="always" /><embed src="http://c.brightcove.com/services/viewer/federated_f9?isVid=1" bgcolor="#FFFFFF" flashVars="videoId=4117768692001&playerID=741496470001&playerKey=AQ~~,AAAArH1stHk~,LuRqJUw7MaeYQkat5frTpWWPINh71g7p&domain=embed&dynamicStreaming=true" base="http://admin.brightcove.com" name="flashObj" width="565" height="367" seamlesstabbing="false" type="application/x-shockwave-flash" allowFullScreen="true" swLiveConnect="true" allowScriptAccess="always" pluginspage="http://www.macromedia.com/shockwave/download/index.cgi?P1_Prod_Version=ShockwaveFlash"></embed></object>
</div> -->

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

[View detailed instructions »](details-device_mode_cable.html)
</div>

[![Animated gif: using device mode](images/device_mode-animated.gif)](details-device_mode_cable.html)


## UART/serial micro-USB cable

<div class="tldr" markdown="1">
Use the bottom micro-USB port to send serial commands to your Intel® Edison via Terminal or PuTTY. Use these commands to flash firmware, configure Wi-Fi, or identify the board's IP address. 

[View detailed instructions »](details-serial_cable.html)
</div>

[![Animated gif: using UART/serial cable](images/serial-animated.gif)](details-serial_cable.html)


## DC power supply

<div class="tldr" markdown="1">
The Arduino expansion board for Intel® Edison can be powered via the DC power jack, the device mode micro-USB port, or both. If you are going to use more power intensive features such as Wi-Fi, a servo motor, or an Arduino shield, use a DC power supply in addition to the device mode micro-USB cable. 

[View detailed instructions »](details-power_barrel.html)
</div>

[![Animated gif: using power barrel connector](images/power_barrel-animated.gif)](details-power_barrel.html)


## Host mode USB cable

<div class="tldr" markdown="1">
Use the standard-sized USB port in USB host mode to allow the Intel® Edison to accept USB peripherals such as mice, keyboards, etc. 

[View detailed instructions »](details-host_mode_cable.html)
</div>

[![Animated gif: using host mode](images/host_mode-animated.gif)](details-host_mode_cable.html)


<div id="next-steps" class="note" markdown="1">
### Next Steps

Install software and drivers specifically for your computer's operating system. 

* **Mac or Linux user?** Install the Flashing Tool:

  * [Mac »](/docs/flash_firmware/mac_install.html)
  * [Linux »](/docs/flash_firmware/linux_install.html)

* **Windows user?**

  [Set Up Your Computer - Windows (manual installation) »](/docs/computer_setup/windows/manual_installation.html)
</div>