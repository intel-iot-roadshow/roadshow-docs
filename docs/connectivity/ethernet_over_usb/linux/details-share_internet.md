---
layout: default
title: Getting Started
---

## Share your computer's WiFi connection (optional)

Turn on Internet Sharing to cut down on Wi-Fi traffic in a crowded room. Sharing your computer's internet connection also means that you can log into networks that have HTML password pages and then share the connection with the Intel® Edison.
Internet sharing is an optional step but is highly recommended if you are at a hackathon.

---

1. (These steps coming soon! Please do a pull request with screenshots/commands if you can.)

2. Use Terminal to establish a serial connection to the Intel® Edison. {% strip %}{% include shell_access.md os="linux" %}{% endstrip %}

3. On your Intel® Edison, disconnect from any WiFi networks the board might be logged into using the wireless command line interface (`wpa_cli`) command:

    ```
    wpa_cli disconnect
    ```

4. Then use the `route` command to add a default gateway. Use the same static IP address you set in the **Network** settings in the previous section.

    ```
    route add default gw 192.168.2.2
    ```

<div class="callout done" markdown="1">
You can now use the Intel® Edison as if it is connected to the internet on its own as long as you keep the device mode micro-USB cable plugged in.

Try pinging a network from Terminal to make sure the Intel® Edison is connected to the internet through your computer's network connection:

```
ping google.com
```

(Use the Ctrl+C keyboard command to exit the ping process.)

To re-enable WiFi on the Intel® Edison, use the `configure_edison --wifi` command as described in [Connect Your Intel Edison to Wi-Fi](/docs/connectivity/wifi/connect.html).
</div>

<div class="callout troubleshooting" markdown="1">
**Unable to ping anything from the Intel® Edison?**

Unplug and replug the device mode micro-USB cable to reset the Ethernet over USB connection.
</div>