---
layout: default
title: Install Intel® XDK IoT Edition
---

1. Get the latest Intel® XDK IoT Edition installer.

    <div class="callout goto" markdown="1">
    1.  On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">[your OS]</span>.
    2.  Copy the <span class="icon file">iot_web_[your OS]\_master\_[version]</span> installer file to your computer.
    </div>

### On Windows

2. Double-click on <span class="icon file">iot_web_win_master_[version].exe</span> to start the installer. 

### On Mac

2. Double-click on <span class="icon file">iot_web_mac_master_[version].dmg</span> to open the Apple Disk Image.

3. Double-click on the extracted <span class="icon file">xdk_full_[version].pkg</span> to start the installer.

### On Linux

2. Open Terminal.

3. Use the `cd` command to go into the folder where the installer file is. For example:

    ```
    cd ~/Desktop/
    ```

4. Use the `tar` command to extract the <span class="icon file">.tgz</span>. For example:

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

After launching the Intel® XDK installer, follow the installation wizard and click **Next** where needed.

![First screen of the Intel® XDK installer](images/xdk_installer.jpg)
