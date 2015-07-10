---
layout: default
title: Getting Started
---

# Once connected...


<div id="toc" class="box" markdown="1">
* [Ping or visit 192.168.2.15 »](#ping-or-visit-192168215)
* [Use SSH instead of a serial connection »](#use-ssh-instead-of-a-serial-connection)
* [Program IoT board while offline »](#program-iot-board-while-offline)
</div>

<!-- <div id="related-videos" class="callout video">
* [Ethernet over USB - Intel Edison - Windows (preview)](https://drive.google.com/open?id=0B2ywC78pxngCUWJxZXJiYngycU0&authuser=0)
* [Ethernet over USB - Intel Edison - Mac (preview)](https://drive.google.com/open?id=0B2ywC78pxngCSlJtbTNmNGhVVEU&authuser=0)
</div> -->

## Ping or visit 192.168.2.15

You can now ping your Intel® Edison board on address "**192.168.2.15"** from Terminal or Command Prompt on your computer. Or visit [http://192.168.2.15](http://192.168.2.15) from your web browser.

```
ping 192.168.2.15
```

## Use SSH instead of a serial connection

Use Terminal or PuTTY to wirelessly SSH into the Intel® Edison at "192.168.2.15" instead of using a wired serial connection. 

```
ssh root@192.168.2.15
```

(You can also continue to use `ssh root@edison.local` if your device is still named "edison".)

## Program IoT board while offline

The Intel® XDK IoT Edition IDE should automatically detect your Intel® Edison board. Select "192.168.2.15:58888" from the "IoT Device" drop down to upload your programs. 

!["192.168.2.15:58888" entry selected in "IoT Device" drop down](images/xdk-select_dot_15.png)

<div class="callout troubleshooting" markdown="1">
**Ethernet over USB device not showing up Intel® XDK?**

Shell into your board and restart the XDK Daemon.

```
systemctl restart xdk-daemon
```
</div>

<div class="callout goto" markdown="1">
Return to **Ethernet over USB** for:

* [Windows »](windows.html)
* [Mac »](mac.html)
* [Linux »](linux.html)
</div>
