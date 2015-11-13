---
layout: default
title: Select a target IoT device
parentUrl: index.html#select-a-target-iot-device
parentTitle: Intel® XDK IoT Edition - Run a Sample Project
---

1. In the bottom left corner of the Intel® XDK, click the "**IoT Device**" drop down list which currently indicates " - Select a Device - ".

    !["IoT Device" drop down list highlighted](images/xdk-iot_device_dropdown_highlighted.png)

2. Select your target Intel® Edison from the list. 

    If you will be using Wi-Fi to program your board and there are multiple devices, choose the target based on the device name and IP address.

    If you are using Ethernet over USB, select the board with the IP address "192.168.2.15".

    ![A target device being selected in "IoT Device" drop down list](images/xdk-iot_device_dropdown_options_and_devices.png)

3. A dialog window will appear to input the login credentials of your Intel® Edison.
  
    ![Device credentials input screen](images/xdk-username_password.png)

    * **Address:** IP should be auto-filled from the target device selected in Step 2
    * **Port:** Leave port as "**58888**"
    * **User Name:** Unless you have changed it, use "**root**"
    * **Password:** Unless you have changed it, use "**intel123**"

4. Wait a moment for the connection to be established. A popup window will appear to confirm the connection status. 

    ![Connection established message](images/xdk-connection_established.png)


<div class="callout troubleshooting" markdown="1">
**Problems with Wi-Fi? Need to program while offline?**

Refer to the instructions in the [XDK troubleshooting guide](troubleshooting.html#problems-with-wi-fi-need-to-program-while-offline).

---

**Do not see your device in the "IoT Device" drop down list?**

Refer to the instructions in the [XDK troubleshooting guide](troubleshooting.html#dont-see-your-device-in-the-iot-device-drop-down-list
).
</div>