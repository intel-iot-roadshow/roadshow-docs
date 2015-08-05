---
layout: default
title: Select a target IoT device - Eclipse IDE
---

1. Click the "**Remote System Explorer**" tab in the top right corner of the Eclipse screen.

    !["Remote System Explorer" tab](images/eclipse-remote_system_explorer_tab.png)

2. From the "**Remote Systems**" panel on the left side, select "**galileo**".

    !["galileo" option in "Remote Systems" panel](images/eclipse-remote_systems-galileo.png)

    <div class="callout troubleshooting" markdown="1">
    **But I have an Intel® Edison board?**

    The "galileo" entry is just a nomenclature and does not affect the environment even if you have an Intel® Edison and not an Intel® Galileo.
    </div>

3. A "**Properties**" panel will update in the lower left of the Eclipse screen. Replace the entry for "**Host name**" with the IP address of your Intel® Edison or Intel® Galileo.

    ![Editing "Host name" in the "Properties" panel](images/eclipse-properties-host_name.png)

    <div class="callout troubleshooting" markdown="1">
    **Don't know the IP address?**

    Refer to:

    * [Connect Your Intel Edison to Wi-Fi → Identify the IP address](../../connectivity/wifi/details-identify_ip.html). 
    * Or use 192.168.2.15 if you're using [Ethernet over USB](../../connectivity/ethernet_over_usb/).
    </div>

<div class="callout troubleshooting" markdown="1">
**Problems with Wi-Fi? Need to program while offline?**

The dev kit Eclipse IDE requires the IP address of your IoT board in order to program it. If you are unable to get your IoT board online to the same network as your computer due to restricted or busy Wi-Fi networks, try a direct cable-based method.

**Intel® Galileo users:**

  Connect an Ethernet cable directly from your computer to the Intel® Galileo.

**Intel® Edison users:**

  Use the device mode micro-USB cable to establish an "Ethernet over USB" connection. Refer to [Ethernet over USB](../../connectivity/ethernet_over_usb/) for further instruction.
</div>