---
layout: default
title: Identify the IP address
parentUrl: index.html#identify-the-ip-address
parentTitle: Wi-Fi
---

1. Establish a serial connection to the Intel® Edison. {% strip %}{% include shell_access.md %}{% endstrip %}

2. In newer versions of the Intel® Edison firmware you can use the `configure_edison` command with the `--showWiFiIP` flag.

    ```
    configure_edison --showWiFiIP
    ```

3. If the `--showWiFiIP` flag is not available to you, use the `ip a` command to output details of your network connection.

    ```
    ip a
    ```

4. It should be listed as "**wlan0**", inside the third listed entry. 

    ![Result after running 'ip a' command with wlan0 entry highlighted](images/ip_a_result-wlan0_highlighted.jpg)

    In this example, the IP address is "192.168.1.14". The number after the slash ("24") is the netmask (which we do not have to worry about here).

    <div class="callout troubleshooting" markdown="1">
    **Do not see an IP address in the "wlan0" entry?**
    
    Your Intel® Edison is not online via Wi-Fi. You may need to re-run the steps in [Connect to a Wi-Fi network](index.html#connect-to-a-wi-fi-network).
    </div>
