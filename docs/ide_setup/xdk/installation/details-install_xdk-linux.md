---
layout: default
title: Install Intel® XDK - Linux
parentUrl: index.html#install-intel-xdk-iot-edition
parentTitle: Intel® XDK IoT Edition - Standalone Installation
---

1. Get the latest Intel® XDK IoT Edition installer.

    <div class="callout goto" markdown="1">
    1.  On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Linux</span> → <span class="icon folder">edison_media</span>.
    2.  Copy the <span class="icon file">iot_web_[your OS]\_master\_[version]</span> installer file to your computer.
    </div>

2. Open <span class="icon linux">Terminal</span>.

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

6. After launching the Intel® XDK installer, follow the installation wizard and click **Next** where needed.

    ![First screen of the Intel® XDK installer](images/xdk_installer.jpg)
