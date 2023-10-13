[MacOS BigSur]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/BigSur
[MacOS Monterey]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Monterey
[MacOS Ventura]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Ventura
[MacOS Sonoma]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Sonoma-beta
[BigSur]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/BigSur#supported-wlan-cards-by-intel
[Monterey, Ventura and Sonoma]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Monterey#supported-wlan-cards-by-intel

# Acer Aspire E5-572G/TravelMate-P246 Hackintosh OpenCore

##**PROJECT IS STOPPED FOR NOW**

This is a "big" project to bring MacOS OSes for these laptops with Opencore Bootloader, for more information, click on "More info of **MacOS Version** below:


![img](https://i.imgur.com/SP2LYM8.png)

 **More info of [MacOS BigSur]**


---

![img](https://i.imgur.com/BKvumkU.png)

**More info of [MacOS Monterey]**

---


![img](https://i.imgur.com/Y3QSYAZ.png)                                                   

**More info of [MacOS Ventura]**

---


![img](https://i.imgur.com/fjkDYMh.png)                                                   

**More info of [MacOS Sonoma]**

---

<pre> Warning ⚠️: My hardware is inherited from Aspire E5-471G model, this EFI works with Aspire V3-572G
 and some Aspire E5-573G models too (anyways, I'll wanna name "E5-471MG" 😂😂😂) </pre>
---



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
WLAN Card | Some Intel Card (see supported models on [BigSur] or [Monterey, Ventura and Sonoma])
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
