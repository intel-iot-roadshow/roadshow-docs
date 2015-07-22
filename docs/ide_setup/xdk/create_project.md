---
layout: default
title: Getting Started
---

# Set Up Intel® XDK IoT Edition - Part 2: Run a Sample Project

This document will guide you through creating and running a Hello Word project (blinking the onboard LED) on the Intel® Edison.

<div id="toc" class="box" markdown="1">
* [Create a project »](#create-a-project)
* [Select a target IoT device »](#select-a-target-iot-device)
* [Sync device clocks »](#sync-device-clocks)
* [Build the application »](#build-the-application)
* [Upload and run the application »](#upload-and-run-the-application)
</div>

<!-- <div id="related-videos" class="callout video">
[Setting Up The Intel XDK IoT Edition Part 2: Run a Sample Project](https://software.intel.com/en-us/videos/setting-up-the-intel-xdk-iot-edition-part-2-run-a-sample-project)
</div> -->

### Create a project

<div class="tldr" markdown="1">
The Intel® XDK IoT Edition has various project creation options. To start, create a blinking LED project from a pre-existing sample. 

[View detailed instructions »](details-create_project.html)
</div>

[![Animated gif: creating a project in the Intel® XDK](images/create_xdk_project-animated.gif)](details-create_project.html)


### Select a target IoT device

<div class="tldr" markdown="1">
The Intel® XDK IoT Edition will automatically detect Intel® IoT devices on your network and display them in the "IoT Device" drop down list. 

[View detailed instructions »](details-select_target_device.html)
</div>

[![Animated gif: selecting a target device in "IoT Device" drop down list](images/select_target_device-animated.gif)](details-select_target_device.html)


### Sync device clocks

<div class="tldr" markdown="1">
Sync your computer's time with the clock on the target board to avoid timing issues. Do this step any time you connect to a new target IoT device or the device has been powered off. 

[View detailed instructions »](details-sync_clock.html)
</div>

[![Animated gif: syncing PC time w/ clock on target device](images/sync_clock-animated.gif)](details-sync_clock.html)


### Build the application

<div class="tldr" markdown="1">
Fetch all the Node modules specified in package.json and install them on the IoT device. Run build any time you create a new project, or add/remove Node modules from an existing project. 

[View detailed instructions »](details-build.html)
</div>

[![Animated gif: building the app](images/build-animated.gif)](details-build.html)


### Upload and run the application

<div class="tldr" markdown="1">
Upload the project files to the IoT device and run it. Remember that every time you make changes to files and you want to see the changes: (1) save the file, (2) upload, (3) run. 

[View detailed instructions »](details-upload_run.html)
</div>

[![Animated gif: creating a project in the Intel® XDK](images/upload_run-animated.gif)](details-upload_run.html)


<div class="callout done" markdown="1">
**Look at your Intel® IoT board for a blinking light.**

* **Intel® Edison Kit for Arduino**
  
  The LED is located near the center of the board.

  ![Green LED on Intel® Edison](../../assembly/arduino_expansion_board/images/on_board_led.png)

**Congratulations, you just ran your first Intel® XDK application!**
</div>

<div class="callout troubleshooting" markdown="1">
**Having troubles?** Refer to the [Troubleshooting »](troubleshooting.html)
</div>

<div id="next-steps" class="note" markdown="1">
### Next Steps

Experiment with sample code supplied for available sensors and actuators.

* **[Grove Starter Kit - Intro »](../../sensor_examples/grove_starter_kit/index.html)**
  * [JavaScript »](../../sensor_examples/grove_starter_kit/javascript/samples.html)
</div>