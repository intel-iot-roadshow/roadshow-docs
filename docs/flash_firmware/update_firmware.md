---
layout: default
title: Getting Started
---

# Flash the Edison

1. Unplug any USB or power cables connected to the Intel® Edison.

2. Get the latest Yocto firmware image for the Intel® Edison.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Firmware</span> - <span class="icon folder">Edison Yocto</span>
    2. Copy <span class="icon file">edison-image-[version].zip</span> to your computer.
    </div>

3. Launch the **Flash Tool Lite** installed in the previous step.

4. Click browse and select <span class="icon file">edison-image-[version].zip</span> file.
 
    ![Browse Edison Image](images/browse_flash_tool.jpg)

    The tool extracts the zip file and loads FlashEdison.json.
 
    ![Load FlashEdison.json](images/json_flash_tool.jpg)

5. For the "Configuration" drop down, if your host machine is:
    
    * **OS X or Linux:** choose "CDC" 
    * **Windows:** choose "RNDIS".

6. Click **Start to Flash** (the Edison board is not plugged in yet).
 
    ![Start to Flash](images/start_flash_tool.jpg)

6. Plug a micro-USB cable into the **_top_** micro-USB connector on the expansion board.

    ![Micro-USB cable being plugged into the top micro-USB connector](../assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)

    You should see the Flash Tool detect the board and begin the flash process.

    ![Plug the USB cable](images/plug_usb_flash_tool.jpg)

    **Firmware flash progress**

    ![Flash progress](images/progress_flash_tool.png)
   
7. Once the flashing is completed, the board restarts. Do not unplug the board for at least 2-3 minutes.

<div id="next-steps" class="note" markdown="1">
### Next Steps

Gain command line access of your IoT board. Execute special Linux commands to configure your IoT board such as setting up Wi-Fi.

Please pick your operating system from the options below to proceed.

* [Windows »](../shell_access/windows/serial_connection.html)
* [Mac »](../shell_access/mac/serial_connection.html)
* [Linux »](../shell_access/linux/serial_connection.html)
</div>
