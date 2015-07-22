---
layout: default
title: Getting Started
---

## Step 2: Copy over the latest image

Extract the contents of the [Yocto complete image](http://software.intel.com/iot/hardware/edison/downloads) zip, then copy the contents to your Intel® Edison drive.

![Animated gif: copying images files to flash storage](images/copy_image_files-animated.gif)

---

1. Get the latest Yocto firmware image for the Intel® Edison.

    <div class="callout goto" markdown="1">
    1. On the USB key: **downloads → Firmware - Edison Yocto**
    2. Copy **edison-image-[version].zip** to your computer.
    </div>
      
    <div class="callout info" markdown="1">
    **Interested in finding out what's new with each firmware release?**
    
    Visit [Intel® Edison Boards and Compute Modules — Support Package Release Notes](http://www.intel.com/support/edison/sb/CS-035253.htm) to view the release notes PDF.
    </div>

2. Extract the contents of **edison-image-[version].zip** to your hard drive.

3. Copy the **entire** contents of the **edison-image-[version]** folder to the "**Edison**" drive that shows up after plugging the Intel® Edison to your computer. 

    Do **not** include the containing/parent edison-image-[version] folder; just the contents of the folder.

    ![Progress of copying files to Edison drive](images/windows-copying_files.jpg)

<div class="callout done" markdown="1">
Your "Edison" drive should now look similar to this:

![All edison-image files copied to the Edison drive](images/windows-edison_drive_with_files.jpg)
</div>