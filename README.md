# Acer Aspire V3-472G/TravelMate P246-MG Hackintosh OpenCore (Monterey 12.x)

![img](https://i.imgur.com/ZJytYpS.png)

**Now, the hardware**:

<details>

Hardware | Model
--- |:--:
CPU | i7 5500U 2 Cores/4 Threads@2,4Ghz
iGPU| Intel HD Graphics 5500
Audio Card | Realtek ALC283
dGPU | NVIDIA GeForce 820M (Not supported on MacOS)
WLAN Card | Intel Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8111
---
 
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

## Works：

<details>
 
Opencore Bootloader 0.7.5 ✔ (DON'T USE Clear NVRAM or Reset System options) 
 
Integrated Graphics ✔ (taken by system as HD 6000) 

Native Screen ✔ (1366x768) 

Multi Screen ✔ (Native + Any up 3840x2160) 

RJ45 Ethernet Connection ✔
 
USB Ports ✔ (2.0, 3.0/3.1) 

Touchpad ✔ (It's partially working, some gestures may not work; If you use dual boot, touchpad may not work on Windows/Linux/BSD for ACPI changes)
 
HDMI ✔ (Works fully, HDMI Audio works too).

VGA ✔

Camera ✔
 
Card Reader ✔ (Now it's works) 

Keyboard shortcuts ✔ (At least, volume, touchpad and brightness control; hibernate, and network may not work)

Screen Backlit ✔ (Backlight work as in Linux distros)
**For using brightness control: pressing "Pause" (up backlit ☀+) and "Lock Scroll" (down Backlit ☼-)**.
 
Audio Card ✔ (Now it's fixed *thanks to Alejandro Barreiro from Hackintosh Hispanic 2.0 telegram group*, change "alcid" bootflag *In config.plist --> NVRAM --> Add --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> boot-args* for the supported coded for you audio hardware (list below): https://github.com/acidanthera/AppleALC/wiki/Supported-codecs).

Battery Stats & Charge level ✔ (But for ACPI modifications, may have some of battery drain)

Hibernate ✔ (If you did Dualboot with Windows, works partially in this OS)
 
Bluetooth ✔ (Fully working; this EFI build is for Intel Cards only).

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
 
</details>

## Partially work:

Apple ID's apps ✔❌ (you need to fix SMBIOS)
 

 
