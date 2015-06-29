---
layout: default
title: Getting Started
---

## Step 1: Prepare built-in flash storage (Windows)

Make sure there are no files on the built-in flash storage of the Intel® Edison by formatting the storage. The storage **must** be formatted as FAT32.

![Animated gif: formatting the Edison flash storage](images/format_storage-windows-animated.gif)

---

1. In order to read or write to the Intel® Edison's built-in flash storage, connect the Intel® Edison to your computer via the **device mode** micro-USB connector.

  ![Micro-USB cable being plugged into the top micro-USB connector](/docs/assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)

2. Use Windows File Explorer to format the flash storage drive. Right-click on the "**Edison**" drive that appears after plugging in the Intel® Edison to your computer, then select "Format".

  ![Right-click and select format](images/windows-format_drive.png)

3. In the "Format Edison" dialog window, keep the default settings. Click "Start".

  ![Format drive default settings](images/windows-format_settings.png)

4. In the popup, click "Ok" to confirm the formatting of the "Edison" drive. 
Formatting should only take a few seconds.

---

The "Edison" folder should now be empty.
