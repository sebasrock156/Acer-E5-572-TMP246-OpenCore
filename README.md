# Acer Aspire V3-572G/TravelMate P246-MG Hackintosh OpenCore (WIP-Ventura 13.x)

[Library Files]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Ventura/System/Library
[Library README.md]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/blob/Ventura/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/releases/tag/pre-releases

![img](https://i.imgur.com/YKIPyaT.png)

**⚠️ADVICE⚠️:  THE PROJECT IS A WIP TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS, NOW IS RESUMED**


**For test [DOWNLOAD HERE]**

Works (for now):
- Opencore 0.9.2 ✅
- Installer Boot ✅ (installation is a less of 35 minutes with SSD) 
- System Boot ✅ (It's fixed disabling SecureBootModel from config.plist)
- Ethernet ✅
- Audio Card ✅ (Now, works perfect)
- USB Devices ✅ (2.0, 3.0/3.1)
- Screen ✅ (1366x768)
- Wi-Fi ✅ (altrough is some slow to connect)

Partially Works:

- Graphics ✅❌ (Natively, doesn't work, but try to patch with OCLP 0.6.5 or newer; for enable it, delete **-igfxvesa** boot argument after to patch with OCLP).

- VoodooPS2Controller ✅❌ (Works randomly, in installation doesn't work; if you do a successful instalation, maybe works when boot in first time to system and maybe you could create an user).

Not works:

- Touchpad ❌ (**DON'T TRY TO ENABLE/DISABLE IT** makes break the laptop keyboard).

- Bluetooth ❌ (I'll trying to fix it; If causes crash, delete to NVRAM --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> [ADD] bluetoothExternalDongleFailed and bluetoothInternalControllerInfo values).

**⚠️IMPORTANT NOTE⚠️**:
Use OCLP 0.6.x for fix the iGPU; this works moving and patching the [Library Files] to System , read [Library README.md] for more info.


 
