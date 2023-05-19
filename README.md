# Acer TravelMate P246-MG Hackintosh OpenCore (Monterey 12.x)



The first pre-release is available on **RELEASE** section.

**How works (for now)**:
- Opencore Bootloader (0.7.2)
- Installation (is a bit slower than normal).
- Ethernet RJ45 Port
- Intel HD Graphics 5500 (patched in system as HD 6000)
- Touchpad (works, but not gestures)
- USB Ports
- VGA and HDMI (but HDMI audio is missing)
- SATA and IDE Drives
- Wireless/Bluetooth Card (at least Intel)
- Dualboot (W10/11 and Archlinux)

**What's not work?**:
- Brightness control (I'll try to fix it)
- Audio/Microphone (It's a fail patching ALC283 in Kernel, only works other Audio DACs as Bluetooth headsets or external USB audio jacks)
- Touchpad gestures (Monterey only detects native Apple Bluetooth trackpads)
- Hibernation (Broken from BigSur)
- Touchpad (in other OSes if you use Dualboot)
- Apple ID's apps (you need to fix SMBIOS)
- dGPU (for obvious macOS limits with NVIDIA)
 
