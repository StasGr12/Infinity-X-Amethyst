# Project Infinity X for Redmi Note 14 Pro+ 5G (Amethyst)
# Instructions:
## Flashing Instuctions
Before installing please remember that:

> [!WARNING]
> **YOU are choosing to make these modifications and**
> **I am not responsible for bricked devices or dead SD cards**

### Prequirements:
- Unlocked Bootloader
### Instructions:
 1. Download and install:
   - [ADB & FASTBOOT](https://developer.android.com/tools/releases/platform-tools?hl=en)
   - [Google USB Drivers](https://developer.android.com/studio/run/win-usb?hl=en)
 2. Reboot the PC
 3. Download the ROM ZIP and boot.img from [releases](https://sourceforge.net/projects/stasgr12-builds/files/amethyst/17/Project%20Infinity%20X/) and move them to the directory with ADB & FASTBOOT
 4. Flash the recovery.img and reboot to recovery:
    - Enter the directory with ADB & FASTBOOT from CMD using cd command
    - Hold power button and volume down until the screen shows FASTBOOT
    - Plug your phone to your PC via USB and run fastboot devices in the CMD
      - If it shows a device your good to go
    - Flash the recovery.img
      - Run this command in CMD:
          ```bash
          fastboot flash recovery recovery.img
          ```
    - Reboot to recovery
      - Run this command in CMD:
      - fastboot reboot recovery
 5. Install the ROM
    - When in recovery press the Factory Reset button then press format data twice
    - Press apply update button and Apply from ADB
    - Run this command in CMD:
      ```bash
      adb sideload "ROM NAME".zip
      ```
    - Make sure that you replace "ROM NAME" with the real name of ROM zip file
    - Press the reboot to system button
 6. Enjoy!
