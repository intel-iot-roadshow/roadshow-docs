---
layout: default
title: Installation - Windows
parentUrl: index.html#install-arduino-ide
parentTitle: Arduino IDE
---

1. Get the latest Arduino IDE.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Windows</span> → <span class="icon folder">edison_media</span>
    2. Copy <span class="icon file">arduino-[version]-windows.exe</span> to your computer.
    </div>

2. Double-click <span class="icon file">arduino-[version]-windows.exe</span> to start the installation wizard.

3. Click **I Agree** when prompted by the installer.

4. Click **Next** and then **Install** to install the Arduino IDE.  When prompted to install device software, select **Install**.

5. Once the Arduino IDE is installed, you should see an Arduino shortcut on your desktop. Double-click on it to open the Arduino IDE.

6. To save on internet bandwidth, install the "Intel i686 Boards" toolchain manually to your Arduino IDE installation.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Windows</span> → <span class="icon folder">edison_media</span>
    2. Copy <span class="icon file">IntelArduinoToolchain.7z</span> to your computer and unzip it using **7zip**.
    3. Copy the uncompressed <span class="icon folder">Intel</span> folder and its contents to <span class="icon folder">C:\Users\\[YOUR_USER_NAME]\AppData\Roaming\Arduino15\packages\Intel</span> on your computer.
    </div>

7. Restart the Arduino IDE.

<div class="callout info" markdown="1">
When you are using a more reliable internet connection, you can use the method below to update the Arduino boards list:

1. Choose **Tools** > **Board** > **Boards Manager** to open the Boards Manager.
  
    ![Boards Manager - Windows](images/BoardMan-Win.png)

2. In the list of boards, select **Intel i686 Boards** which includes the Intel® Edison board.

3. Click **Install**.

4. When the installation process is finished, click **OK**.
</div>
