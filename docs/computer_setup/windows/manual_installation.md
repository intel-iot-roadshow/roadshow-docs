---
layout: default
title: Getting Started
---

# Set Up Your Computer - Windows (manual installation)

This setup document will guide you through manually preparing your Windows 32-bit or 64-bit computer with any Windows-specific software or drivers required for Intel® Edison development. 

<div id="toc" class="box" markdown="1">
* [Install Intel® Edison standalone drivers »](#install-intel-edison-standalone-drivers)
* [Install FTDI serial drivers »](#install-ftdi-serial-drivers)
* [Restart your computer »](#restart-your-computer)
</div>

<!-- <div class="related-videos" class="callout video">
  <iframe src="https://drive.google.com/file/d/0B6gHgawzKtxCbUxicmpBc2JZSmM/preview" width="565" height="367"></iframe>
</div> -->


## Install Intel® Edison standalone drivers

<div class="tldr" markdown="1">
The Windows standalone drivers for Intel® Edison include several USB drivers in one installer package. These drivers enable important features, such as:

* Composite Device Class (CDC) for programming the board via the Arduino IDE,
* Remote Network Driver Interface Spec (RNDIS) for Ethernet over USB, and
* Device Firmware Upgrade (DFU) for updating firmware on devices.

[View detailed instructions »](details-install_edison_drivers.html)
</div>

[![Animated gif: installing Intel® Edison drivers](images/install_edison_drivers-animated.gif)](details-install_edison_drivers.html)


## Install FTDI serial drivers

<div class="tldr" markdown="1">
FTDI CDM drivers allow your computer to communicate with USB serial devices, including the Intel® Edison. 

[View detailed instructions »](details-install_ftdi_cdm_drivers.html)
</div>

[![Animated gif: installing Intel® Edison drivers](images/install_ftdi_cdm_drivers-animated.gif)](details-install_ftdi_cdm_drivers.html)


## Restart your computer

<div class="tldr" markdown="1">
To ensure driver installation changes take effect, reboot your Windows computer at this point.
</div>

![Choose Restart from the Windows Start menu](images/restart_windows.png)


<div id="next-steps" class="note" markdown="1">
### Next Steps

[Confirm driver installation »](confirm_drivers.html)
</div>
