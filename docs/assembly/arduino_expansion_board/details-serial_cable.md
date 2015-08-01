---
layout: default
title: UART/serial micro-USB cable
---

1. **Power** the Intel® Edison via the power barrel connector ***and/or** the device mode micro-USB port.

    ![DC power supply plugged into power barrel connector or micro-USB cable plugged into the top micro-USB connector](../../assembly/arduino_expansion_board/images/edison_powered.png)

2. Plug a micro-USB cable into the **_bottom_** serial micro-USB connector on the expansion board.

    ![Micro-USB cable being plugged into the bottom micro-USB connector](images/uart_serial-usb_cable-before_after.png)

3. Connect the other end of the USB cable into your computer.

    ![USB cable being plugged into laptop](images/computer-usb_cable-before_after.png)

<div class="callout info" markdown="1">
Refer to [Shell Access](../../shell_access/) for more instructions on gaining command line access.

---

Once your Intel® Edison is online and has an addressable IP address, you may find it more convenient to SSH into your board to run Linux commands. In that case, you will not need the micro-USB serial cable on a regular basis.

![Serial cable not required for SSH access](images/ssh_access-no_cable_needed.png)
</div>