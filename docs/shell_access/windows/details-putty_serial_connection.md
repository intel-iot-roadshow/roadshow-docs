---
layout: default
title: Getting Started
---

# Establish a serial connection

Use PuTTY to establish a **serial** connection to the IoT board using the COM # you noted in the previous [Identify the serial COM port](details-identify_com_port.html) section and the baud rate **115200**.

---

1. In PuTTY, double-check that you are in the "Session" screen. 

  ![Session tab in PuTTY](images/putty-session_tab.png)

2. Select the "**Serial**" radio button under "Connection type".

  ![Serial radio button in PuTTY](images/putty-serial_radio_button.png)

3. Specify the destination you want to connect to:

  * **Serial Line**: use the **COM #** (e.g. "COM3") noted in [Identify the serial COM port](details-identify_com_port.html)
  * **Speed**: use "115200" for the baud rate
  
  ![Serial line and speed text fields in PuTTY](images/putty-serial_line_and_speed.png)

4. Click "**Open**" to connect to the board.

  ![Open connection button in PuTTY](images/putty-open_button.png)

5. When you see a blank screen, **press the Enter key**.
 
  **For Intel® Edison boards running older firmware**: You may need to press the Enter key **twice**.

  ![Blank screen in PuTTY after connecting to Intel® Edison](images/putty-blank_screen.png)

6. Once connected you will see a login prompt. 

  Type in "**root**" for the username and press **Enter**.

  ![Login as root user](images/putty-login_as_root.png)
