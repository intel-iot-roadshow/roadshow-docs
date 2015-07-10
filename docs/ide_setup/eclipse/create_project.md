---
layout: default
title: Getting Started
---

# Set Up Intel® IoT Dev Kit Eclipse - Part 2: Run a Sample Project

This document will guide you through creating and running a Hello Word project (blinking the onboard LED) on the Intel® Edison.

**Create a New Project**

1. Select **IoT DevKit > Create C/C++ IoT Project.**

   ![Create IoT Project](images/create-project-eclipse.png)

2. Type a name for your project in the **Project name** field.
   
   ![Name your IoT Project](images/project-name-eclipse.png)

3. From the Project list, select **On board LED blink C++**. Click **Next**. The SSH Connection page displays.
4. To search for connections and select your board from a list, click **Search Target**. The Create Target Connection page opens.
   
   ![Create Target Connection](images/target-connection-eclipse.png)

5. By default, Eclipse searches for boards available via the Bonjour service and displays them in a list. If your board is not displayed in the list, select the **Enable broadcast target search** check box to widen your search to all devices on    your network.
6. From the list, select your board and click **OK**.

   ![Target list](images/target-list-eclipse.png)

   Note: If you already know your board's connection information, you can type it manually. Do the following:
    * In the Connection Name field, type a name to use for the connection to your board.
    * In the Target Name field, type the IP address or host name of your board.

7. Click **Finish**. Your project is created.
8. From the **Run** drop-down list in the toolbar, select the name of your project.

   ![Run the application](images/run-app-eclipse.png)
   
9. In the **User ID** field, type the user name to log in to your board.

10. In the **Password** field, type the password for your board.

    ![Enter the Edison password](images/password-eclipse.png)
   
11. If a warning message about host authenticity displays, click Yes to upload and run your project.

    ![Accept the warning and upload the project](images/ssh-eclipse.png)

12. Once your project runs, you'll see an LED blinking on your board, as shown below.

<div class="callout done" markdown="1">
**Look at your Intel® Edison board for a blinking light.**
  
  The LED is located near the center of the board.

  ![Green LED on Intel® Edison](/docs/assembly/arduino_expansion_board/images/on_board_led.png)

**Congratulations, you just ran your first C++ application!**
</div>

<div class="callout troubleshooting" markdown="1">
Refer to the [Troubleshooting - Intel XDK »](troubleshooting.md)
</div>

<div id="next-steps" class="note" markdown="1">
### Next Steps

Experiment with sample code supplied for available sensors and actuators.

* **[Grove Starter Kit - Intro »](/docs/sensor_examples/grove_starter_kit/index.html)**
  * [C++ »](/docs/sensor_examples/grove_starter_kit/c/samples.html)
</div>
