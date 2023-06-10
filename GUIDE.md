[Ventura Guide]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/blob/Ventura/GUIA.md
[Metal incompatibilities problems]: https://github.com/dortania/OpenCore-Legacy-Patcher/issues/1076
[OpenCore Legacy Patcher]: https://github.com/dortania/OpenCore-Legacy-Patcher
[itlwm]: https://github.com/OpenIntelWireless/itlwm/releases/download/v2.2.0/itlwm_v2.2.0_stable.kext.zip
[HeliPort]: https://github.com/OpenIntelWireless/HeliPort


# Build your own Hackintosh EFI for Sonoma for a 5th Gen Processor (Broadwell-U) [WIP-Version]

Resume: Follow the [Ventura Guide], for thee moment MacOS Sonoma is in Beta; some differents are explained below.

### About Hardware:

Apple has dropped even more hardware with the release of MacOS 14 (Sonoma), now only Coffee Lake (8th generation Intel) and higher processors being officially supported.

Thus completely ending support for Skylake X and Kaby Lake (7th Generation) processors and graphics.

As far as we are concerned (Hackintosh), all Skylake and lower processors are completely removed from official MacOS support, so it would be advisable not to update to versions higher than MacOS 12.x.x (Monterey); but if in any case we want to try this first Beta, the advice and steps to follow are the following:

1. Change for a new SMBIOS

**With any of these, is safest that the system starts**

SMBIOS | Hardware
--- | :--:
MacBookPro15,1 | Coffee Lake, UHD 630
MacBookPro15,2 | Coffee Lake, Iris Plus 655    
MacBookPro15,3 | Coffee Lake, UHD 630  
MacBookPro15,4 | Coffee Lake, Iris Plus 645   
MacBookPro16,1 | Coffee Lake, UHD 630
MacBookPro16,2 | Ice Lake, Iris Plus G4/G7     
MacBookPro16,3 | Coffee Lake, Iris Plus 645  
MacBookPro16,4 | Coffee Lake, UHD 630
---


2. Forget about 3D acceleration (for now): For those of us with older hardware, [OpenCore Legacy Patcher] will be our solution to the GPU problem; but, until the [Metal incompatibilities problems] are resolved; we will have to do without 3D acceleration and get used to using generic drivers **VESA**; in this case, adding to our boot-args: **-igfxvesa**.


3. Getting used to using HeliPort (for now): With all the Hardware removal, Apple has dropped support for Broadcom network cards for good; On the other hand, with those of Intel, we can still have Wi-Fi via [itlwm] along with [HeliPort].


4. Solucionar problemas de audio: Solve audio problems: As a good beta version that is recognized, it will leave the audio card without working, no matter how active it is; if you come from Ventura and you had already made it work perfectly; just add in boot-args: **-lilubetaall** and **-alcbeta** in your config.plist for Sonoma.
