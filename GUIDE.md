# Build your own Ventura Hackintosh EFI for a Broadwell-U Chipset [WIP-Version]
[Getting Started]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIDE.md#getting-started

This guide is based on my own experience trying to do that some MacOS versions boots and run functionally on a Broadwell-U device; now I will try explain a some steps/tips for get it:


---

. | Content Table
--- | :--:
1 | Getting Started 
2 | Creating SSDTs
3 | Fixing problems
4 | Opinions
---

---

![img](https://i.imgur.com/YKIPyaT.png)

---
## Getting Started

### Hardware Support

#### About Processors:
Any Broadwell-U processors are supported until MacOS Monterey; on Ventura, Broadwell processors (and graphics) has been dropped.

#### About dedicated/external graphic cards:
Any Nvidia GPUs are dropped from MacOS BigSur, although some Nvidia graphics may be works on latest MacOS versions, the Low Power devices (and older architectures, like Fermi, Kepler and Maxwell) don't works. 
