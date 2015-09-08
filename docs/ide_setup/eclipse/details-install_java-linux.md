---
layout: default
title: Install Java - Linux
parentUrl: index.html#install-java
parentTitle: Intel® IoT Dev Kit Eclipse - Installation
---

1. Check if you have Java installed.

    1. Open a Terminal window.

    2. Type:

        ```
        java
        ```
      
      If you see a "The program ‘java’ can not be found" message, you do not have Java installed and you will need to install it.

2. Install a Java runtime using the `apt-get` command. You may need to enter your user password.

    ```
    sudo apt-get install default.jre
    ```
