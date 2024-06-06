# GA-Z77X-UP4-TH BIOS Mod

This is a BIOS modified to show all the hidden options. Some options may not work or do nothing because Gigabyte may not have implemented them correctly. These ghost options might fail, blocking the board, requiring you to start with the backup BIOS to flash the main BIOS. Therefore, it is recommended not to change these options unless you are testing and aware of the potential issues.

Hidden options, once revealed, will not lock the board if left unmodified. These options are either enabled, disabled, or have factory default values that will remain even if not shown in the BIOS interface or after restoring default settings.

## Installation Steps

1. **Flashing**: Flash the modified BIOS.
2. **Reboot PC**: Restart your computer.
3. **Enter BIOS Setup**: Restore default settings.
4. **Reboot PC**: Restart your computer.
5. **Optional**: Enter BIOS Setup and save a copy of the BIOS with default settings on a USB drive.
6. **Optional**: Reboot your computer.
7. **Enter BIOS Setup**: Enable desired options with caution. In the System section, under Advanced Settings, enable Above 4G Decoding. Optionally, disable Gfx Low Performance. Leave TOLUT options as is unless testing for potential conflicts with DSDT patch.
8. **Save, Exit, and Reboot PC**: Apply changes and restart.
9. **Run Windows**: Execute `ReBarState.exe` and select the desired number according to your VRAM (e.g., 32 for unlimited or automatic memory allocation for ReBar based on VRAM).
10. **Reboot PC**: Restart your computer.
11. **Verify ReBar**: Run Windows and check if ReBar is active and verify memory allocation using GPU-Z.

> **Note**: Your PC may shut down twice after making BIOS changes, flashing, or enabling ReBar with `ReBarState.exe`.

## Compatibility and Testing

- **GA-Z77X-UP4-TH F11C MODED**: Tested and works fine.
- **GA-Z77X-UP4-TH F11C MODED CUSTOM MOD3**: After several restarts with ReBar 16GB and CSM, the 3060 RTX works without issues, signaled by the beeper that the video card is defined.

## About the Files

- **GA-Z77X-UP4-TH F10B MODED**
- **GA-Z77X-UP4-TH F11C MODED**: Modified from the official Gigabyte website. (F11C was sourced from TweakTown forum, believed to be from Gigabyte technical support.)

### GA-Z77X-UP4-TH F11C MODED CUSTOM MOD3

Modified by Acebmxer, sourced from TweakTown forum. Changes include:

- Intel Legacy RAID ROM: 11.1.0.1413 to 13.1.0.2030
- Intel UEFI SataDriver: 11.6.0.1702 to 13.1.0.2030
- Marvell 88SE91xx SATA RAID: 1.0.0.0027 to 1.0.1.0025
- Realtek PCIe GBE Controller: 2.50 to 2.58
- Realtek EFI UNDI: 2.024
- Intel PCI Accelerated SVGA: 2137 PC 14.34 to 2170
- Sandy GOP Driver: 2.0.1023 to 2.0.1024
- Ivy GOP Driver: 3.0.1023 to 3.0.1027
- CPU MicroCode Pack (with Sandy 6A728 and Ivy 6A919)
- ME Firmware: 8.1.30.1350 to 8.1.51.1471
- Modified splash logo 2

## Credits

- [XCuri0](https://github.com/xCuri0) for making it possible to run ReBar on unsupported boards and providing instructions on GitHub.
- [fabriguzden](https://github.com/xCuri0/ReBarUEFI/files/13465369/Z77XUD5H%2BReBar%2BNVMe%2B4G.Decode.All.Options.Show.zip) for creating an example modification on the GA-Z77X-UD5H board.
- [Other motherboards with ReBar](https://github.com/xCuri0/ReBarUEFI/issues/11)
