---
layout: default
title: Set Up Your Computer - Windows (manual installation)
---

<div id="toc" markdown="1">
* [Install Intel® Edison standalone drivers »](#install-intel-edison-standalone-drivers)
* [Install FTDI serial drivers »](#install-ftdi-serial-drivers)
* [Restart your computer »](#restart-your-computer)
</div>

# Set Up Your Computer - Windows (manual installation)

This setup document will guide you through manually preparing your Windows 32-bit or 64-bit computer with any Windows-specific software or drivers required for Intel® Edison development. 

<!-- <div class="related-videos" class="callout video">
  <iframe src="https://drive.google.com/file/d/0B6gHgawzKtxCbUxicmpBc2JZSmM/preview" width="565" height="367"></iframe>
</div> -->


## Install Intel® Edison standalone drivers

<div class="tldr" markdown="1">
The Windows standalone drivers (<span class="icon file">IntelEdisonDriverSetup[version].exe</span>) for Intel® Edison include several USB drivers in one installer package. These drivers enable important features, such as:

* Composite Device Class (CDC) for programming the board via the Arduino IDE,
* Remote Network Driver Interface Spec (RNDIS) for Ethernet over USB, and
* Device Firmware Upgrade (DFU) for updating firmware on devices.
</div>

[![Animated gif: installing Intel® Edison drivers](){: .animated data-still="images/install_edison_drivers-no_download-firstframe.jpg" data-animated="images/install_edison_drivers-no_download-animated.gif"}](details-install_edison_drivers.html)

[View detailed instructions »](details-install_edison_drivers.html){: .link-button .centered}


## Install FTDI serial drivers

<div class="tldr" markdown="1">
FTDI CDM drivers (<span class="icon file">CDM [version] WHQL Certified.exe</span>) allow your computer to communicate with USB serial devices, including the Intel® Edison. 
</div>

[![Animated gif: installing Intel® Edison drivers](){: .animated data-still="images/install_ftdi_cdm_drivers-no_download-firstframe.jpg" data-animated="images/install_ftdi_cdm_drivers-no_download-animated.gif"}](details-install_ftdi_cdm_drivers.html)

[View detailed instructions »](details-install_ftdi_cdm_drivers.html){: .link-button .centered}


## Restart your computer

<div class="tldr" markdown="1">
To ensure driver installation changes take effect, reboot your Windows computer at this point.
</div>

![Choose Restart from the Windows Start menu](images/restart_windows.png)


<div id="next-steps" class="note" markdown="1">
### Next Steps

[Confirm driver installation »](confirm_drivers.html)
</div>
