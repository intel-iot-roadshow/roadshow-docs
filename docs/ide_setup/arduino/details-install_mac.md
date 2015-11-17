---
layout: default
title: Installation - Mac
parentUrl: index.html#install-arduino-ide
parentTitle: Arduino IDE
---

1. Get the latest Arduino IDE.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Mac</span>
    2. Copy <span class="icon file">arduino-[version]-macosx.zip</span> to your computer.
    </div>

2. Double-click <span class="icon file">arduino-[version]-macosx.zip</span> to extract the archive. 
  
    ![Extracting Arduino IDE](images/macOSXExtract.png)

3. Rename <span class="icon file">Arduino</span> to be <span class="icon file">ArduinoEdison</span>.

4. Move <span class="icon file">ArduinoEdison</span> into your Mac <span class="icon folder">Applications</span> folder. 
  
    ![Macintosh Arduino IDE](images/MacApp.png)

4. Double-click on <span class="icon file">ArduinoEdison</span> to open the Arduino IDE.

6. To save on internet bandwidth, install the "Intel i686 Boards" toolchain manually to your Arduino IDE installation.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Mac</span> → <span class="icon folder">edison_media</span>
    2. Copy <span class="icon file">IntelArduinoToolChain_mac.zip</span> to your computer and unzip it.
    3. Copy the uncompressed <span class="icon folder">Intel</span> folder and its contents to <span class="icon folder">/Users/[YOUR_USER_NAME]/Library/Arduino15/packages</span> on your computer.
    </div>

7. Restart the Arduino IDE.

<div class="callout info" markdown="1">
When you are using a more reliable internet connection, you can use the method below to update the Arduino boards list:

1. Choose **Tools** > **Board** > **Boards Manager** to open the Boards Manager.
  
    ![Boards Manager - Windows](images/boardman-mac.png)

2. In the list of boards, select **Intel i686 Boards** which includes the Intel® Edison board.

3. Click **Install**.

4. When the installation process is finished, click **OK**.
</div>
