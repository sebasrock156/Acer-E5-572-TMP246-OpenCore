[BigSur]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/BigSur
[Monterey]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Monterey
[Ventura]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Ventura

# Acer Aspire V3-572G/TravelMate-P246 Hackintosh OpenCore

This is a "big" project to bring MacOS OSes for those laptops with Opencore Bootloader, for more information, click on "More info of **MacOS Version** below:

---

![img](https://i.imgur.com/h9xiMsp.png)                          |                           **More info of MacOS [BigSur]**

---

---

![img](https://i.imgur.com/Evxt8TX.png)                          |                           **More info of MacOS [Monterey]**

---

---

![img](https://i.imgur.com/vohhCJk.png)                          |                           **More info of MacOS [Ventura]**

---


**Warning ⚠️**: My hardware is inherited from Aspire E5-471G model, this EFI works with Aspire V3-572G and some Aspire E5-573G models too (anyways, I'll wanna name "E5-471MG" 😂😂😂).

<details>
 
 
![img](https://i.imgur.com/mj0FBuD.jpg)
 
 
</details>

**Firstly we will go the base hardware for those EFIs needs to work**:
---

Hardware | Model
--- |:--:
CPU | i7 5500U 2 Cores/4 Threads@2,4Ghz
iGPU| Intel HD Graphics 5500
Audio Card | Realtek ALC283
dGPU | NVIDIA GeForce 820M (Not supported on MacOS)
WLAN Card | Some Intel Card (see supported models on [BigSur] or [Monterey]
Ethernet | Realtek RTL8168
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
