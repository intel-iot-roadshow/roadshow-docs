---
layout: default
title: Getting Started
---

## Step 1: Install Intel® XDK IoT Edition

Get the latest [Intel® XDK IoT Edition installer](http://software.intel.com/en-us/html5/xdk-iot) for your computer's OS. Simply run the installer and follow the prompts. 

![Animated gif: installing the Intel® XDK](images/install_xdk-animated.gif)

---

**Using a 64-bit Windows computer?**

Intel® XDK IoT Edition can be installed via the Windows 64-bit integrated installer. Refer to [Set Up Your Computer - Windows (64-bit integrated installer)](/docs/computer_setup/windows/64bit_integrated_installer.html) for more info.

---

1. Get the latest Intel® XDK IoT Edition installer.

  **Hackathon attendees:**
  
  1. On the USB key: files → [your OS]
  2. Copy the appropriate **iot_web** installer file to your computer: 
    * **Windows**: iot_web_win_master_[version].exe
    * **Mac**: iot_web_mac_master_[version].dmg
    * **Linux 32-bit**: iot_web_linux32_master_[version].tgz
    * **Linux 64-bit**: iot_web_linux64_master_[version].tgz

  **Online option:**

  1. Visit [software.intel.com/en-us/html5/xdk-iot](http://software.intel.com/en-us/html5/xdk-iot). 
  2. Ensure that your OS platform is selected in the green download box, then click "Go!" to start downloading the installer.

### On Windows

2. Double-click on **iot_web_win_master_[version].exe** to start the installer. 

### On Mac

2. Double-click on **iot_web_mac_master_[version].dmg** to open the Apple Disk Image.

3. Double-click on the extracted **xdk_full_[version].pkg** to start the installer.

### On Linux

2. Open Terminal.

3. Use the `cd` command to go into the folder where the installer file is. For example:

  ```
  cd ~/Desktop/
  ```

4. Use the `tar` command to extract the .tgz. For example:

  ```
  tar zxvf iot_web_linux64_master_1912.tgz
  ```

  (Note: Replace the filename shown below with your .tgz filename.)

5. Go into the extracted folder, then run the installer shell file. For example:

  ```
  cd iot_web_linux64
  ./install.sh
  ```

### All platforms

After launching the Intel® XDK installer, follow the installation wizard and click "Next" where needed.

![First screen of the Intel® XDK installer](images/xdk_installer.jpg)
