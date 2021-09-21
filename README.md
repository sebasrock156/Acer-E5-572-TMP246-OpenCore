# ACER TravelMate P246-MG Hackintosh OpenCore (Big Sur 11.x)

---

Hardware | Model
--- |:--:
CPU | i7 5500U
iGPU| Intel HD Graphics 5500
SATA Drive | SSD Crucial BX500 480GB (For a better installation)
IDE Driver | HDD Western Digital WD10SPZX (Needed for backup all your files)
RAM | Kingston & Hynix DDR3 8GB (4GB is little for MacOS, you can expand it 'till 16GB)
Audio Card | Realtek ALC283
dGPU | NVIDIA 820M (Not supported on MacOS)
Ethernet | Realtek RTL8111
---


## Works：
Integrated Graphics (taken by system as Iris HD 6100) &radic;

720P (1366x768) Screen &radic;

RJ45 Ethernet Connection &radic;

Touchpad &radic; (It's fully working)
 
HDMI &radic;

VGA &radic;

Camera &radic;

Screen Backlit&radic; (But brightness control only works manually; Backlight work as in Linux distros)

Battery Stats & Charge level &radic;

WLAN &radic; (Always that you have an Intel Dual Band *support table below*):

## Supported WLAN Cards (by Intel):
---

Generation | Models
---|:--:
3xxx | Dual Band AC 3160, Dual Band AC 3165, Dual Band AC 3168
4xxx | Dual Band AC 4165
7xxx | Dual Band AC 7260, Dual Band AC 7265
8xxx | Dual Band AC 8260, Dual Band AC 8265
9xxx | Dual Band AC 9260, Dual Band AC 9461, Dual Band AC 9462, Dual Band AC 9560 
---

## Not work (IDK how to fix it):
Bluetooth &times; (Don't use any Bluetooth Kext for fix, causes Kernel panics)

Hibernate &times; (Really, works partially)

Audio Card &times; (Recognize hardware as ALC283, but doesn't work, you can "fix" using USB Audio DACs)

Card Reader &times; (ACPI Problems)

## Installation Method:

**Before to try it:**

Maybe you need a External Keyboard and Mouse for use, and evite use USB 3.0/3.1 for Bootable USB Drive.

1. Using any macOS BigSur (or Monterrey Beta) Image based on Olarila project and Balena Ecther for doing Booteable USB Drive.

2. If macOS image won't boot, mount Booteable USB Drive ESP (EFI) partition with ESP Mounter Pro or Clover/OpenCore Configurator (MacOS) or MiniTool Partition (Windows) and replace EFI Folder with THIS repo EFI Folder.

3. Boot to USB Drive always with BIOS Secure Boot ENABLED (if you disable Secure Boot, MacOS Preinstalled on Hard Drive/Solid Drive never will boot, stuck on Apple logo). 

## Post-Installation：
 **WARNING⚠️**: If you wanna have Dualboot with Windows or Linux, Touchpad may be don't work, OpenCore EFI modify some ACPI (BIOS Memory) directions and Touchpad (Synaptics or Elantech) crash with that modifies.

1. Mount the macOS Drive EFI Partition (with ESP Mounter Pro), later, drag EFI Folder from Booteable USB Drive and reboot.

2. Now, when you boot from your macOS Drive, go to Extras folder and run "GenSMBIOS.command", select option 2 for select included config.plist, after, select option 3 for generate a new Apple SMBIOS and Serial. This is for fix not working Apple ID and Apple Aplications.

3. If you have any Intel Wi-Fi card mentioned above, move and open "HeliPort" and configurate for enable in Autostart (System Preferences), Network connection aren't the best, but works.

## Misc:
Some additional drivers and SSDTs are imported from Dell i7 5500U devices, enable for Backlight and some Keyboard controls, could be some Fn commands doesn't work correctly.
