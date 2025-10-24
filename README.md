# HWXR-Release
Release versions of the PC VR [HWXR mod for Halo CE](https://github.com/bigelod/HaloCEWXR) to be run via WinlatorXR PC containers

# Credits

Thanks to LivingFray for the awesome [Halo CE VR](https://github.com/LivingFray/HaloCEVR/) mod for SteamVR, and for sharing its source code with the world.

Additional thanks to these contributors to the LivingFray Halo CE VR mod:

97saundersj, slipperfish, codyherzog, HaMM4R, teddybear082, kyanite-rock, s-ilent, TheKrisSodroski

**Note: This is a Halo CE PC VR mod that makes breaking changes from the parent mod it's based on, please do not spam any of the above developers with requests or issues related to this conversion!**

Thanks to Luboš for his work on [WinlatorXR](https://github.com/lvonasek/WinlatorXR) , Team Beef for their support of his work, and everyone else who had contributed to portable PC gaming via Winlator in all its various versions and forks.

Thanks to GmoLargey for his testing and tutorial videos!

WinlatorXR API conversion (of the VR conversion, of the original PC version of Halo: Combat Evolved) by Bigelowed

# Installation

Usage of this mod requires a full retail copy of Halo CE for PC

WinlatorXR can be installed from its [SideQuestVR page](https://sidequestvr.com/app/37320/winlatorxr) or its [GitHub page](https://github.com/lvonasek/WinlatorXR)

Tutorial videos for installation coming soon!

# Option 1: HWXR Setup EXE

This is the recommended way to install HWXR and is designed to run directly inside WinlatorXR (once you have installed **Wine Mono Installer** from the **System Tools** menu), extract the installer to your **Downloads** folder on your Quest

Install Halo CE Retail edition inside of your container, then run HWXR_Setup.exe

# Option 2: HWXR "Release Only" ZIP

This ZIP file can be extracted over top of a working Halo CE Retail install with the 1.0.10 patch for PC (not Custom Edition), I recommend using [7-Zip](https://www.7-zip.org/download.html) directly inside your container to do this, or installing Halo CE Retail to your **Downloads** folder and extracting the ZIP over that

In addition to the **Wine Mono Installer** in the **System Tools** menu required for Option 1, do these steps:

* **Copy these DLLs** from a Windows PC to C:/Windows/System32 and C:/Windows/SysWow64 directories in your container:
*  ---> vcruntime140.dll
*  ---> msvcp140.dll
*  ---> webservices.dll
*  ---> ws2_32.dll
*  ---> ws2help.dll
* **Install** the [Visual C++ All-In-One Installer](https://github.com/abbodi1406/vcredist) on your container
* **Install** the [OpenAL Installer](https://www.openal.org/downloads/) on your container

# Final step: Shortcut configuration and running
* Right-click and **Create Shortcut** to your Halo.exe file if it doesn't already exist
* Exit the container and go to the **Shortcuts** section of WinlatorXR
* Edit the shortcut to a **Custom** resolution of **1400x1400**
* Run the Halo EXE shortcut directly from this screen

# WinlatorXR Controls:

* Left Stick - Move / UI arrows
* Right Stick - Turn left/right
* Right Stick Up - Switch Weapon
* Right Stick Down - Melee Attack
* Left Grip - Jump
* Left Trigger - Zoom / Scope or ENTER for UI panels
* Right Grip - Grenade
* Right Trigger - Shoot
* Left Click - Crouch (does not move the camera vertical position)
* Right Click - NONE (WinlatorXR menu)
* Left Menu Button - Escape / Menu (hold to recenter currently not implemented)
* X - Switch Grenades
* Y - Flashlight
* B - Reload
* A - Action

[See the full project README](https://github.com/bigelod/HaloCEWXR/edit/master/README.md)
