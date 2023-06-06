# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (ULTRA WIP-Sonoma 14 BETA)

[Library Files]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Sonoma-beta/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIDE.md
[MIRA LA GUIA]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIA.md

![img](https://i.imgur.com/zLH08nx.png)

**⚠️ADVICE⚠️:  THIS IS A ULTRA WIP PROJECT TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS**

If do you want try to build your own EFI:
**[SEE THE GUIDE]** | **[MIRA LA GUIA]** para hispanohablantes.

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

Works (for now):
- Opencore 0.9.2 ✅
- Installer Boot ✅ (installation is a less of 40 minutes with SSD) 
- System Boot ✅ (Boots really slow, but works)
- Ethernet ✅
- Audio Card ✅❌(It's detected, but doesn't work)
- Battery charging and stats ✅
- USB Devices ✅ (2.0, 3.0/3.1)
- Screen ✅ (1366x768)
- Wi-Fi ✅❌ (It's detected, but doesn't work)

Partially Works:

- Graphics ✅❌ (Natively, doesn't work, but try to patch with OCLP 0.6.5 or newer; for enable it, delete **-igfxvesa** boot argument after to patch with OCLP; if **-igfxvesa** argument isn't available, add it for install system and first boot; this, enable the generic GPU drivers with 4MB of VRAM only).

- VoodooPS2Controller ✅❌ (For now, only works internal keyboard and external mices).

Not works:

- Touchpad ❌ ( **DON'T ENABLE VoodooPS2ControllerTouchpad compliment, IT'S BROKEN** ).

- Bluetooth ❌ (It's broken for most Hackintosh devices for now, sorry).

- Microphone ❌ (It's broken since MacOS Ventura)

- Camera ❌ (It's broken since MacOS Ventura)

- Card reader ❌ (Try booting with their kexts causes kernel panics)

**⚠️IMPORTANT NOTE⚠️**:
Use OCLP 0.6.x for fix the iGPU; this works moving and patching the [Library Files] to System , read [Library README.md] for more info.


 
