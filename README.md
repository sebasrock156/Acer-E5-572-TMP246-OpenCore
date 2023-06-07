# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (ULTRA WIP-Sonoma 14 BETA)

[Library Files]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Sonoma-beta/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIDE.md
[MIRA LA GUIA]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta/GUIA.md

![img](https://i.imgur.com/zLH08nx.png)

**⚠️ADVICE⚠️:  THIS IS A ULTRA WIP PROJECT TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS**

If do you want try to build your own EFI: **[MIRA LA GUIA]** para hispanohablantes.

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

Works (for now):
- Opencore 0.9.2 ✅
- Installer Boot ✅ (installation is a less of 40 minutes with SSD) 
- System Boot ✅ (Now, booting pretty well)
- Ethernet ✅
- Audio Card ✅ (Now it's fixed, using **-lilubetaall** and **-alcbeta** args)
- Microphone ✅ (Fixed with beta args; I'll try the same in Ventura)
- Battery charging and stats ✅
- USB Devices ✅ (2.0, 3.0/3.1)
- Screen ✅ (1366x768)
- Wi-Fi ✅ (It's working using HeliPort)

Partially Works:

- Graphics ✅❌ (Like a beta, OCLP isn't made for fix it for now, **-igfxvesa** argument is **NEEDED**).

- VoodooPS2Controller ✅❌ (For now, only works internal keyboard and external mices).

Not works:

- Touchpad ❌ ( **DON'T ENABLE VoodooPS2ControllerTouchpad compliment, IT'S BROKEN** ).

- Bluetooth ❌ (It's broken since MacOS Ventura, but is possible enable it *may not work*).

- Camera ❌ (It's broken since MacOS Ventura, it's recognize but, doesn't work for Graphic Drivers fault)

- Card reader ❌ (Try booting with their kexts causes kernel panics)

**⚠️IMPORTANT NOTE⚠️**:
Use OCLP 0.6.x for fix the iGPU; this works moving and patching the [Library Files] to System , read [Library README.md] for more info.


 
