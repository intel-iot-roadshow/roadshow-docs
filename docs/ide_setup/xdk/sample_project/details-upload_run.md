---
layout: default
title: Upload and run the application
parentUrl: index.html#upload-and-run-the-application
parentTitle: Intel® XDK IoT Edition - Run a Sample Project
---

1. In the bottom toolbar, click the "**Upload**" icon to upload the current project to the device.

    !["Upload" button in bottom toolbar](images/xdk-upload_button.png)

2. Check the console log for a message confirming the upload.

    ![An "upload complete" message in the console](images/xdk-console-upload_complete.png)

3. In the bottom toolbar, click the "**Run**" icon to run the project that is currently uploaded.

    !["Run" button in bottom toolbar](images/xdk-run_button.png)

4. Keep an eye on the console for any runtime errors. If there are no errors, you should see the MRAA library version number outputted to the console.

    ![MRAA version number output in the console](images/xdk-mraa_version_outputted.png)

    `console.log('MRAA Version: ' + mraa.getVersion());` was declared in the app code on line 20:

    ![MRAA version number output in the code](images/xdk-mraa_console_log_code.png)

    **If you see a version number outputted, your Intel® Edison is running its first app!**
    

<div class="callout troubleshooting" markdown="1">
**Get a "cannot find module mraa" message?**

!["cannot find module mraa" message](images/xdk-console-mraa_missing.png)

Refer to the instructions in the [XDK troubleshooting guide](troubleshooting.html#get-a-cannot-find-module-mraa-message).
</div>
