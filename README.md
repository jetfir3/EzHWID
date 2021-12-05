# EzHWID w/ Core -> Non-Core Support
Easy to use and robust DL/KMS38 activation script with added ability to switch edition.  
This fork, originally from [/ExeCsrss/EzHWID/](https://github.com/ExeCsrss/EzHWID/), adds support for upgrading Core to Non-Core.  

## Overview  
Easy to use script that defeats activation on Windows 10/11 and Server 2016/2019/2022 on UEFI-GPT systems using SLIC emulation technique.

## How to  
Run the script.

Press [D] to activate permanently (only on Client operating systems).  
If everything went well you should be activated!  

Press [K] to activate till 2038 (also supported on Server).  

Press [X] to check activation status.

Press [C] to create $OEM$ folder which can be placed in source directory of Windows installation media/ISO to preactivate.  
A $OEM$ folder which uses traditional script will be created when traditional script is used to create $OEM$ folder.  
A $OEM$ folder which uses AIO script will be created when AIO script is used to create $OEM$ folder.  

Press [R] to view this read-me document.

Press [G] to open the Github repo of this project.

Press [S] to switch your edition (Windows 10 1803+ only).

Press [H] to open the discord server of this project.

Press [F] to toggle forceful mode.

## Switches  
/dl: Start installation process for DL activation and skip main menu.  
/k38: Start installation process for KMS38 activation and skip main menu.  
/silent: Used with /dl or /k38. Don't prompt user for anything.  
/force: Bypasses the message "Windows is also permanently activated." and force installs a generic key.  
/pkey: Used for specifying product key to be insalled.  

Example of syntax: EzHWID.cmd /dl /silent /force /pkey P42PH-HYD6B-Y3DHY-B79JH-CT8YK  

## Q & A
Q: Which operating systems are supported?  
A: The following Windows editions are supported,

HWID: Windows 10/11 Home (N + SL + China)  
Windows 10/11 Pro (WS + Edu) (N)  
Windows 10/11 Education (N)  
Windows 10/11 (IoT) Enterprise (Multi-session / N)  
Windows 11 SE (N)  

KMS38: Windows 10/11: Enterprise, Enterprise LTSC/LTSB, Enterprise G, Enterprise multi-session, Enterprise, Education, Pro, Pro Workstation, Pro Education, Home, Home Single Language, Home China + N editions, Windows Server 2022/2019/2016: LTSC editions (Standard, Datacenter, Essentials, Cloud Storage, Azure Core, Server ARM64), SAC editions (Standard ACor, Datacenter ACor, Azure Datacenter)  

Q: I get error "PowerShell is not installed in your system". How to fix?  
A: Enable powershell using optional features control panel.  

Q: How to upgrade edition from Core to Non-Core editions?  
A: This fork adds the ability to upgrade from Core to Non-Core.  

Q: Why did I get an error when upgrading edition from Core to Non-Core?  
A: In some cases, disabling the internet before switching editions may be needed.  
Upgrading from Core to Non-Core may produce an error.  
Ignore error, close script, reboot and edition should have switched.  

Check out [Windows-Edition-Switcher](https://github.com/jetfir3/Windows-Edition-Switcher) for an alternative Windows 10/11 edition switcher.  

## Credits
@mspaintmsi for integrated patcher method.  
@Windows_Addict and @abbodi1406 for scripting ideas and great assistance in scripting.  
@ExeCsrss for original EzHWID script(s).  
