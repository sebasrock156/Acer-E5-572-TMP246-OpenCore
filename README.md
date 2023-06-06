# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (WIP-Ventura 13.x)

[Library Files]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases/tag/ventura-05
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/GUIDE.md
[MIRA LA GUIA]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura/GUIA.md

![img](https://i.imgur.com/YKIPyaT.png)

**⚠️ADVICE⚠️:  THIS IS A WIP PROJECT TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS, NOW IS RESUMED**

If do you want try to build your own EFI:
**[SEE THE GUIDE]** | **[MIRA LA GUIA]** para hispanohablantes.

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

**Now, the hardware**:

<details>

Hardware | Model
--- |:--:
CPU | i7 5500U 2 Cores/4 Threads@2,4Ghz
iGPU| Intel HD Graphics 5500
Audio Card | Realtek ALC283
dGPU | NVIDIA GeForce 820M (Not supported on MacOS)
WLAN Card | Intel Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8168
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

Works (for now):
- Opencore 0.9.2 ✅
- Installer Boot ✅ (installation is a less of 35 minutes with SSD) 
- System Boot ✅ (It's fixed disabling SecureBootModel from config.plist)
- Ethernet ✅
- Audio Card ✅ (Now, works only audio output, I mean, headphone jack)
- Battery charging and stats ✅
- USB Devices ✅ (2.0, 3.0/3.1)
- Screen ✅ (1366x768)
- Wi-Fi ✅ (altrough is some slow to connect)

Partially Works:

- Graphics ✅❌ (Natively, doesn't work, but try to patch with OCLP 0.6.5 or newer; for enable it, delete **-igfxvesa** boot argument after to patch with OCLP; if **-igfxvesa** argument isn't available, add it for install system and first boot; this, enable the generic GPU drivers with 4MB of VRAM only).

- VoodooPS2Controller ✅❌ (Works randomly, in installation doesn't work; if you do a successful instalation, maybe works when boot in first time to system and maybe you could create an user).

Not works:

- Touchpad ❌ (**DON'T TRY TO ENABLE/DISABLE IT** makes break the laptop keyboard).

- Bluetooth ❌ (It's broken for most Hackintosh devices for now, sorry).

- Microphone ❌ (It's broken for some Security Setting of MacOS Ventura)

- Camera ❌ (It's broken for some Security Setting of MacOS Ventura)

- Card reader ❌ (Try booting with their kexts causes kernel panics)

**⚠️IMPORTANT NOTE⚠️**:
Use OCLP 0.6.x for fix the iGPU; this works moving and patching the [Library Files] to System , read [Library README.md] for more info.


 
