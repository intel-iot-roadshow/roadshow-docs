---
layout: default
title: Getting Started
---

## UART/serial micro-USB cable

Use the bottom micro-USB port to send serial commands to your Intel® Edison via Terminal or PuTTY. Use these commands to flash firmware, configure Wi-Fi, or identify the board's IP address.

![Animated gif: using UART/serial cable](images/serial-animated.gif)

---

1. Power the Intel® Edison via the **device mode** micro-USB port and/or via the power barrel connector.

  ![DC power supply plugged into power barrel connector](images/ac_power_barrel.png) or ![Micro-USB cable plugged into the top micro-USB connector](images/device_mode-usb-cable.png)

2. Plug a micro-USB cable into the **_bottom_** serial micro-USB connector on the expansion board. 

  ![Micro-USB cable being plugged into the bottom micro-USB connector](images/uart_serial-usb_cable-before_after.png)

3. Connect the other end of the USB cable into your computer.

  ![USB cable being plugged into laptop](images/computer-usb_cable-before_after.png)

---

Refer to [Shell Access](/docs/shell_access/) for more instructions on gaining command line access.

---

Once your Intel® Edison is online and has an addressable IP address, you may find it more convenient to SSH into your board to run Linux commands. In that case, you will not need the micro-USB serial cable on a regular basis.

![Serial cable not required for SSH access](images/ssh_access-no_cable_needed.png)

---