---
layout: default
title: Identify the "usbserial" device name 
---

1. Launch Terminal.

    <div class="side-by-side">
      <div class="left" markdown="1">
      **Option 1:**
  
      1. Launch Spotlight (type Cmd+Space).
      2. Type "terminal". 
      3. Select the "Terminal" app.
      </div>
      <div class="right" markdown="1">
      **Option 2:**

      1. Go to Applications on your Mac. 
      2. Open Utilities. 
      3. Launch Terminal.app.
      </div>
    </div>

2. Use the "ls" command to list any connected devices.

    ```
    ls /dev/tty.*
    ```

3. Look for a device that contains "**usbserial**".

    ![the device found was "/dev/tty.usbserial-A402YSYU"](images/terminal-usbserial_device_highlighted.png)

    In this case, the device found was "/dev/tty.usbserial-A402YSYU".

<div class="callout troubleshooting" markdown="1">
**Don't see a "usbserial" device listed?**

* **Do you have the UART/serial cable connected?** Refer to [UART/serial micro-USB cable](../../assembly/arduino_expansion_board/details-serial_cable.html).

* Is your IoT board powered on?
</div>