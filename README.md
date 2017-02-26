# Hackintosh

## Intro
How to use hackintosh for Lenovo IdeaPad Y410P.<br>
The work introduced here is gathered and collected from many sources.<br>
You should buy Apple computer to be able to use Apple software legally in compliance with Apple's macOS EULA.<br>

## Prerequisites
*** | Raw |
---------|:---------:
Computer		| Lenovo IdeaPad Y410P Laptop   
CPU				| Intel Core i7-4700MQ @ 2.40G
Chipset			| Lenovo (Intel HM86 Chipset)
Graphics		| HD4600	(using Intel GPU only)
Audio			| ALC282 @ Intel  Lynx Point High Definition Audio
Ethernet		| Atheros QCA8171 Gigabit Ethernet
WiFi			| Broadcom BCM94352HMB 802.11AC
Bluetooth		| BCM20702 (4.0)
BIOS Version	| 3.08

## Update
support 10.12.x (macOS Sierra) Latest<br>
support 10.11.x (El Capitan)<br>
support 10.10.x (Yosemite)<br>
support 10.9.5  (Mavericks)<br>

## Usage
Due to the different chipset, Some sound card speaker node different, If there is no sound, Please replace Sound_driver_2.zip<br>

Clover Patch(on the fly), Fake-PCI-ID(https://bitbucket.org/RehabMan/os-x-fake-pci-id), Support cross version upgrade.<br>
Installed BCM94352(Wireless Adapter), Please unzip Clover_EFI_xxx/DSDT_BCM94352.zip for Clover/ACPI/patched/ folder.<br>

System Integrity Protection (SIP) is a security technology in OS X El Capitan and later that's designed.<br>
This can lead to limit system file modification, More info(https://support.apple.com/en-us/HT204899).<br>
Recommend install drive for L/E(/Library/Extensions/), Next run Kext Utility.app Restore permissions and rebuild cache.<br>
After the install drive is complete, Please open "Terminal", Must run rep.sh for Terminal(Need to enter the system password).<br>


## Links
Clover EFI bootloader: [Link](https://sourceforge.net/projects/cloverefiboot/)<br>
RehabMan / BrcmPatchRAM: [Link](https://bitbucket.org/RehabMan/os-x-brcmpatchram/downloads/)<br>
RehabMan / FakeSMC: [Link](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/)<br>
RehabMan / OS-X-ACPI-Battery-Driver: [Link](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver/downloads/)<br>
RehabMan / OS-X-Fake-PCI-ID: [Link](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/)<br>
RehabMan / VoodooPS2Controller: [Link](https://bitbucket.org/RehabMan/os-x-voodoo-ps2-controller/downloads/)<br>
Mieze / AtherosE2200Ethernet：[Link](https://github.com/Mieze/AtherosE2200Ethernet)<br>

## Thanks
panybbib<br>
Rehabman<br>
Mieze<br>

## License
[MIT](https://github.com/yunsur/hackintosh/blob/master/LICENSE)