This is a BIOS modified to such an extent that it shows all the hidden options, some options may not work or do nothing because perhaps Gigabyte did not implement them completely correctly, they are like ghost options or they may fail, blocking the board and you would have to start with the backup bios to flash the main bios, so it is recommended not to change those options unless you are doing tests and knowing the problems it would

These hidden options, already shown at a glance, will not lock the board if they are not modified, since they are options that are enabled or disabled or have factory default values that will always be there even if they are not shown in the bios interface and even if you restore default settings

1. Flashing
2. Reboot PC
3. Enter Bios Setup and restore default settings
4. Reboot PC
5. Optional enter Bios Setup and save your copy of the BIOS with default settings on a USB
6. Optional Reboot PC
7. Enter Bios Setup and enable all the desired options with caution and know what you are activating, then enter the System section and enter the Anvanced Settings option and enable Above 4G Decoding.
Is optional to disable Gfx Low Performance, as for the TOLUT options, leave them how is it unless you are doing testing thinking about the problems that may cause conflict with the patch DSDT 
8. Save, Exit and Reboot PC
9. Run Windows and run ReBarState.exe y select the desired number according to the amount of memory in your VRAM, by example 32 what is for Unlimited or automatic memory allocation for ReBar based on its amount of VRAM
10. Reboot PC
11. Run Windows and verify whether ReBar is active and the amount of memory allocated with GPU-Z

Note: Your PC may shut down twice after making BIOS changes, flashing, or when you enable ReBar with ReBarState.exe

I'm using GA-Z77X-UP4-TH F11C MODED and everything works fine on it. 
On GA-Z77X-UP4-TH F11C MODED CUSTOM MOD3 after several restarts with ReBar 16Gb and CSM never 
stopped working my 3060 RTX with a signal from the beeper that the video card is undefined 

About the files:
GA-Z77X-UP4-TH F10B MODED
GA-Z77X-UP4-TH F11C MODED
-the bios I modified were taken from the official Gigabyte website (F11C was taken from tweaktownforum, but as far as I understand, it was taken directly from Gigabyte technical support)

GA-Z77X-UP4-TH F11C MODED CUSTOM MOD3
-the bios I modified was taken from tweaktownforum and modified by Acebmxer, here are the changes he made:

Intel Legacy RAID ROM 11.1.0.1413 to 13.1.0.2030
Intel UEFI SataDriver 11.6.0.1702 to 13.1.0.2030
Marvell 88SE91xx SATA RAID 1.0.0.0027 to 1.0.1.0025
Realtek PCIe GBE Controller 2.50 to 2.58
Realtek EFI UNDI 2.024
Intel PCI Accelerated SVGA 2137 PC 14.34 to 2170
Sandy GOPdriver 2.0.1023 to 2.0.1024
Ivy GOPdriver 3.0.1023 to 3.0.1027
CPU MicroCode Pack (with Sandy 6A728 and Ivy 6A919)
ME Firmware 8.1.30.1350 to 8.1.51.1471
Modified splash logo 2



Credits:
XCuri0 for making it possible to run ReBar on unsupported boards and its instructions on Wiki in Github
fabriguzden for creating an example of modification on the GA-Z77X-UD5H board