---
layout: default
title: Getting Started
---

# Confirm driver installation - Windows 


<div class="toc" markdown="1">
**Table of contents**

* [Open Windows Device Manager »](#open-windows-device-manager)
* [Confirm installation of Intel® Edison Drivers »](#confirm-installation-of-intel-edison-drivers)
* [Confirm installation of FTDI serial drivers »](#confirm-installation-of-ftdi-serial-drivers)
</div>

<div class="related-videos" markdown="1">
**Related video**

* [Intel Edison: Set Up Your Computer Manually - Windows (preview video)](https://drive.google.com/open?id=0B6gHgawzKtxCbUxicmpBc2JZSmM&authuser=0)
* [Intel Edison: Set Up Your Computer - Windows Integrated Installer (preview video)](https://drive.google.com/open?id=0B6gHgawzKtxCejNuYjc3a216X3M&authuser=0)
</div>

## Open Windows Device Manager

Launch the Device Manager utility on Windows in order to debug your Intel® IoT board USB connections. [View detailed instructions »](details-open_device_manager.html)

![Animated gif: opening Windows Device Manager using the Start menu](images/open_device_manager-animated.gif)


## Confirm installation of Intel® Edison Drivers

Look for both "Intel Edison USB Composite Device" and "Intel Edison Virtual Com Port" items in Device Manager under “Ports (COM & LPT)” after plugging in the device mode USB cable. [View detailed instructions »](details-confirm_edison_drivers.html)

![Animated gif: confirming the installation of Intel Edison drivers](images/confirm_edison_drivers-animated.gif)


## Confirm installation of FTDI serial drivers

Look for "USB Serial Port" in Device Manager under “Ports (COM & LPT)” after plugging in the UART/serial USB cable. [View detailed instructions »](details-confirm_ftdi_cdm_drivers.html)

![Animated gif: confirming the installation of FTDI CDM drivers](images/confirm_ftdi_cdm_drivers-animated.gif)


---

### Next Steps

Gain command line access of your IoT board. Execute special Linux commands to configure your IoT board such as setting up Wi-Fi. 

[Shell Access - Windows »](/docs/shell_access/windows/serial_connection.html)