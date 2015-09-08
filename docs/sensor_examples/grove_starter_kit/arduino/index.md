---
layout: default
title: Arduino samples
parentUrl: ../index.html#next-steps
parentTitle: Grove Starter Kit
---

# Arduino samples for the Grove Starter Kit

1. Get the Arduino sample code created by Seeed Studio.

    <div class="callout goto" markdown="1">
    1. On the USB key: <span class="icon folder">downloads</span> → <span class="icon folder">Arduino_Code</span>
    2. Copy <span class="icon file">Sketchbook_Starter_Kit_V2.0-master.zip</span> to your computer.

    _These are the same files downloaded from the [Seeed-Studio Github repo](https://github.com/Seeed-Studio/Sketchbook_Starter_Kit_V2.0)._
    </div>

2. Double-click <span class="icon file">Sketchbook_Starter_Kit_V2.0-master.zip</span> to unzip the archive.

3. Remove ".0-master" in the folder name to make the folder name "**Sketchbook_Starter_Kit_V2**".  

4. Locate your default <span class="icon folder">Arduino</span> project folder on your computer system.

    * **Windows:** it will likely be called "My Documents\Arduino\libraries"
    * **Mac:** it will likely be called "Documents/Arduino/libraries"
    * **Linux:** it will be the "libraries" folder in your sketchbook

5. Copy the contents of <span class="icon folder">Sketchbook_Starter_Kit_V2</span> to <span class="icon folder">Arduino</span> → <span class="icon folder">libraries</span>.

6. Restart the Arduino IDE. 

7. From the Arduino IDE menu, choose **File** > **Examples**. You should now see a "**Sketchbook_Starter_Kit_V2**" option. 

8. Choose a sample project. Read the code comments to find out which pin you need to connect your Grove component to.

9. Click the **Upload icon** to upload the code to your board and run the code.

For a good hardware primer, check out the [Grove Starter Kit Wiki](http://www.seeedstudio.com/wiki/Grove_-_Starter_Kit_Plus), which includes an overview and example code for all the hardware included in the Grove Starter Kit Plus. If you have other hardware, searching for the name of your hardware in conjunction with "Arduino" will come up with example code and libraries to use. 

Note: The Intel Edison board with the Arduino expansion board and the Intel Galileo board can be treated as an Arduino Uno and is compatible with all Arduino Uno sensor shields. However it should be noted that Pins 10 and 11 on the Intel Edison board are NOT in fact capable of variable voltage output (PWM), despite being marked so on the expansion board.

<div id="next-steps" class="callout done" markdown="1">
You should now know the basics of programming the Grove components with the Arduino IDE. Ready to make your own creation? 

[Return back to the START HERE guide »](../../../#done-sensors){: .link-button .centered}
</div>