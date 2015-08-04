---
layout: default
title: Install a shell session manager (Screen)
---

1. Launch Terminal.

2. Install **Screen** via the `apt-get install` command.

    ```
    sudo apt-get install screen
    ```

    You may be asked for your root password. Type in your root password and press Enter.

3. Wait for Screen to finish downloading and the installation to complete.

    ![Installing Screen via Terminal](images/install_screen.jpg)

<div class="callout done" markdown="1">
You should now have a shell session manager for your Terminal.

To confirm that it has been installed, you can run the `screen` command with the `--help` flag to see what your options are.

```
sudo screen --help
```
</div>
