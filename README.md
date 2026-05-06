# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (ULTRA WIP - Tahoe 26.X)

This is the Functional Phase of the EFI

![img](https://i.imgur.com/zmItFrW.png)
![img](https://i.imgur.com/CVMGCL8.png)

**⚠️ADVICE⚠️:  THIS IS A ULTRA WIP PROJECT TRYING TO RUN THE SYSTEM, MAY BE HAVE SOME ACPI PROBLEMS, IF YOU WANT TO TRY, USE THIS [PRE-RELEASE EFI](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases/tag/tahoe-pr-rc1)**


**Now, the hardware**:

Hardware | Model
--- |:--:
![processor](https://i.imgur.com/hWNvzxy.png) | Core i7 (5th Gen) 5500U 2 Cores/4 Threads@2,4Ghz
![igpu](https://i.imgur.com/ywW6onH.png)| HD 5500 2GB VRAM @900Mhz (Patched)
![audio](https://i.imgur.com/A7RRuUn.png) | ALC283 (in-build)
![dgpu](https://i.imgur.com/1frTIg4.png) | GeForce 820M (Not supported on MacOS)
![wlan](https://i.imgur.com/9eDLwo9.png) | Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8168
![ddr3](https://i.imgur.com/5MAnSyf.png) | SK Hynix 16GB(8x2) DDR3L@1600Mhz
![ssd](https://i.imgur.com/pozDx4X.png) | Kingston A400 SSD 960GB (QLC SM2259XT Controller)
---

### Works (for now):
---

<details>

- Opencore 1.0.3 ✅

- Installer Boot ✅  (installation is a less of 40 minutes with SSD) 

- System Boot ✅  (Now, booting pretty well)

- Ethernet ✅

- Audio Card ✅  (Installing AppleHDA with MyKextsInstaller)

- USB Devices ✅ (2.0, 3.0/3.1)

- Microphone ✅ 

- Screen ✅  (1366x768, 1920x1080)

- Camera ✅  (Works, but without Graphic Drivers, using FaceTime or apps that required it, is really awful).

- Wi-Fi ✅  (It's working using HeliPort)

- Bluetooth ✅ (Now it's working).
 
</details>


### Not works:
---
<details>

- Graphics ❌ (Only works with OCLP 3.X+ installed, doesn't exist a stable build for now).

- Touchpad ❌  (**DON'T ENABLE VoodooPS2ControllerTouchpad compliment, IT'S BROKEN; USE AN USB MOUSE THEN**; *Some XHCI USB ports are dropped with new macOS versions, some USB 1.0/1.1 devices may not work*).

- Keyboard ❌ (Maybe it's the same fault than Sonoma; it isn't fixed for now, **USE AN USB KEYBOARD THEN**).

- Card reader ❌  (Try booting with their kexts causes kernel panics).

- OC-Simplify integration ❌ (It's limited to work under Sequoia or earlier versions).

</details>


 
