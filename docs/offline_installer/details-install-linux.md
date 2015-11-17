---
layout: default
title: Install Intel® IoT DevKit offline installer - Linux
parentUrl: index.html#install-and-run-offline-installer
parentTitle: Set Up Your Computer - Offline Installer
---

1. Get the latest Intel® IoT DevKit offline installer files.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span>
    2. Copy the entire <span class="icon folder">Linux</span> folder to your computer
    </div>

2. When the file transfer is complete, go into the <span class="icon folder">Linux</span> folder you copied to your development machine.

3. Extract <span class="icon file">l_iot_dev_kit_[version].tar.gz</span> to the same directory. 

4. Go into the extracted folder <span class="icon folder">l_iot_dev_kit_[version]</span>.

5. Launch <span class="icon file">install.sh</span> to start the installer.

    ![Launch screen](images/installer-launch_screen.png)

6. Follow the installation wizard prompts. Click **Next** where needed.

7. When you reach the "**Installation Summary**" screen, click **Customize installation**.

    !["Installation Summary" screen](images/installer_linux-customize_installation.png)

8. Click **Next** on the "**Choose a destination folder**" screen.
    
    !["Choose a destination folder" screen](images/installer_linux-destination_folder.png)  

9. On the "**Select components to install**" screen, ***select one or more*** of the IDEs to install: 

    * **Arduino™ Software** -- for simplified C++ development 
    * **Eclipse™ IDE** -- for C/C++ development
    * **Intel® XDK IoT Edition** -- for JavaScript / NodeJS development

    Leave the last option ***selected***:
    
    * **Intel® Phone Flash Tool Lite** -- installs tool to flash Intel® Edison firmware

    **WARNING: If you have a previous version of an IDE installed, it will be replaced.**
    
    Click **Next**.

    ![Components screen](images/installer_linux-config_options.png)

10. On the "**Intel® Edison advanced options**" screen, leave "**Update firmware image**" selected to flash the latest firmware image directly on your Intel® Edison .

    ![Components screen](images/installer_linux-advanced_options.png)

11. When prompted, connect the device mode and UART/serial cables to your computer, along with powering the board using DC power. 

    ![Intel® Edison cables screen](images/installer_linux-cable_screen.png)

    Click **Next** when ready. 

    If the Next button is greyed out, wait one minute for the Intel® Edison to finish booting up.

12. Follow the instructions for the Phone Flash Tool Lite installer when it appears, and click **Continue** or **Install** when prompted.

13. The entire flashing process may take up to 5-6 minutes. When done, click **Finish** to close the installation wizard.

    ![Final installer screen](images/installer-finish_screen.png)
