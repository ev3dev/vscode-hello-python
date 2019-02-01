# vscode-hello-python
Hello World for [ev3dev] + [Visual Studio Code][code] + [Python]


## Overview
This is a git repository to help you get started programming a robot using
ev3dev in Visual Studio Code using the Python programming language.


## Prerequisites
* LEGO MINDSTORMS EV3, Dexter Industries Brick Pi, Mindsensors PiStorms, or
  FatcatLab EVB with [ev3dev] installed. **Does not work with ev3dev-jessie!
  Be sure to grab a snapshot image of ev3dev-stretch.**
* A computer (Windows, macOS, or Linux) with [Visual Studio Code][code]
  installed.


## Step-by-Step
1.  Download the [vscode-hello-python][zip] project from GitHub and unzip it.

    [zip]: https://github.com/ev3dev/vscode-hello-python/archive/master.zip

2.  Open the `vscode-hello-python-master` folder in Visual Studio Code.

    ![screenshot](.README/vscode-open-folder.png)

    ![screenshot](.README/vscode-open-folder-dialog.png)

6.  Click *Show Recommendations* when asked.

    ![screenshot](.README/vscode-show-recommendations.png)

7.  Install the `ev3dev-browser` extension. If you have Python installed on your
    computer, you can install that extension too. (Don't install it if you don't
    have Python already installed.)

    ![screenshot](.README/vscode-extensions-recommended.png)

8.  After installation completes, click *Reload* and *Reload Window*.

    ![screenshot](.README/vscode-ev3dev-browser-reload.png)

    ![screenshot](.README/vscode-reload-window.png)

9. Open the *Explorer* activity pane.

    ![screenshot](.README/vscode-explorer-icon.png)

10. Click the arrow next to *EV3DEV DEVICE BROWSER* to open it.

    ![screenshot](.README/vscode-ev3dev-browser-collapsed.png)

    ![screenshot](.README/vscode-ev3dev-browser-expanded.png)

11. Ensure that your ev3dev device is turned on and has a network connection to
    the host computer. USB, Bluetooth, Wi-Fi or wired will work.

12. Click the text where it says "Click here to connect to a device".
    A box will pop up that lists discovered devices. Select one.

    ![screenshot](.README/vscode-searching-for-devices.png)

13. Once the device has connected, you will see a green dot and the
    `/home/robot` folder.

    ![screenshot](.README/vscode-home-robot.png)

14. Press <kbd>F5</kbd> to download the program and run it.

15. The *Output* pane will automatically open and show the status of the
    program and any error/debug messages.

    ![screenshot](.README/vscode-output.png)

18. Open the source code file, `hello.py`, to learn more.


## Code Completion

To get code completion working and fix errors like "Unable to import 'ev3dev2.motor'"
you will need to install Python and the `python-ev3dev` package on your computer.

1.  If you don't already have Python installed, get it from https://python.org
    or your favorite package manager (Chocolaty, Homebrew, Apt, etc.).

2.  Then set up a virtual environment. You can type these commands on the
    built-in terminal in VS Code.

    On Windows (make sure you are using CMD, not PowerShell):

        py -3 -m venv .venv
        .venv\Scripts\activate
        python -m pip install --upgrade pip
        pip install python-ev3dev2

    Or non-Windows:

        python3 -m venv .venv
        . .venv/bin/activate
        pip install --upgrade pip
        pip install python-ev3dev2

3.  In the VS Code command pallete, run the `Python: Select Interpreter` command
    to select the `.venv` folder that you just created.

    ![screenshot](.README/vscode-python-select-interpreter.png)


[ev3dev]: http://www.ev3dev.org
[code]: https://code.visualstudio.com/
[python]: https://www.python.org/
[git]: https://git-scm.com/
[github]: https://desktop.github.com/
