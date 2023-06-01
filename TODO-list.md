[Ventura/System/]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/tree/Ventura/System/Library
[**COMPLETLY STOPPED FOR NOW**]: https://github.com/sebasrock156/Acer-V3-572-TMP246-OpenCore/blob/Ventura/README.md

For BigSur:

- Fix card reader, at least for Realtek; Genesys and others may not work.


For Monterey:

- Try to fix touchpad gestures and delete unused kexts and patches, or not.
(This is a bug from own MacOS Monterey builds, try to use 12.4.X builds, there touchpad seems work well).

- Try to fix battery charge status (putting in a kext).

- Enable tools and drivers on OC0.9.2 for update release


For Ventura:

- Abord project in future [**COMPLETLY STOPPED FOR NOW**]

- Fix Graphics ⚠️ **URGENT, so, see [Ventura/System/] Tree**

- Fix touchpad (Later, I should try on with ApplePS2SmartTouchpad).

- Fix audio (mixing old Dell EFI and current Acer EFI; for now, audio is disabled for strange ACPI Errors, **PS: DON'T ENABLE HPET Patches, cause APCI error with Kernel Panic on MacOS, ACPI Error BSOD on Windows and some peripherical fails on Linux**
; it's solve using a older version of OpenCore).
