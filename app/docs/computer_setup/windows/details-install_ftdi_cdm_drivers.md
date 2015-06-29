---
layout: default
title: Getting Started
---

## Install FTDI serial drivers

[FTDI CDM drivers](http://ftdichip.com/Drivers/D2XX.htm) allow your computer to communicate with USB serial devices, including the Intel® Edison.

![Animated gif: installing Intel® Edison drivers](images/install_ftdi_cdm_drivers-animated.gif)

---

**Do you already have FTDI CDM drivers installed?**

If you have done Arduino development on your current computer before, you may already have the FTDI CDM drivers installed. Refer to [Confirm installation of FTDI serial drivers](confirm_drivers.html#confirm-installation-of-ftdi-serial-drivers) to see if you need to skip over this step.

However, if you see a "New Hardware Found" message when you plug in the Intel® Edison via the UART/serial micro-USB port and the automatic device driver installation fails, you will need to install the FTDI drivers. Ignore Windows' request to install the drivers for you and follow the steps below. 

![Windows message that a device driver software was not successfully installed](images/device_driver_software_not_installed.jpg)
---
 
1. Get the latest FTDI CDM driver installer.
    
  * **Hackathon attendees:**
    1. On the USB key: files → Windows
    2. Copy **CDM [version] WHQL Certified.exe** to your computer.

  * **Online option:**
    1. Visit [ftdichip.com/Drivers/D2XX.htm](http://ftdichip.com/Drivers/D2XX.htm).
    2. Scroll down to the "**Currently Supported D2XX Drivers**" table. 
    3. In the row for "**Windows**", click the "**setup executable**" link to download **CDM [version] WHQL Certified.exe** to your computer.

2. Right-click on **CDM [version] WHQL Certified.exe**. Select "**Run as administrator**".

  ![Select "Run as administrator" in file context menu](images/cdm_drivers-run_as_admin.png)

3. Click "**Extract**" to start the installation process. 

  ![FTDI CDM Drivers installer wizard](images/cdm_drivers-installer_wizard.png)

4. Follow the installation wizard prompts. Click "**Next**" where needed.

5. Click "**Finish**" to close the installation wizard.
