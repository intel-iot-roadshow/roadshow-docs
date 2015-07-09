---
layout: default
title: Getting Started
---

## Step 1: Prepare built-in flash storage (Mac)

Make sure there are no files on the built-in flash storage of the Intel® Edison by formatting the storage. The storage **must** be formatted as FAT32.

![Animated gif: formatting the Edison flash storage](images/format_storage-mac-animated.gif)

---

1. In order to read or write to the Intel® Edison's built-in flash storage, connect the Intel® Edison to your computer via the **device mode** micro-USB connector.

  ![Micro-USB cable being plugged into the top micro-USB connector](/docs/assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)

2. Use Disk Utility to format the flash storage drive. 

  **Option 1:**

  * Launch Spotlight (type Cmd+Space).
  * Type "disk". 
  * Select the "Disk Utility" app.

  **Option 2:**
  
  * Go to Applications on your Mac.
  * Open Utilities. 
  * Launch Disk Utility.app.

3. In the left hand sidebar of Disk Utility, select the "**Edison**" drive.

  ![Edison drive in Disk Utility sidebar](images/disk_utility-select_drive.png)

4. Select the "**Erase**" tab.

  ![Erase tab in Disk Utility](images/disk_utility-erase_tab.png)

5. For "**Format**", make sure "**MS-DOS (FAT)**" is selected.

  ![FAT32 selected in Disk Utility](images/disk_utility-format_fat.png)

  ---
  
  The Intel® Edison will not flash properly if the memory is not formatted as FAT32. Make sure "MS-DOS (FAT)" is selected which is FAT32.
  
  ---

6. Click the "**Erase**" button.

  ![image alt text](images/disk_utility-erase_button.png)

7. In the popup, click "**Erase**" to confirm.

---

The Intel® Edison on-board storage memory should now be formatted as FAT32 and empty. 
