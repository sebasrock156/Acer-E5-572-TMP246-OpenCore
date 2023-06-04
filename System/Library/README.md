[OC Legacy Patcher]: https://github.com/dortania/OpenCore-Legacy-Patcher/releases
## INFORMATION


> THIS IS A DISCLAIMER FOR ADVICE: The files putted here, is an referential for code schema only. don't try to putting on your system.

Using OpenCore Legacy Patch, is possible fix the HD 5xxx/6000 Drivers.

Follow the next steps for fix it:

1. Download the latest [OC Legacy Patcher] on MacOS
2. A
3. Accept manually the grants on Gatekeeper (System Settings --> Security and Privacy --> Sources)
4. Edit config.plist and delete **-igfxvesa** from **NVRAM** --> **7C436110-AB2A-4BBB-A880-FE41995C9F82** --> **boot-args**
5. Reboot and enjoy 
