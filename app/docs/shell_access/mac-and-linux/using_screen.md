---
layout: default
title: Getting Started
---

# Using Screen - Mac / Linux

<div class="toc" markdown="1">
**Table of contents**

* [Cancel/exit an already submitted command »](#cancelexit-an-already-submitted-command)
* [Disconnect from the serial connection »](#disconnect-from-the-serial-connection)
</div>

## Cancel/exit an already submitted command

If you submitted a command and it is taking a long time to complete, or you do not want to complete it, quit the process using Ctrl+C.

1. Make sure the Terminal window has focus.

2. Type **Ctrl+C** to send a break command.


## Disconnect from the serial connection

Failing to close the Screen connection fully may stop you from being able to log in next time without rebooting the IoT board. Close Screen sessions every time you are done with your serial connection.

1. To exit your Screen session completely:

    1. Make sure the Terminal window has focus.

    2. Type **Ctrl+A** (you won't see anything displayed yet)

    3. Then type **Ctrl+\\** (the forward slash is located below Delete)

2. At the bottom of the Terminal window, you should see "Really quit and kill all your windows [y/n]". Type "**y**".

  ![A confirmation to quit screen will show up in the bottom left corner of Terminal](images/screen-quit.png)

3. You are now back in your regular Terminal command line.
