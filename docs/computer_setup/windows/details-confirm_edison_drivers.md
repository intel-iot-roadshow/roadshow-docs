---
layout: default
title: Confirm installation of Intel® Edison Drivers
parentUrl: index-confirm_drivers.html#confirm-installation-of-intel-edison-drivers
parentTitle: Confirm driver installation
parentParentUrl: index.html
parentParentTitle: Set Up Your Computer - Windows
---

1. Connect a micro-USB cable to the [device mode](../../assembly/arduino_expansion_board/details-device_mode_cable.html) micro-USB port of the Intel® Edison expansion board, and the other end to your computer.
  
    ![Micro-USB cable being plugged into the top micro-USB connector](../../assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)
  
<div class="callout done" markdown="1">
If you see both "**Intel Edison USB Composite Device**" and "**Intel Edison Virtual Com Port**" items show up in Device Manager under "Ports (COM & LPT)", the drivers have been successfully installed. 

![Two "Intel Edison" entries in Device Manager](images/device_manager-intel_edison.png)
</div>


<div class="callout troubleshooting" markdown="1">
**Do not see Intel® Edison devices show up in Device Manager?**

* Check that the Intel® Edison is in [device mode](../../assembly/arduino_expansion_board/index-connecting_cables.html#device-mode-vs-host-mode).
* Check that the micro-USB cable is securely connected to the [device mode micro-USB port](../../assembly/arduino_expansion_board/index-connecting_cables.html#device-mode-micro-usb-cable) of the Intel® Edison expansion board.
* Restart your computer to ensure driver changes to take effect.
* Try a different micro-USB cable to eliminate errors due to a bad cable.
* Update the firmware on the Intel® Edison. Refer to [Flash Edison Firmware Manually](../../flash_firmware/manually/index.html).
</div>