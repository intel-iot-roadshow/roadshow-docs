---
layout: default
title: Install FTDI serial drivers
---

<div class="callout info" markdown="1">
**Do you already have FTDI CDM drivers installed?**

If you have done Arduino development on your current computer before, you may already have the FTDI CDM drivers installed. Refer to [Confirm installation of FTDI serial drivers](confirm_drivers.html#confirm-installation-of-ftdi-serial-drivers){: .icon .bookmark} to see if you need to skip over this step.

However, if you see a "New Hardware Found" message when you plug in the Intel® Edison via the UART/serial micro-USB port and the automatic device driver installation fails, you will need to install the FTDI drivers. Ignore Windows' request to install the drivers for you and follow the steps below. 

![Windows message that a device driver software was not successfully installed](images/device_driver_software_not_installed.jpg)
</div>
 
1. Get the latest FTDI CDM driver installer.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Windows</span>
    2. Copy <span class="icon file">CDM [version] WHQL Certified.exe</span> to your computer.
    </div>

2. Right-click on <span class="icon file">CDM [version] WHQL Certified.exe</span>. Select **Run as administrator**.

    ![Select "Run as administrator" in file context menu](images/cdm_drivers-run_as_admin.png)

3. Click **Extract** to start the installation process. 
  
    ![FTDI CDM Drivers installer wizard](images/cdm_drivers-installer_wizard.png)

4. Follow the installation wizard prompts. Click **Next** where needed.

5. Click **Finish** to close the installation wizard.
