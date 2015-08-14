---
layout: default
title: Getting Started
---

<div id="toc" markdown="1">
* [Step 1: Prepare built-in flash storage »](#step-1-prepare-built-in-flash-storage)
* [Step 2: Copy over the latest image »](#step-2-copy-over-the-latest-image)
* [Step 3: Flash the image »](#step-3-flash-the-image)
</div>

# Flash Firmware Manually

The firmware on your Intel® Edison is the board's operating system. Intel® IoT firmware engineers are constantly improving the performance of the Intel® Edison and enabling new features. When you receive a brand new Intel® Edison, update the firmware on the board to get the best developer experience.

This document will guide you through the manual process required to flash the firmware on the Intel® Edison using any OS platform.

<div class="callout info" markdown="1">
**Want to know if your current firmware is old before flashing?**

Refer to [Check installed firmware version »](check_firmware_version.html).
</div>

<!-- <div id="related-videos" class="callout video">
[How to Flash Firmware Manually on the Intel® Edison (preview)](https://drive.google.com/open?id=0B2ywC78pxngCWkNUT3dkWklBdDg&authuser=0)
</div> -->

## Step 1: Prepare built-in flash storage

<div class="tldr" markdown="1">
Make sure there are no files on the built-in flash storage of the Intel® Edison by formatting the storage. The storage **must** be formatted as FAT32.
</div>

![Animated gif: formatting the Edison flash storage](images/format_storage-windows-animated.gif)

<div class="link-button-container" markdown="1">
<span class="link-button-container-title">View detailed instructions for:</span>
[Windows »](details-format_storage-windows.html){: .link-button}
[Mac »](details-format_storage-mac.html){: .link-button}
[Linux »](details-format_storage-linux.html){: .link-button}
</div>


## Step 2: Copy over the latest image

<div class="tldr" markdown="1">
Extract the contents of the [Yocto complete image](http://software.intel.com/iot/hardware/edison/downloads) zip, then copy the contents to your Intel® Edison drive. 
</div>

[![Animated gif: copying images files to flash storage](images/copy_image_files-animated.gif)](details-copy_image_files.html)

[View detailed instructions »](details-copy_image_files.html){: .link-button .centered}


## Step 3: Flash the image

<div class="tldr" markdown="1">
Run the `reboot ota` command on the Intel® Edison to flash the board with the files you copied over in Step 2. 
</div>

[![Animated gif: flashing the Intel® Edison](images/reboot_ota-animated.gif)](details-reboot_ota.html)

[View detailed instructions »](details-reboot_ota.html){: .link-button .centered}


<div id="next-steps" class="note" markdown="1">
### Next Steps

Get your board online in order to turn your IoT board into a true "Internet of Things" device. You also need the IP address of your IoT board to program it using the dev kit IDEs.

**At a hackathon? On a busy or restricted Wi-Fi network?**

Connect to the Intel® Edison using the device mode micro-USB cable and a virtual Ethernet connection known as "Ethernet over USB":

* [Windows »](../../connectivity/ethernet_over_usb/windows/connect.html)
* [Linux »](../../connectivity/ethernet_over_usb/linux/connect.html)
* Note: At this time, Ethernet over USB on Mac is not officially supported.

**At home? Have a dependable Wi-Fi connection?**

* [Get Your Edison Board Online »](../../connectivity/wifi/connect.html)
</div>