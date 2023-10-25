[MacOS Sonoma]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta
[BigSur]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/BigSur#supported-wlan-cards-by-intel
[Monterey, Ventura and Sonoma]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Monterey#supported-wlan-cards-by-intel

# Acer Aspire E5-572G/TravelMate-P246 Hackintosh OpenCore

![progress](https://img.shields.io/badge/progress-developing-yellow.svg)
![571G](https://img.shields.io/badge/works-on_E5_571G-green.svg)
![572G](https://img.shields.io/badge/works-on_E5_572G-green.svg)
![573G](https://img.shields.io/badge/works-on_E5_573G-green.svg)
![TMP246](https://img.shields.io/badge/works-on_TravelMate_P246-green.svg)
[![471G](https://img.shields.io/badge/malfunctioning-on_E5_471G_click_for_info-orange.svg)](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/main/471G-INFO.md)
[![AMD OSX](https://img.shields.io/badge/AMDOSX-coming_soon-violet.svg)](https://github.com/sebasrock156/Asus-X555QA-Hackintosh)

**⚠️ PROJECT IS STOPPED FOR NOW ⚠️**

This is a "big" project to bring MacOS OSes for these laptops with Opencore Bootloader, for more information, click on "More info of **MacOS Version** below:

**More info of MacOS BigSur:**

[![MacOS BigSur](https://i.imgur.com/SP2LYM8.png)](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/BigSur)

---

**More info of MacOS Monterey:**

[![MacOS Monterey](https://i.imgur.com/BKvumkU.png)](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Monterey)

---

**More info of MacOS Ventura:**

[![MacOS Ventura](https://i.imgur.com/Y3QSYAZ.png)](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura)

---

**More info of MacOS Sonoma:**

[![MacOS Sonoma](https://i.imgur.com/fjkDYMh.png)](https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta)

---

<pre> Warning ⚠️: My hardware is inherited from Aspire E5-471G model, this EFI works with Aspire V3-572G
 and some Aspire E5-573G models too (anyways, I'll wanna name "E5-471MG" 😂😂😂) </pre>
---



<details>
 
 
![img](https://i.imgur.com/mj0FBuD.jpg)
 
 
</details>

**Firstly we will go the base hardware for those EFIs needs to work**:

---

--- |:--:
![processor](https://i.imgur.com/hWNvzxy.png) | Core i7 5500U, 2 Cores/4 Threads@2,4Ghz
![igpu](https://i.imgur.com/ywW6onH.png)| HD 5500 2GB VRAM @900Mhz
![audio](https://i.imgur.com/A7RRuUn.png) | Realtek ALC283
![dgpu](https://i.imgur.com/1frTIg4.png) | GeForce 820M (Not supported on MacOS)
![wlan](https://i.imgur.com/9eDLwo9.png) | Dual Band AC 3160 (From E5-471G) (see supported models on [BigSur] or [Monterey, Ventura and Sonoma])
Ethernet | Realtek RTL8168
![ddr3](https://i.imgur.com/5MAnSyf.png) | Kingston 8GBx2 CL11@1600Mhz
![ssd](https://i.imgur.com/pozDx4X.png) | Kingston A400 SSD 960GB (QLC SM2259XT Controller)
---

---

<details>
 
**Now, some minimum hardware recommendations**:

---

Hardware | Model
--- |:--:
RAM | Any Samsung, Hynix or Kingston DDR3 8GB(4GBx2).
Audio Card | Any Realtek Audio Card (some Broadcom cards may not work).
WLAN Card | Any Intel network card (A few Realtek cards works externally or a recommend Broadcom Apple supported card).
SATA Drive	| Any Solid State Drive (SSD) with 240GB of storage.
IDE Drive | Add a caddy for SATA Output, then, I recommend any Hard Disk with 500GB/1000GB of storage.
---
 
</details>

## Misc:
Some additional drivers and SSDTs are imported from Dell, Samsung, HP, Acer and Lenovo i7 5500U EFI Laptops, some native properties may be broken (like touchpad, keyboard shortcuts or card readers), I don't make responsible if your laptop explode later to try Hackintosh.
