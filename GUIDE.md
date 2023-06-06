# Build your own Ventura Hackintosh EFI for a Broadwell-U Chipset [WIP-Version]
[Getting Started]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#getting-started
[Hardware Support]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#hardware-support
[Creating SSDTs]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#creating-ssdts
[Fixing Problems]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#fixing-problems
[Opinions]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#opinions


This guide is based on my own experience trying to do that some MacOS versions boots and run functionally on a Broadwell-U device; now I will try explain a some steps/tips for get it:


---

Art. | Content Table
---|:--:
1 | [Getting Started]
1.1 | [Hardware Support]
2 | [Creating SSDTs]
3 | [Fixing Problems]
4 | [Opinions]
---

**In my case, I'm use as base, my laptop (Acer Aspire E5-572G/TravelMateP246-MG)**


![img](https://i.imgur.com/YKIPyaT.png)

---
## Getting Started

<details>

### Hardware Support
 
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
 
 

**NOT SUPPORTED DEVICES NATIVELY**: 
 
 Processor Line | Graphics
 --- | :--:
 Pentium U Series | HD 4100 (Basic Broadwell Graphics)
 Celeron U Series | HD 4100 (Basic Broadwell Graphics)
 
The Pentium and Celeron processors doesn't have a real framebuffer for MacOS, if you really try to use, patch like a HD 4000 (Haswell) iGPU
 
---
---
  
#### About dedicated/external graphic cards:

Any Nvidia GPUs are dropped from MacOS BigSur, although some Nvidia graphics may be works on latest MacOS versions, the Low Power devices (and older architectures, like Fermi, Kepler and Maxwell) don't works.
  
#### About wireless/bluetooth cards:

#### About audio cards (internal and external):

**For Internal:** In this guide, we talking about [AppleALC's supported cards] and how config it in our Hackintosh EFI.

**For External:** Any USB Audio Card DAC what is compatible with MacOS or Windows may be work.

</details>

## Creating SSDTs

<details>
</details>

## Fixing Problems

<details>
</details>

## Opinions

<details>
</details>

