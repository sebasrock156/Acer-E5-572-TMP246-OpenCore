# Acer TravelMate P246-MG Hackintosh OpenCore (Big Sur 11.x)

![img](https://i.imgur.com/DCbWePN.png)

---

Hardware | Model
--- |:--:
CPU | i7 5500U 2 Cores/4 Threads@2,4Ghz (You could try overclock by BCLK, but not recommended).
iGPU| Intel HD Graphics 5500
SATA Drive | SSD Crucial BX500 480GB (For a better installation)
IDE Driver | HDD Western Digital WD10SPZX (Needed for backup all your files)
RAM | Kingston & Hynix DDR3 8GB (4GB is little for MacOS, you can expand it 'till 16GB)
Audio Card | Realtek ALC283
dGPU | NVIDIA 820M (Not supported on MacOS)
WLAN Card | Intel Dual Band AC 3160
Ethernet | Realtek RTL8111
---
**Warning ⚠️**: My hardware is inherited from Aspire E5-471G model, this EFI works with Aspire E5-573G model too.
![img](https://i.imgur.com/mj0FBuD.jpg)

## Works：
Integrated Graphics (taken by system as Iris HD 6100) ✔

720P Screen (1366x768) ✔

RJ45 Ethernet Connection ✔

Touchpad ✔ (It's fully working, enable for "One touch" in System Preferences-->Trackpad)

Audio Card ✔ (Fixed, Audio driver now is correctly configured, if audio seems louder or lower change "alcid" bootflag *In config.plist --> NVRAM --> Add --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> boot-args* for the supported coded for you audio hardware (list below): https://github.com/acidanthera/AppleALC/wiki/Adding-codec-support).
 
HDMI ✔ (Works fully, HDMI Audio works too).

![img](https://i.imgur.com/chOTKRN.png)


VGA ✔

Camera ✔

Screen Backlit ✔ (But brightness control only works manually; Backlight work as in Linux distros)

Battery Stats & Charge level ✔

Hibernate ✔ (If you did Dualboot with Windows, works partially in this OS)

WLAN ✔ (Always that you have an Intel Dual Band *support table below*):

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

Bluetooth ❌ (Don't use any Bluetooth Kext for fix, causes Kernel panics)

Card Reader ❌ (ACPI Problems)

## Installation Method:

**Before to try it:**

Maybe you need a External Keyboard and Mouse for use, and evite use USB 3.0/3.1 for Bootable USB Drive.

1. Using any macOS BigSur (or Monterrey Beta) Image based on Olarila project and Balena Ecther for doing Booteable USB Drive.

2. If macOS image won't boot, mount Booteable USB Drive ESP (EFI) partition with ESP Mounter Pro or Clover/OpenCore Configurator (MacOS) or MiniTool Partition (Windows) and replace EFI Folder with THIS repo EFI Folder.

3. Boot to USB Drive always with BIOS Secure Boot ENABLED (if you disable Secure Boot, MacOS Preinstalled on Hard Drive/Solid Drive never will boot, stuck on Apple logo). 

## Post-Installation：
 **WARNING ⚠️** : If you wanna have Dualboot with Windows or Linux, Touchpad may be don't work, OpenCore EFI modify some ACPI values (Advanced Configuration and Power Interface, a.k.a. memory access & Power from BIOS/Chipset to peripherics and motherboard components) and Touchpad (Synaptics or Elantech) crash with these modifies.

1. Mount the macOS Drive EFI Partition (with ESP Mounter Pro), later, drag EFI Folder from Booteable USB Drive and reboot.

2. Now, when you boot from your macOS Drive, go to Extras folder and run "GenSMBIOS.command", select option 2 for select included config.plist, after, select option 3 for generate a new Apple SMBIOS and Serial. This is for fix not working Apple ID and Apple Aplications.

3. If you have any Intel Wi-Fi card mentioned above, move and open "HeliPort" and configurate for enable in Autostart (System Preferences), Network connection aren't the best, but works.

## Applications Support:
**Warning**: Some Apple apps as iMessage, FaceTime, App Store, Apple Music and etc won't login although you have patched SMBIOS before, you need an Apple product serial compatible with Apple Support too, consult in Olarila how fix it.

---

Developer | App(s)
---|:--:
Adobe | Photoshop, Premiere Pro, Audition, Illustrator, Acrobat DC, After Effects, XD, InDesign, etc. (2019, 20 & 21 versions)
Electronic Arts | Origin, The Sims 4, Battlefield 1 and V (worse performance than Windows).
Microsoft | Office Suite, Teams, Edge. 
Blackmagic | Davinci Resolve (17.x)
TechSmith | Camtasia Studio (latest version)
Valve | Steam (IDK if Proton is included)
Facebook | Facebook, Whatsapp, Instagram, etc.
Adobe(x2) | Lightroom/Lightroom Classic, Dreamweaver (not working) 
---


## Misc:
Some additional drivers and SSDTs are imported from Dell i7 5500U EFI Laptops, enable for backlight and some keyboard controls, could be some Fn commands doesn't work correctly, for example: Brightness control works pressing "Pause" (for up backlit) or "Lock Scroll" (for down Backlit).
