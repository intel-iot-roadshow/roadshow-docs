---
layout: default
title: Select a target IoT device - Intel® XDK
---

1. In the bottom left corner of the Intel® XDK, click the "**IoT Device**" drop down list which currently indicates " - Select a Device - ".

    !["IoT Device" drop down list highlighted](images/xdk-iot_device_dropdown_highlighted.png)

2. Select your target Intel® Galileo or Intel® Edison from the list. If there are multiple devices, choose based on the device name and IP address. 

    ![A target device being selected in "IoT Device" drop down list](images/xdk-iot_device_dropdown_options_and_devices.png)

<div class="callout done" markdown="1">
Wait a moment for the connection to be established. A popup window will appear to confirm the connection status. 

![Connection established message](images/xdk-connection_established.png)
</div>

<div class="callout troubleshooting" markdown="1">
**Problems with Wi-Fi? Need to program while offline?**

The Intel® XDK requires the IP address of your IoT board in order to program it. If your IoT board is online, the IP address is automatically detected in most cases. 

However, if you are unable to get your IoT board online to the same network as your computer due to restricted or busy Wi-Fi networks, try [Ethernet over USB](../../connectivity/ethernet_over_usb/) and <span class="icon bookmark">[Add a device manually](troubleshooting.html#add-a-device-manually)</span> to the drop down list.

---

**Do not see your device in the "IoT Device" drop down list?**

* Check that your Intel® IoT board is online via Wi-Fi or ethernet, and that your development computer is on the same network as the IoT board.

* If your internet network requires additional login credentials (e.g. a university Wi-Fi network), you may need to add the IP address manually. Refer to <span class="icon bookmark">[Add a device manually](troubleshooting.html#add-a-device-manually)</span> in the Troubleshooting appendix.

* If you are using Ethernet over USB for the Intel® Edison, you may need to add the IP address manually. Refer to <span class="icon bookmark">[Add a device manually](troubleshooting.html#add-a-device-manually)</span> in the Troubleshooting appendix.

* For more detailed troubleshooting steps, refer to <span class="icon bookmark">[Don't see your device in the "IoT Device" drop down list?](troubleshooting.html#dont-see-your-device-in-the-iot-device-drop-down-list)</span> in the Troubleshooting appendix.
</div>