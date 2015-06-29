---
layout: default
title: Getting Started
---

## Confirm installation of FTDI serial drivers

Look for "USB Serial Port" in Device Manager under “Ports (COM & LPT)” after plugging in the UART/serial USB cable.

![Animated gif: confirming the installation of FTDI CDM drivers](images/confirm_ftdi_cdm_drivers-animated.gif)

---

1. _Power_ the Intel® Edison via the **device mode** micro-USB port and/or via the power barrel connector.

  ![DC power supply plugged into power barrel connector](/docs/assembly/arduino_expansion_board/images/ac_power_barrel.png) or ![Micro-USB cable plugged into the top micro-USB connector](/docs/assembly/arduino_expansion_board/images/device_mode-usb-cable.png)

2. Connect a micro-USB cable to the **UART/serial** micro-USB port of the Intel® Edison expansion board, and the other end to your computer.

  ![Micro-USB cable being plugged into the bottom micro-USB connector](/docs/assembly/arduino_expansion_board/images/uart_serial-usb_cable-before_after.png)

  Refer to [UART/serial micro-USB cable](/docs/assembly/arduino_expansion_board/details-serial_cable.html) for more detailed cable connection information.

---

If you see "USB Serial Port" show up in Device Manager under "Ports (COM & LPT)", the drivers have been successfully installed. 

!["USB Serial Port" entry in Device Manager](images/device_manager-usb_serial_port.png)
