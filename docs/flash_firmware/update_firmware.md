---
layout: default
title: Getting Started
---

# Flash the Edison

To start this process, do not have the Edison board plugged in on USB or powered on with a power supply.

![Edison Board Configuration](images/edison_board_config.jpg)

1. Get the latest Yocto firmware image for the Intel® Edison.

    <div class="callout goto" markdown="1">
    1. On the USB key: **downloads → Firmware - Edison Yocto**
    2. Copy **edison-image-[version].zip** to your computer.
    </div>

2. Launch Flash Tool Lite, click browse and select **edison-image-[version].zip** file.
 
   ![Browse Edison Image](images/browse_flash_tool.jpg)

3. The tool extracts the zip file and loads FlashEdison.json.
 
   ![Load FlashEdison.json](images/json_flash_tool.jpg)

4. On the Configuration drop down, **choose CDC if your host machine is OS X or Linux**, **choose RNDIS for Windows**.

5. Click Start to Flash (the Edison board is not plugged in yet).
 
   ![Start to Flash](images/start_flash_tool.jpg)

6. Plug the USB cable into the Multigadget port of the Edison board. You should see the Flash Tool detect the board and begin the flash process.

   ![Plug the USB cable](images/plug_usb_flash_tool.jpg)


   **Firmware flash progress**

   ![Flash progress](images/progress_flash_tool.png)
   
7. Once the flashing is completed, the board restarts do not unplug the board for atleast 2-3 minutes.

<div id="next-steps" class="note" markdown="1">
### Next Steps

You'll need to now gain command line access of your IoT board, in order to set up an internet connection. You'll also be executing special Linux commands to configure your IoT board such as setting up Wi-Fi.

Please pick your operating system from the options below to proceed.

* [Windows »](../shell_access/windows/serial_connection.html)
* [Mac »](../shell_access/mac/serial_connection.html)
* [Linux »](../shell_access/linux/serial_connection.html)
</div>
