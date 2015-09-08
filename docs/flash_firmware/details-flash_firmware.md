---
layout: default
title: Flash Intel® Edison firmware
parentUrl: index.html#flash-intel-edison-firmware
parentTitle: Flash Firmware using Flash Tool Lite
---

1. Unplug any USB or power cables connected to the Intel® Edison.

2. Get the latest Yocto firmware image for the Intel® Edison.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Firmware</span>
    2. Copy <span class="icon file">edison-image-[version].zip</span> to your computer.
    </div>

3. Launch the **Flash Tool Lite** program installed in the previous section.

4. Click **Browse** in the upper righthand corner. Select <span class="icon file">edison-image-[version].zip</span> file.
 
    ![Browse Edison Image](images/browse_flash_tool.jpg)

    The tool extracts the zip file and loads FlashEdison.json.
 
    ![Load FlashEdison.json](images/json_flash_tool.jpg)

5. For the "**Configuration**" drop down, if your host machine is:
    
    * **OS X or Linux:** choose "CDC" 
    * **Windows:** choose "RNDIS"

6. Unplug all cables from the Intel® Edison. 

7. Click **Start to Flash**.
 
    ![Start to Flash](images/start_flash_tool.jpg)

8. When you see the prompt, plug a micro-USB cable into the **_top_** micro-USB connector on the expansion board.

    ![Micro-USB cable being plugged into the top micro-USB connector](../assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)

    You should see the Flash Tool detect the board and begin the flash process.

    ![Plug the USB cable](images/plug_usb_flash_tool.jpg)

9. Wait 3-4 minutes for the firmware progress to finish. Do **not** unplug the board during this time!

    ![Firmware flash progress](images/progress_flash_tool.png)
   
<div class="callout done" markdown="1">
Once the flashing is completed, the board will restart and you will see a "Flash success" indicated in the Flash Tool.
</div>
