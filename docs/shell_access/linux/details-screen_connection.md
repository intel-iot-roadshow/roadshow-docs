---
layout: default
title: Establish a serial connection
parentUrl: index.html#establish-a-serial-connection
parentTitle: Shell Access - Linux
---

1. Connect a micro-USB cable to the **UART/serial** micro-USB port of the Intel® Edison expansion board, and the other end to your computer.

    ![Micro-USB cable being plugged into the bottom micro-USB connector](../../assembly/arduino_expansion_board/images/uart_serial-usb_cable-before_after.png)
  
    Refer to [UART/serial micro-USB cable](../../assembly/arduino_expansion_board/details-serial_cable.html) for more detailed cable connection information.

2. Open a new Terminal window.

3. Connect to the USB serial device using Screen.

    ```
    sudo screen /dev/ttyUSB0 115200
    ```

    * "115200" indicates the baud rate. Always use 115200.

    * You may be asked for your root password. Type in your root password and press Enter.

4. When you see a blank screen, **press the Enter key**. 

    **For Intel® Edison boards running older firmware**: You may need to press the Enter key **twice**.

5. Once connected you will see a login prompt. 

    Type in "**root**" for the username and press **Enter**.

    ![Login prompt](images/screen-login_prompt.jpg)

<div class="callout troubleshooting" markdown="1">
**Don't see a "usbserial" device listed?**

* Is your IoT board powered on?
* **Do you have the UART/serial cable connected?** Refer to [UART/serial micro-USB cable](../../assembly/arduino_expansion_board/details-serial_cable.html).
</div>

<div class="callout goto" markdown="1">
For more info on using Screen such as quitting, read [Using Screen »](../mac-and-linux/using_screen.html)
</div>