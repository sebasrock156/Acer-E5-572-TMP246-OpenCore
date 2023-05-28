# Acer Aspire V3-572G/TravelMate P246-MG Hackintosh OpenCore (WIP-Ventura 13.x)

[Pre-Releases]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/releases/tag/pre-releases

![img](https://i.imgur.com/iRjYEHF.png)

**⚠️ADVICE⚠️:  THE PROJECT HAS BEEN STOPPED FOR NOW**
**For test, see the [Pre-Releases]**

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
- Bluetooth ❌ (I'll trying to fix it; possible fix: Add to NVRAM --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> [ADD] bluetoothExternalDongleFailed --> [as DATA] --> [HEX Value] 00 and [ADD] bluetoothInternalControllerInfo --> [as DATA] --> [HEX Value] 0000000000000000000000000000).
- Graphics ❌ (seen 4MB of Memory for HD 5500 incompatibility; I'll try to patch with OCLP; if not, I'll try to patch "backporting" kexts from Monterey)


 
