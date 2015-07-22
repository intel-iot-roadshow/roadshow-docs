---
layout: default
title: Getting Started
---

# Confirm driver installation - Windows 

<div id="toc" class="box" markdown="1">
* [Open Windows Device Manager »](#open-windows-device-manager)
* [Confirm installation of Intel® Edison Drivers »](#confirm-installation-of-intel-edison-drivers)
* [Confirm installation of FTDI serial drivers »](#confirm-installation-of-ftdi-serial-drivers)
</div>

<!-- <div class="related-videos" class="callout video">
* [Intel Edison: Set Up Your Computer Manually - Windows (preview video)](https://drive.google.com/open?id=0B6gHgawzKtxCbUxicmpBc2JZSmM&authuser=0)
* [Intel Edison: Set Up Your Computer - Windows Integrated Installer (preview video)](https://drive.google.com/open?id=0B6gHgawzKtxCejNuYjc3a216X3M&authuser=0)
</div> -->

## Open Windows Device Manager

<div class="tldr" markdown="1">
Launch the Device Manager utility on Windows in order to debug your Intel® IoT board USB connections. 

[View detailed instructions »](details-open_device_manager.html)
</div>

[![Animated gif: opening Windows Device Manager using the Start menu](images/open_device_manager-animated.gif)](details-open_device_manager.html)


## Confirm installation of Intel® Edison Drivers

<div class="tldr" markdown="1">
Look for both "Intel Edison USB Composite Device" and "Intel Edison Virtual Com Port" items in Device Manager under “Ports (COM & LPT)” after plugging in the device mode USB cable. 

[View detailed instructions »](details-confirm_edison_drivers.html)
</div>

[![Animated gif: confirming the installation of Intel Edison drivers](images/confirm_edison_drivers-animated.gif)](details-confirm_edison_drivers.html)


## Confirm installation of FTDI serial drivers

<div class="tldr" markdown="1">
Look for "USB Serial Port" in Device Manager under “Ports (COM & LPT)” after plugging in the UART/serial USB cable. 

[View detailed instructions »](details-confirm_ftdi_cdm_drivers.html)
</div>

[![Animated gif: confirming the installation of FTDI CDM drivers](images/confirm_ftdi_cdm_drivers-animated.gif)](details-confirm_ftdi_cdm_drivers.html)


<div id="next-steps" class="note" markdown="1">
### Next Steps

Some Edison boards have older firmware images on them. You **_may_** need to update the firmware to a newer version to get access to important features.

* [Install Edison Flash Tool »](../../flash_firmware/windows_install.html)
</div>
