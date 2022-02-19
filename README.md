# hackintosh-asus-prime-z490-p

Hackintosh build using OpenCore 0.7.8.

Drivers, SSDts and Kexts are at the (current) latest release.

https://dortania.github.io/OpenCore-Install-Guide/

## Hardware Specifications
|||
|-|-|
|Motherboard|[Asus PRIME Z490-P](https://www.asus.com/Motherboards-Components/Motherboards/PRIME/PRIME-Z490-P/)|
|CPU|[Intel(R) Core(TM) i5-10500 CPU @ 3.10GHz](https://ark.intel.com/content/www/us/en/ark/products/199277/intel-core-i510500-processor-12m-cache-up-to-4-50-ghz.html)|
|GPU|[AMD Radeon RX 570](https://www.amd.com/en/products/graphics/radeon-rx-570)|
|RAM|[G.Skill Ripjaws V F4-3200C16-16GVKG (32GB)](https://www.gskill.com/specification/165/184/1536110676/F4-3200C16D-16GVKB-Specification)|
|Storage|[Samsung M.2 970 Evo Plus 1TB](https://semiconductor.samsung.com/consumer-storage/internal-ssd/970evoplus/)|

### Motherboard - Asus PRIME Z490-P
|||
|-|-|
|Ethernet|Realtek RTL8111H|
|Audio|Realtek ALC887|
|BIOS|Version 1621|

### SSDTs

* [SSDT-AWAC.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-AWAC.aml)
* [SSDT-EC-USBX-DESKTOP.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml)
* [SSDT-PLUG-DRTNIA.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml)
* [SSDT-RHUB.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-RHUB.aml)

### Drivers

* [HfsPlus.efi](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)
* [OpenCanopy.efi](https://github.com/acidanthera/OpenCorePkg/tree/0.7.8)
* [OpenRuntime.efi](https://github.com/acidanthera/OpenCorePkg/tree/0.7.8)

### Kexts
* [AppleALC](https://github.com/acidanthera/AppleALC/releases/tag/1.6.9)
* [Lilu](https://github.com/acidanthera/Lilu/releases/tag/1.6.0)
* [LucyRTL8125Ethernet](https://github.com/Mieze/LucyRTL8125Ethernet/releases/tag/1.1.0)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases/tag/2.4.2)
* [SMCProcessor](https://github.com/acidanthera/VirtualSMC/releases/tag/1.2.8)
* [SMCSuperIO](https://github.com/acidanthera/VirtualSMC/releases/tag/1.2.8)
* USBMap (Create mapping using [USBMap](https://github.com/corpnewt/USBMap))
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases/tag/1.2.8)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases/tag/1.5.7)

The config.plist was crafted based on the recommendations from [this OpenCore documentation](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html). Reference the documentation that matches your own CPU.

Ensure to do a OC Clean SnapShot from [ProperTree](https://github.com/corpnewt/ProperTree) to build up your config.plist once your EFI directory has been finalised.

## Known Issues

None that I am aware of.
