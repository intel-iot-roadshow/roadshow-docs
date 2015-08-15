---
layout: default
title: Find serial port - Windows
---

### Finding your port on a system with Windows

1. Find the port for your board called "**Intel Edison Virtual Com Port**" in Windows Device Manager. 

    ![Windows Device Manager](images/comport-win-blink.png)
    
    <div class="callout warning" markdown="1">
    It is **not** "USB Serial Port". 

    And it will not be COM1 and COM2 which are usually reserved for hardware serial ports.
    </div>

2. Select your COM port in the Arduino IDE.
  
    ![Arduino IDE COM Port Selection](images/comport-ide-blink.png)

3. Now the bottom right should match the COM port number of the **Intel Edison Virtual Com Port (COM#)** from the Device Manager.
 
    ![COM Port Verification](images/comport-verif-blink.png)

4. Once you have selected your port, continue to upload the sketch to your board.
