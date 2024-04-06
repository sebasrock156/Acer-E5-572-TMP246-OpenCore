# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (WIP - Ventura 13.5/Sonoma 14.1)

[Library Files]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Sonoma-beta/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases/tag/sonoma-beta02
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIDE.md
[MIRA LA GUIA]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIA.md
[DOWNLOAD OCLP]: https://github.com/dortania/OpenCore-Legacy-Patcher/releases
[FROM SOURCE]: https://github.com/dortania/OpenCore-Legacy-Patcher/blob/main/SOURCE.md

![progress](https://img.shields.io/badge/progress-finished-blue.svg)
![3Dgraphics](https://img.shields.io/badge/3Dgraphics-working_with_OCLP-orange.svg)
![periphericals](https://img.shields.io/badge/periphericals-almost_working-orange)
![installation](https://img.shields.io/badge/installation-working-green)

![img](https://i.imgur.com/EpvNpoN.png)

**⚠️ADVICE⚠️:  THIS IS A WIP PROJECT TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS**

If do you want try to build your own EFI: **[SEE THE GUIDE]** | **[MIRA LA GUIA]** para hispanohablantes.

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

For fix Graphic 3D Acceleration:
**[DOWNLOAD OCLP]** (Not works for me, but some people could use for fix it)

**NOTE⚠️: This OpenCore-Legacy Patcher is a testing and development version, built by me for try to fix graphics, if this isn't work, wait for new OCLP releases.**

**Now, the hardware**:

Hardware | Model
--- |:--:
![processor](https://i.imgur.com/hWNvzxy.png) | Core i7 (5th Gen) 5500U 2 Cores/4 Threads@2,4Ghz
![igpu](https://i.imgur.com/ywW6onH.png)| HD 5500 2GB VRAM @900Mhz (Patched)
![audio](https://i.imgur.com/A7RRuUn.png) | ALC283 (in-build)
![dgpu](https://i.imgur.com/1frTIg4.png) | GeForce 820M (Not supported on MacOS)
![wlan](https://i.imgur.com/9eDLwo9.png) | Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8168
![ddr3](https://i.imgur.com/5MAnSyf.png) | Kingston 16GB(8x2) DDR3L@1600Mhz
![ssd](https://i.imgur.com/pozDx4X.png) | Kingston A400 SSD 960GB (QLC SM2259XT Controller)
---

### Works (for now):
---

<details>

- Opencore 0.9.2 ✅

- Installer Boot ✅  (installation is a less of 40 minutes with SSD) 

- System Boot ✅  (Now, booting pretty well)

- Ethernet ✅

- Audio Card ✅  (Now it's fixed, using **-lilubetaall** and **-alcbeta** args)

- USB Devices ✅ (2.0, 3.0/3.1)

- Microphone ✅  (Fixed with beta args)

- Battery charging and stats ✅

- Screen ✅  (1366x768, 1920x1080)

- Camera ✅  (Works, but without Graphic Drivers, using FaceTime or apps that required it, is really awful).

- Wi-Fi ✅  (It's working using HeliPort)

- Bluetooth ✅ (Now it's working).
 
</details>

### Partially Works:
---

<details>

- Graphics ✅❌ (Only works with OCLP 1.1.0 installed, **-igfxvesa** argument is **NEEDED** before install OCLP).
 
- VoodooPS2Controller ✅❌  (Same bugs than Ventura).

</details>

### Not works:
---
<details>

- Touchpad ❌  (**DON'T ENABLE VoodooPS2ControllerTouchpad compliment, IT'S BROKEN**; *Some XHCI USB ports are dropped with new macOS versions, some USB 1.0/1.1 devices may not work*).

- Card reader ❌  (Try booting with their kexts causes kernel panics).

</details>


 
