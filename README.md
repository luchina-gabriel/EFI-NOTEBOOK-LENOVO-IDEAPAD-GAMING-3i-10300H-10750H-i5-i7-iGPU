# Notebook Lenovo Ideapad Gaming 3i - i5 10300H & i7 10750H

![overview-12 3](https://user-images.githubusercontent.com/23700365/158817960-413b6870-4d0e-4eef-b941-272ab61cd9ae.png)

# EFI Details
**Latest working macOS**: 12.3
<br>
**Current OpenCore**: 0.7.9
<br>
**Release date**: 18/03/2022

# Notebook specifications
|Item|Description|
|-|:-------:|
|CPU|Intel(R) Core(TM) i3-10300H (Also works with i7 10750H)|
|Memory|16GB DDR4 (8Gx2)|
|Storage|NVMe KBG40ZNS512G|
|GPU|Intel(R) UHD Graphics 630|
|GPU|NVIDIA GeForce GTX 1650 Ti (Unsupported)|
|Ethernet|Realtek RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller|
|WLAN|Intel Corporation Wi-Fi 6 AX201 160MHz|
|Bluetooth|Intel Bluetooth(R)|
|Audio|Realtek ALC257 HD Audio Controller|
|Display|15,6" 60Hz|
|Webcam|USB Buil-in|
|Card Reader|USB Built-in|
|TouchPad & Keyboard|PS/2 - SYNAPTICS (for ELAN001, please read instruction below)|

### Working features
- Intel UHD Graphics 630 (3072 Mb)
- Audio & Microphone
- All USB ports
- Wifi

### Don't work
- HDMI

### For ELAN0001 Trackpads

Open `config.plist` with ProperTree and:

1. Disable KEXT: VoodooI2C.kext
2. Disable KEXT: VoodooI2CHID.kext
3. Enable KEXT: VoodooI2C-ELAN0001.kext
4. Enable KEXT: VoodooI2CHID-ELAN0001.kext
5. Disable ACPI: SSDT-GPI0.aml
6. Disable ACPI: SSDT-TPD0.aml
7. Enable ACPI: SSDT-I2C.aml

Kexts: config.plist > Kernel > Add
<br>
ACPI: config.plist > ACPI > Add

## Discord - Universo Hackintosh
- [Access Discord](https://discord.universohackintosh.com.br)
