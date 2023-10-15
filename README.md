# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (Ventura 13.0-13.4)

[GO HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/README.md
[Library Files]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases/tag/ventura-06
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/GUIDE.md
[MIRA LA GUIA]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/GUIA.md

![progress](https://img.shields.io/badge/progress-developing-yellow.svg)
![3Dgraphics](https://img.shields.io/badge/3Dgraphics-almost_working-orange.svg)
![periphericals](https://img.shields.io/badge/periphericals-almost_working-orange)
![installation](https://img.shields.io/badge/installation-working-green)

![img](https://i.imgur.com/YKIPyaT.png)

**⚠️ADVICE⚠️: For Ventura 13.5 (or newer) and Sonoma 14 [GO HERE]**

If do you want try to build your own EFI:
**[SEE THE GUIDE]** (Unfinished)| **[MIRA LA GUIA]** para hispanohablantes (Aún inacabada).

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

**Now, the hardware**:



Hardware | Model
--- |:--:
![processor](https://i.imgur.com/hWNvzxy.png) | Core i7 5500U 2 Cores/4 Threads @2,4Ghz
![igpu](https://i.imgur.com/ywW6onH.png)| HD 5500 2GB VRAM @900Mhz
![audio](https://i.imgur.com/A7RRuUn.png) | Realtek ALC283
![dgpu](https://i.imgur.com/1frTIg4.png) | GeForce 820M (Not supported on MacOS)
![wlan](https://i.imgur.com/9eDLwo9.png) | Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8168
![ddr3](https://i.imgur.com/5MAnSyf.png) | Kingston 8GBx2 CL11@1600Mhz
![ssd](https://i.imgur.com/pozDx4X.png) | Kingston A400 SSD 960GB (QLC SM2259XT Controller)
---
 
**Now, some minimum hardware recommendations**:

<details>
 
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

### Works:
---
<details>

- Opencore 0.9.2 ✅ 

- Installer Boot ✅ (installation is a less of 35 minutes with SSD)

- System Boot ✅ (It's fixed disabling SecureBootModel from config.plist)

- Ethernet ✅

- Audio Card ✅ (Now it's fixed using **-lilubetaall** and **-alcbeta** args)

- Microphone ✅ (Now it's working)

- Camera ✅ (Now works pretty well)

- Battery charging and stats ✅

- USB Devices ✅ (2.0, 3.0/3.1)

- Screen ✅ (1366x768 to 1080x1920)

- VGA ✅ (Tested with a 1024x1280 screen)

<details>
 
 ![img](https://i.imgur.com/N6Z3nJD.png)
 
</details>

- HDMI ✅

- Screen Backlit ✅ (Backlight work as in Linux distros)

**For using brightness control: pressing "Pause" (up backlit ☀+) and "Lock Scroll" (down Backlit ☼-)**.

- Wi-Fi ✅ (altrough is some slow to connect)

- Bluetooth ✅ (Now it's working).
 
</details>


### Partially Works:

---
<details>

- Graphics ✅❌ (Natively, doesn't work (*by Apple dropped hardware with this MacOS Version*), but try to patch with OCLP 0.6.5 or newer; for enable it, delete **-igfxvesa** boot argument after to patch with OCLP; if **-igfxvesa** argument isn't available, add it for install system and first boot; this, enable the generic GPU drivers with 4MB of VRAM only).

- VoodooPS2Controller ✅❌ (Works, but touchpad is broken, **DON'T TRY TO ENABLE IT**; Internal keyboard and external devices, works; If after to boot, keyboard doesn't work, use the Touchpad shortcut and reboot to MacOS again).

</details>


### Not works:
---

<details>
 
 
- Touchpad ❌ (**DON'T TRY TO ENABLE IT** makes break the laptop keyboard).

- Card reader ❌ (Try booting with their kexts causes kernel panics)

- EA Origin ❌ (Doesn't work for OCLP patch, 3DGfx fix is PARTIAL)
</details>


**⚠️IMPORTANT NOTE⚠️**:
Use OCLP 0.6.x for fix the iGPU; this works moving and patching the [Library Files] to System , read [Library README.md] for more info.


 
