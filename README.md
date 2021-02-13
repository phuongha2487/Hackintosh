# Hackintosh

- OS: macOS Big Sur
- CPU: Intel Core i5-10400
- RAM: Kingston HyperX Fury 8GB DDR4 @2666 Mhz X2
- MB: Gigabyte B460M-DS3H (Bios F3)
- SSD:  SSD M.2 SATA Intel 540s 180GB
- Audio: Realtek ALC887
- OpenCore Version: 0.6.6
- SMBIOS: iMacPro1,1


https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#starting-point

- #ACPI:
SSDT-EC.aml => Từ SSDTTime lấy ra
SSDT-PLUG-DRTNIA.aml
SSDT-AWAC.aml
- #DeviceProperties
PciRoot(0x0)/Pci(0x2,0x0)
PciRoot(0x0)/Pci(0x1C,0x4)/Pci(0x0,0x0)
- #Kernel
Lilu.kext
VirtualSMC.kext
WhateverGreen.kext
AppleALC.kext
RealtekRTL8111.kext => Chọn bản V2.2.2
- #Drivers
HfsPlus.efi
OpenRuntime.efi
