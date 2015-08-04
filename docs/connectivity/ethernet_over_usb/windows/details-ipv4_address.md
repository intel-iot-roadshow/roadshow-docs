---
layout: default
title: Add static IPv4 address
---

<div class="callout warning" markdown="1">
**Have you installed the Intel® Edison Drivers?**

If you have not followed [Set Up Your Computer - Windows (manual installation)](../../../computer_setup/windows/manual_installation.html), please do so now. RNDIS drivers are included with the Intel® Edison Drivers.
</div>

1. View your **Network Connections**.
    
    <div class="side-by-side">
      <div class="left" markdown="1">
      **Windows 8**: 

      1. Right-click on the Start menu button.

      2. Select "**Network Connections**".
      </div>
      <div class="right" markdown="1">
      **Windows 7 and below**: 

      1. Go to the Windows Control Panel. 

      2. Under "**Network and Internet**", click "**View network status and tasks**".
          !["View network status and tasks" under "Network and Internet" in Control Panel](images/control_panel-view_network_status_and_tasks.png)

      3. Click "**Change Adapter Settings**" in sidebar.
          !["Change Adapter Settings" in sidebar](images/control_panel-chanage_adpater_settings.png)
      </div>
    </div>

2. Make sure your IoT board has the microswitch set to **device mode** and plug in the **device mode micro-USB cable** from your Intel® Edison to your computer. 

    Wait one minute for the Intel® Edison to finish booting up.

    ![Micro-USB cable being plugged into the top micro-USB connector](../../../assembly/arduino_expansion_board/images/device_mode-usb_cable-before_after.png)

    _Refer to [Device mode micro-USB cable](../../../assembly/arduino_expansion_board/details-device_mode_cable.html) for full assembly instructions._

3. **Right-click** on the "**Local Area Connection**" network adapter entry with the label "**Intel Edison USB RNDIS Device**", then select "**Properties**".

    <div class="side-by-side">
      <div class="left" markdown="1">
      !["Local Area Connection" network adapter entry with label "Intel Edison USB RNDIS Device"](images/control_panel-lan_adapter.png)
      </div>
      <div class="right" markdown="1">
      ![Select "Properties" in context menu](images/control_panel-context_menu-properties.png)
      </div>
    </div>

4. In the new "Local Area Connection Properties" window, select "**Internet Protocol Version 4 (TCP/IPv4)**" from the list, then click "**Properties**".

    !["Internet Protocol Version 4 (TCP/IPv4)" selected. Click "Properties" button.](images/lan_properties-ipv4-properties_button.png)

5. In the new dialog window, select "**Use the following IP address**" and change the IP information as follows:

    * **IP address**: 192.168.2.2

    * **Subnet m****ask**: 255.255.255.0 (default)

    ![Adding 192.168.2.2 static IP address](images/ipv4_properties-add_static_ip.png)

6. Click "OK" to apply your changes and close the IPv4 properties window. 

    <div class="callout troubleshooting" markdown="1">
    **IP address taken?**

    If you get a system notification that 192.168.2.2 is taken, try any IP address within the ranges of 192.168.2.1 to 192.168.2.14. 

    Do ***not*** use 192.168.2.15 which is already reserved for the USB Gadget network interface.
    </div>

7. Click "Close" in any remaining network dialog windows that are open.

<div class="callout done" markdown="1">
There is no noticeable difference to the "Local Area Connection" adapter icon. See [Once connected...](../shared/once_connected.html) to confirm a successful connection to the Intel® Edison.
</div>