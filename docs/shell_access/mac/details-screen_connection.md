---
layout: default
title: Establish a serial connection
---

1. Connect to the USB serial device using the Terminal "screen" utility. 

    ```
    screen /dev/xx.usbserial-XXXXXXXX 115200
    ```

    * **Replace "/dev/xx.usbserial-XXXXXXXX" with your device's unique name.** 

    * "115200" indicates the baud rate. **Always use 115200.**

2. When you see a blank screen, **press the Enter key**.
 
    **For Intel® Edison boards running older firmware**: You may need to press the Enter key **twice**.

    ![blank screen](images/screen-blank_screen.png)

3. Once connected you will see a login prompt. 

    Type in "**root**" for the username and press **Enter**.

    ![login as "root"](images/screen-login_root.png)
