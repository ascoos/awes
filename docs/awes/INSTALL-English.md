# ASCOOS Web Extended Studio Installation Guide

### Abbreviations
`AWES` -- Ascoos Web Extended Studio


## 1. DOWNLOAD
You can download the original `AWES` program from the addresses below.

- `Ascoos` [ https://apps.ascoos.com/awes ]
- `SourceForge` [ https://sourceforge.net/projects/ascoos-web-extended-studio ]
- `Softpedia`  [ https://www.softpedia.com/get/Internet/Servers/WEB-Servers/AWES.shtml ]
- `Github` [ https://github.com/ascoos/awes ]


## 2. INSTALLATION
Select the disk drive on which you want to run AWES.
Unzip the file to the root of the disk. This will create a folder named `AWES` and all necessary subfolders of the program.


## 3. EXECUTION AND FIRST CONFIGURATION
- Enter the Drive:\AWES\ folder and run awes.exe.

- In the action bar press the `Options` button or select from the `Tools` menu -> `Settings...` to open the program configuration window.

### General Settings
- On the first tab press the padlock buttons to unlock the dropdown menus containing the program and servers execution drives as well as the drive where the user files - domains will be located.

- Under `AWES installation drive` select the drive where you have installed AWES. 
The next field containing the path of AWES will be populated automatically.

- In the option `Users Home drive` select the drive where you will have your domains. If the new path does not exist, when you press the `Apply` button, AWES will automatically create the folders and copy the contents of the basic user `awes` to the new path.

- Then select the display language and theme of AWES.
These options apply only to the AWES environment and not to your servers or content.

- From the `AWES Other Options` settings group, select any of the options you need:
    - `Stop services on exit`: If enabled, this option will shut down the servers every time you close the `AWES` program. 
    You should be very careful with this option because you may need the servers running and accidentally close the program. 
    Of course, if your work on the servers is periodic and you need the servers only during the programming of your code and given that you want to always have `AWES` open during this task (e.g. to see the error logs of your website), then enabling this option is a very good practice.

    - `Run in background on exit` : This option is disabled. It will be implemented in the future.
    - `Create system statistics`: This option is disabled. It will be implemented in the future.
    - `Clean temporary files on exit`: If you select this option, AWES will clean up all temporary files created by it and the servers upon shutdown.