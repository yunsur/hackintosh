# Hackintosh

## Intro
How to use hackintosh for Lenovo IdeaPad Y410P.
The work introduced here is gathered and collected from many sources.
You should buy Apple computer to be able to use Apple software legally in compliance with Apple's macOS EULA.

## Prerequisites
Computer		Lenovo IdeaPad Y410P Laptop
CPU				Intel Core i7-4700MQ @ 2.40G
Chipset			Lenovo (Intel HM86 Chipset)
Graphics		HD4600	(using Intel GPU only)
Audio			ALC282 @ Intel  Lynx Point High Definition Audio
Ethernet		Atheros QCA8171 Gigabit Ethernet
WiFi			Broadcom BCM94352HMB 802.11AC
Bluetooth		BCM20702 (4.0)
BIOS Version	3.08

## Update
support 10.12.x (macOS Sierra) Latest
support 10.11.x (El Capitan)
support 10.10.x (Yosemite)
support 10.9.5  (Mavericks)

## Usage
Due to the different chipset, Some sound card speaker node different, If there is no sound, Please replace Sound_driver_2.zip

Clover Patch(on the fly), Fake-PCI-ID(https://bitbucket.org/RehabMan/os-x-fake-pci-id), Support cross version upgrade.
Installed BCM94352(Wireless Adapter), Please unzip Clover_EFI_xxx/DSDT_BCM94352.zip for Clover/ACPI/patched/ folder.

System Integrity Protection (SIP) is a security technology in OS X El Capitan and later that's designed.
This can lead to limit system file modification, More info(https://support.apple.com/en-us/HT204899).
Recommend install drive for L/E(/Library/Extensions/), Next run Kext Utility.app Restore permissions and rebuild cache.
After the install drive is complete, Please open "Terminal", Must run rep.sh for Terminal(Need to enter the system password).


## Links
Clover EFI bootloader: [Link](https://sourceforge.net/projects/cloverefiboot/)
RehabMan / BrcmPatchRAM: [Link](https://bitbucket.org/RehabMan/os-x-brcmpatchram/downloads/)
RehabMan / FakeSMC: [Link](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/)
RehabMan / OS-X-ACPI-Battery-Driver: [Link](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver/downloads/)
RehabMan / OS-X-Fake-PCI-ID: [Link](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/)
RehabMan / VoodooPS2Controller: [Link](https://bitbucket.org/RehabMan/os-x-voodoo-ps2-controller/downloads/)
Mieze / AtherosE2200Ethernet：[Link](https://github.com/Mieze/AtherosE2200Ethernet)

## Thanks
panybbib
Rehabman
Mieze

## License
MIT