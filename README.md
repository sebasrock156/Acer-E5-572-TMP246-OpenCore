[BigSur]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/BigSur
[Monterey]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Monterey
[Ventura]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Ventura

# Acer Aspire V3-572G/TravelMate-P246 Hackintosh OpenCore

This is a "big" project to bring MacOS OSes for those laptops with Opencore Bootloader.

See MacOS version banners below:

**More info of MacOS [BigSur]**

![img](https://i.imgur.com/m3iq85Y.png)


**More info of MacOS [Monterey]**

![img](https://i.imgur.com/Chh5xSE.png)


**More info of MacOS [Ventura]**

![img](https://i.imgur.com/ck3AHOt.png)



**Warning ⚠️**: My hardware is inherited from Aspire E5-471G model, this EFI works with Aspire V3-572G and some Aspire E5-573G models too (anyways, I'll wanna name "E5-471MG" 😂😂😂).

<details>
 
 
![img](https://i.imgur.com/mj0FBuD.jpg)
 
 
</details>

**Firstly we will go the base hardware for those EFIs needs to work**:
---

Hardware | Model
--- |:--:
CPU | i7 5500U 2 Cores/4 Threads@2,4Ghz
iGPU| Intel HD Graphics 5500
Audio Card | Realtek ALC283
dGPU | NVIDIA GeForce 820M (Not supported on MacOS)
WLAN Card | Some Intel Card (see supported models on [BigSur] or [Monterey]
Ethernet | Realtek RTL8111
---

<details>
 
**Now, some minimum hardware recommendations**:

---

Hardware | Model
--- |:--:
RAM | Any Samsung, Hynix or Kingston DDR3 8GB(4GBx2).
Audio Card | Any Realtek Audio Card (some Broadcom cards may not work).
WLAN Card | Any Intel network card (A few Realtek cards works externally; Intel supported cards is listed below).
SATA Drive	| Any Solid State Drive (SSD) with 240GB of storage.
IDE Drive | Add a caddy for SATA Output, then, I recommend any Hard Disk with 500GB/1000GB of storage.
---
 
</details>


## Installation Method:
<details>

**Before to try it**:

Maybe you need a External Keyboard and Mouse for use, and evite use USB 3.0/3.1 for Bootable USB Drive.

1. Using any macOS BigSur/Monterey/Ventura Image based on Olarila project and Balena Ecther for doing Booteable USB Drive.

2. If macOS image won't boot, mount Booteable USB Drive ESP (EFI) partition with ESP Mounter Pro or Clover/OpenCore Configurator (MacOS) or MiniTool Partition (Windows) and replace EFI Folder with THIS repo EFI Folder.

3. Boot to USB Drive always with BIOS Secure Boot ENABLED (if you disable Secure Boot, MacOS Preinstalled on Hard Drive/Solid Drive never will boot, stuck on Apple logo; rarely boots with Secure Boot disabled). 

## Post-Installation：
 **WARNING ⚠️** : If you wanna have Dualboot with Windows or Linux, Touchpad may be don't work, OpenCore EFI modify some ACPI values (Advanced Configuration and Power Interface, a.k.a. memory access & Power from BIOS/Chipset to peripherics and motherboard components) and Touchpad (Synaptics or Elantech) crash with these modifies.

1. Mount the macOS Drive EFI Partition (with ESP Mounter Pro), later, drag EFI Folder from Booteable USB Drive and reboot.

2. Now, when you boot from your macOS Drive, go to Extras folder and run "GenSMBIOS.command", select option 2 for select included config.plist, after, select option 3 for generate a new Apple SMBIOS and Serial. This is for fix not working Apple ID and Apple Aplications.

</details>

## Applications Support:

**Warning**: Some Apple apps as iMessage, FaceTime, App Store, Apple Music and etc won't login although you have patched SMBIOS before, you need an Apple product serial compatible with Apple Support too, consult in Olarila how fix it.

## Misc:
Some additional drivers and SSDTs are imported from Dell, Samsung, HP, Acer and Lenovo i7 5500U EFI Laptops, some native properties may be broken (like touchpad, keyboard shortcuts or card readers), I don't make responsible if your laptop explode later to try Hackintosh.
