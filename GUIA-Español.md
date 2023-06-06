# Build your own Ventura Hackintosh EFI for a Broadwell-U Chipset [WIP-Version]
[Primeros pasos]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA-Español.md#primeros-pasos
[Soporte de Hardware]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA-Español.md#soporte-de-hardware
[Creación de SSDTs]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA-Español.md#creación-de-ssdts
[Solucionando Problemas]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA-Español.md#solucionando-problemas
[Opiniones]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA-Español.md#opiniones


This guide is based on my own experience trying to do that some MacOS versions boots and run functionally on a Broadwell-U device; now I will try explain a some steps/tips for get it:


---

Art. | Content Table
---|:--:
1 | [Primeros Pasos]
1.1 | [Soporte de Hardware]
2 | [Creación de SSDTs]
3 | [Solucionando Problemas]
4 | [Opiniones]
---

**In my case, I'm use as base, my laptop (Acer Aspire E5-572G/TravelMateP246-MG)**


![img](https://i.imgur.com/YKIPyaT.png)

---
## Primeros Pasos

<details>

### Soporte de Hardware
 
---
#### About processors/internal graphic cards:

Any Broadwell-U processors are supported until MacOS Monterey; on Ventura, Broadwell processors (and graphics) has been dropped.
But, based on Dortania's Guide, we could fake patch our laptops for try to boot MacOS Ventura.

In this case, the supported hardware is the follow:
 
**SUPPORTED DEVICES**:
 
Processor Line | Graphics
--- | :--:
Core i7 Series (U, HQ) | HD 5500/5600/6000, Iris 6100 and Iris Pro 6200
Core i5 Series (U, H) | HD 5500/6000, Iris 6100 and Iris Pro 6200
Core i3 Series U | HD 5500 and Iris 6100
---
 
 
**NOT SUPPORTED DEVICES NATIVELY**: 
 
 Processor Line | Graphics
 --- | :--:
 Pentium U Series | HD 4100 (Basic Broadwell Graphics)
 Celeron U Series | HD 4100 (Basic Broadwell Graphics)
 
The Pentium and Celeron processors doesn't have a real framebuffer for MacOS, if you really try to use, patch like a HD 4000 (Haswell) iGPU
 
---
  
#### About dedicated/external graphic cards:

Any Nvidia GPUs are dropped from MacOS BigSur, although some Nvidia graphics may be works on latest MacOS versions, the Low Power devices (and older architectures, like Fermi, Kepler and Maxwell) don't works.
  
#### About wireless/bluetooth cards:

#### About audio cards (internal and external):

**For Internal:** In this guide, we talking about [AppleALC's supported cards] and how config it in our Hackintosh EFI.

**For External:** Any USB Audio Card DAC what is compatible with MacOS or Windows may be work.

</details>

## Creación de SSDTs

<details>
</details>

## Solucionando Problemas

<details>
</details>

## Opiniones

<details>
</details>
