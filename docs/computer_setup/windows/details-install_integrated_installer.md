---
layout: default
title: Getting Started
---

## Download and run the Intel® Edison integrated installer

The Windows 64-bit Integrated Installer gives you options to automatically install:

* Intel® Edison and FTDI serial drivers on your Windows computer,
* an IDE of your choice (Arduino, Intel XDK® for IoT, and/or Eclipse), and
* the latest firmware image on your Intel® Edison.

![Animated gif: installing Intel® Edison drivers using integrated installer](images/install_integrated_installer-animated.gif)

---

1. Get the latest Intel® Edison 64-bit Windows installer.

    <div class="callout goto" markdown="1">
    1. On the USB key: **downloads → Windows**
    2. Copy **iotdk_win_installer.exe** to your computer.
    </div>

2. Connect a micro-USB cable to the **device mode** micro-USB port of the Intel® Edison expansion board, and the other end to your computer.

    ![Micro-USB cable being plugged into the top micro-USB connector](/docs/assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)
  
    Refer to [Device mode micro-USB cable](/docs/assembly/arduino_expansion_board/details-device_mode_cable.html) for more detailed cable connection information.

3. Double-click on the **iotdk_win_installer.exe** on your computer to begin installation. 
  
    ![Intel® Edison 64-bit integrated installer wizard](images/integrated_installer_wizard.png)

4. Follow the installation wizard. Click "**Next**" where needed. 

5. When done, click "**Finish**" to close the installation wizard. 
  
    If there are any errors during installation, you will need to resolve them manually.

<div class="callout troubleshooting" markdown="1">
**Is the "Next" button greyed out?**

The integrated installer is unable to detect your Intel® Edison. Ensure that the board is powered on and plugged into your computer via the device mode micro-USB port on the expansion board.

Otherwise you will need to install the Windows drivers manually. Go to [Set Up Your Computer - Windows (manual installation) »](manual_installation.html) 
</div>

---

The default settings can be adjusted to your needs, or leave the defaults as is. 

![Configure Intel® Edison 64-bit integrated installion](images/integrated_installer_wizard-config_screen.png)

In the component selection screen, check the options you would like to install:

  * **Drivers:** 
    Installs the Intel® Edison drivers and FTDI serial drivers for Windows.

  * **Update image:** 
    Flashes the latest firmware image directly on your Intel® Edison.
    
    (Note: You will not be able to use this option until after you have installed the drivers. Re-run the integrated installer if you wish to use it to flash Intel® Edison firmware.)

  * **Development Environment:** Choose from 
      * **Arduino Software** (simplified C++), 
      * **Intel® XDK IoT Edition** (JavaScript), and/or 
      * **Eclipse** (C/C++).
