# Acer Aspire V3-572G/TravelMate P246-MG Hackintosh OpenCore (WIP-Ventura 13.x)

[System README.md]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/blob/Ventura/System/Library/README.md
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/releases/tag/pre-releases

![img](https://i.imgur.com/iRjYEHF.png)

**⚠️ADVICE⚠️:  THE PROJECT HAS BEEN STOPPED FOR NOW**


**For test [DOWNLOAD HERE]**

Works (for now):
- Opencore 0.9.2 ✅
- Installer Boot ✅ (installation is a less of 35 minutes with SSD) 
- System Boot ✅ (It's fixed disabling SecureBootModel from config.plist)
- Ethernet ✅
- USB Devices ✅ (2.0, 3.0/3.1)
- VoodooPS2Controller ✅❌ (Works partially and randomly, in installation or boot, native keyborad may don't work, reboot until 3 times, if it isn't working later, try to connect a external keyboard and create a temporal user for copy EFI to disk).
- Audio Card ✅❌ (fully working; but isn't enabled)
- Screen ✅ (1366x768)
- Wi-Fi ✅ (altrough is some slow to connect)

Not works (for now):
- Touchpad ❌ (VoodooPS2Controller doesn't work full on Ventura; DON'T TRY TO USE, may break keyboard function)
- Bluetooth ❌ (I'll trying to fix it; If bluetoothd causes crash, delete to NVRAM --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> [ADD] bluetoothExternalDongleFailed and bluetoothInternalControllerInfo values).
- Graphics ❌ (seen 4MB of Memory for HD 5500 incompatibility) 

**⚠️IMPORTANT NOTE⚠️**:
Based on OpenCore Legacy Patch (OCLP) solve for legacy graphics, I'm importing some (S/L/E) files from Monterey to try run on Ventura; basically the kexts/bundles of Broadwell/HD 5XXX Graphics; try to use like a possible GPU patch. See the [System README.md] for more info.


 
