---
layout: default
title: Establish a serial connection with PuTTY
parentUrl: index.html#establish-a-serial-connection
parentTitle: Shell Access - Windows
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

<div class="callout goto" markdown="1">
For more info on using PuTTY such as saving profiles, read [Using PuTTY »](using_putty.html)
</div>
