---
layout: default
title: Identify the "usbserial" device name 
parentUrl: index.html#identify-the-usbserial-device-name
parentTitle: Shell Access - Mac
---

1. Connect a micro-USB cable to the **UART/serial** micro-USB port of the Intel® Edison expansion board, and the other end to your computer.

    ![Micro-USB cable being plugged into the bottom micro-USB connector](../../assembly/arduino_expansion_board/images/uart_serial-usb_cable-before_after.png)
  
    Refer to [UART/serial micro-USB cable](../../assembly/arduino_expansion_board/details-serial_cable.html) for more detailed cable connection information.

2. Launch Terminal.

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

3. Use the "ls" command to list any connected devices.

    ```
    ls /dev/tty.*
    ```

4. Look for a device that contains "**usbserial**".

    ![the device found was "/dev/tty.usbserial-A402YSYU"](images/terminal-usbserial_device_highlighted.png)

    In this case, the device found was "/dev/tty.usbserial-A402YSYU".

<div class="callout troubleshooting" markdown="1">
**Don't see a "usbserial" device listed?**

* **Do you have the UART/serial cable connected?** Refer to [UART/serial micro-USB cable](../../assembly/arduino_expansion_board/details-serial_cable.html).
* Is your IoT board powered on?
</div>