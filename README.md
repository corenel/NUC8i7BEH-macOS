# NUC8i7BEH-macOS
My custom configurations for Hackintosh on NUC8i7BEH.

## Environment

- **Bootloader**: OpenCore 0.5.7 (for Clover EFI files, see the [archived branch](https://github.com/corenel/NUC8i7BEH-macOS/tree/clover))
- **System**: macOS Catalina 10.15.4 (19E287)
- **CPU**: Intel® Core™ i7-8559U Processor (8M Cache, up to 4.50 GHz)
- **Memory**: Curcial DDR4 2666 16GB * 2
- **Disk**: WD Black SN750 500G NVMe SSD + WD Blue 1T SATA SSD
- **Wi-Fi/Bluetooth Card**: BCM943602CDP (Installed in the replacement of SD Card Reader)
- **Monitor**: Dell P2415Q

## Usage

- My configs are based on [RehabMan's guide](https://www.tonymacx86.com/threads/guide-intel-nuc7-nuc8-using-clover-uefi-nuc7i7bxx-nuc8i7bxx-etc.261711/) and [Leesureone's EFI]([https://www.tonymacx86.com/threads/guide-intel-nuc7-nuc8-using-clover-uefi-nuc7i7bxx-nuc8i7bxx-etc.261711/page-90), you can see more details on this post.
- `EFI` directory contains files in `/EFI/`.

## Notes

- Bluetooth
  - `IntelBluetoothFirmware.kext` is disabled in `EFI/OC/config.plist`
  - `AirportBrcmFixup.kext` and `BrcmPatchRAM3.kext` are enabled in `EFI/OC/config.plist`
  - All of the USB internal headers (`HS05` and `HS06`) are enabled in `EFI/OC/Kexts/USBPorts.kext/Contents/Info.plist`
- Serial Number
  - `MLB`, `SystemSerialNumber` and `SystemUUID` are empty in `EFI/OC/config.plist`, please use yours own to replace

## Acknowledgement

- [[Guide] Intel NUC7/NUC8 using Clover UEFI (NUC7i7Bxx,NUC8i7Bxx,etc)](https://www.tonymacx86.com/threads/guide-intel-nuc7-nuc8-using-clover-uefi-nuc7i7bxx-nuc8i7bxx-etc.261711/)
- [Leesureone's EFI](https://www.tonymacx86.com/threads/guide-intel-nuc7-nuc8-using-clover-uefi-nuc7i7bxx-nuc8i7bxx-etc.261711/page-90)
- [sarkrui/NUC8i7BEH-Hackintosh-Build](https://github.com/sarkrui/NUC8i7BEH-Hackintosh-Build)

