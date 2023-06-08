# Windows on ARM
Downloading Windows on Arm for free is quite a challenge, this Markdown file provides some help.

## Steps to download
Tested on M1 Air Macbook June 2022
1. Download Windows VHDX file for Arm [here](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewARM64).
2. Download UTM [here](https://mac.getutm.app/), on the App Store it's paid.
3. Open UTM and use +
4. Choose 'Virtualize'
5. Choose preconfigured Windows
6. Check 'Import VHDX Image' and 'Install Windows 10 or higher' and 'Install drivers and SPICE tools'
7. Click 'Browse' to browse for the Windows VHDX file downloaded in Step 1
8. Follow steps (you can use defaults)
9. Wait quite long till creation of VM is finished
10. Open VM & follow the steps

If you get stuck at internet connection and there is no 'I don't have internet':

11. Reboot VM
12. Wait for Language screen to load
13. Press [Shift + F10 to open CMD and type OOBE\BYPASSNRO](https://docs.getutm.app/guides/windows/), you might have to check 'Use F1, F2, etc. keys as standard function keys' in System Preferences first of MacOS
14. Wait for VM to reboot and simply follow the steps

If internet doesn't work after install:

15. Run Spice tools within Windows it's a drive and reboot
16. Set network to 'Emulated VLAN' with 'virtio-net-pci' Emulated network card
