---
layout: default
title: Getting Started
---

# Set Up Intel® XDK IoT Edition - Part 2: Run a Sample Project

This document will guide you through creating and running a Hello Word project (blinking the onboard LED) on either the Intel® Galileo or the Intel® Edison.


<div class="toc" markdown="1">
**Table of contents**

* [Create a project »](#create-a-project)
* [Select a target IoT device »](#select-a-target-iot-device)
* [Sync device clocks »](#sync-device-clocks)
* [Build the application »](#build-the-application)
* [Upload and run the application »](#upload-and-run-the-application)
</div>

<div class="related-videos" markdown="1">
**Related video**

[Setting Up The Intel XDK IoT Edition Part 2: Run a Sample Project](https://software.intel.com/en-us/videos/setting-up-the-intel-xdk-iot-edition-part-2-run-a-sample-project)
</div>

### Create a project

The Intel® XDK IoT Edition has various project creation options. To start, create a blinking LED project from a pre-existing sample. [View detailed instructions »](details-create_project.html)

![Animated gif: creating a project in the Intel® XDK](images/create_xdk_project-animated.gif)


### Select a target IoT device

The Intel® XDK IoT Edition will automatically detect Intel® IoT devices on your network and display them in the "IoT Device" drop down list. [View detailed instructions »](details-select_target_device.html)

![Animated gif: selecting a target device in "IoT Device" drop down list](images/select_target_device-animated.gif)


### Sync device clocks

Sync your computer's time with the clock on the target board to avoid timing issues. Do this step any time you connect to a new target IoT device or the device has been powered off. [View detailed instructions »](details-sync_clock.html)

![Animated gif: syncing PC time w/ clock on target device](images/sync_clock-animated.gif)


### Build the application

Fetch all the Node modules specified in package.json and install them on the IoT device. Run build any time you create a new project, or add/remove Node modules from an existing project. [View detailed instructions »](details-build.html)

![Animated gif: building the app](images/build-animated.gif)


---


### Upload and run the application

Upload the project files to the IoT device and run it. Remember that every time you make changes to files and you want to see the changes: (1) save the file, (2) upload, (3) run. [View detailed instructions »](details-upload_run.html)

![Animated gif: creating a project in the Intel® XDK](images/upload_run-animated.gif)


---

**Look at your Intel® IoT board for a blinking light.**

* **Intel® Galileo Gen 2**
  
  A green LED is located near the USB port.
  
  ![Green LED on Intel® Galileo Gen 2](/docs/assembly/galileo_gen_2/images/on_board_led.png)

* **Intel® Edison Kit for Arduino**
  
  The LED is located near the center of the board.

  ![Green LED on Intel® Edison](/docs/assembly/arduino_expansion_board/images/on_board_led.png)

**Congratulations, you just ran your first Intel® XDK application!**

---


### Having troubles?

Refer to the [Troubleshooting »](troubleshooting.html)

---

### Next Steps

Experiment with sample code supplied for available sensors and actuators.

* **[Grove Starter Kit - Intro »](/docs/sensor_examples/grove_starter_kit/)**
  * [JavaScript »](/docs/sensor_examples/grove_starter_kit/javascript/samples.html)
