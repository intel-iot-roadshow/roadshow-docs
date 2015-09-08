---
layout: default
title: Set Up Your Computer - Mac
---

# Set Up Your Computer - Mac

_Instructions for the **Xadow Wearables Kit for Intel® Edison** on **Mac**_

This setup document will guide you through preparing your computer with Mac-specific drivers required for the Xadow Wearables Kit for Intel® Edison.

---

**Are you using the Intel® Edison Kit for Arduino expansion board?**

You do not need to go through this step. This document is for installing serial drivers for the Xadow programmer board. Continue to [Shell Access - Mac](../../shell_access/mac/index.html).

---

<div class="toc" markdown="1">
**Table of contents**

* [Download and install FTDI VCP serial drivers](#download-and-install-ftdi-vcp-serial-drivers)
</div>

# Download and install FTDI VCP serial drivers

FTDI Virtual COM port (VCP) drivers allow your Mac to communicate with the Intel® Edison over USB serial when the Intel® Edison is attached to the Xadow expansion board and programmer.

1. Get the latest FTDI VCP driver installer.

    <div class="callout goto" markdown="1">
    1. On the USB key: **downloads → Mac**
    2. Copy *FTDIUSBSerialDriver_version.dmg* to your computer.
    </div>

2. Click on **FTDIUSBSerialDriver_version.dmg** to extract the installer package.

3. In the new Finder window, click on **FTDIUSBSerial.pkg** to start the installer.

4. Follow the installation wizard prompts. Click "**Next**" where needed.

  ![FTDI USB Serial Driver installation wizard](images/ftdi_drivers-installer_wizard.png)

5. Click "**Finish**" to close the installation wizard.

6. Restart your Mac for driver changes to take effect. **You must restart your computer for driver changes to take effect!**

---

### What to do next

Gain command line access of your IoT board. Execute special Linux commands to configure your IoT board such as setting up Wi-Fi. 

[Shell Access - Mac »](../../shell_access/mac/index.html)