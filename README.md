# How to use it.

First of all, you must follow the official coreboot for the [T480/X280](https://doc.coreboot.org/mainboard/lenovo/skylake.html)
When you arrive at the:

## Building Coreboot

_"You can use make menuconfig or make nconfig to select the mainboard matching your machine, enable the inclusion of the IFD/ME/GBE binaries, and select your payload and options. For example, you can also just use the following defconfig for a Thinkpad T480 with EDK2/UEFI as a payload:"_

In this part, just copy the file.
If you use the default coreboot configuration, you will encounter the following problems:
- Booting will take you into a black screen (EDK2/Tianocore UEFI interface won't appear)
- Only 4 threads will be available (alt least with my i7-8650u, but another Skylake/Kabylake are reported to fail)
- UEFI settings won't be saved, that means you cannot create/save boot entries.

![Thinkpad X280 Coreboot](https://github.com/AlguienSasaki/X280Libreboot/blob/main/2026-02-22-13-51-02-995.jpg?raw=true)
![Thinkpad X280 Coreboot EDK2 functional screen](https://github.com/AlguienSasaki/X280Libreboot/blob/main/2026-02-22-13-51-17-893.jpg?raw=true)
