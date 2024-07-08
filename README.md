# Lenovo V15 G2 ALC Hackintosh OpenCore EFI Folder
Hackintosh **OpenCore** EFI folder for Lenovo's V15 G2 ALC laptop.

Tested on Mac OS X Ventura 13.6.7 and OpenCore 1.0.0.
## Information
This is a OpenCore EFI folder for Lenovo's V15 G2 ALC laptop, read what works and what doesn't before using this as well as the hardware specs.

HoRNDIS has also been included due to the lack of compatible WiFi hardware.

***This comes with NootedRed enabled, if you encounter issues regarding graphics during setup, please disable it.***

Please, generate a ***NEW*** SMBios before using this, the one in here is a INVALID one. (It's recommended you use MacBookPro16,3 as the SMBios for iGPU accel.)
## Hardware Specifications
Lenovo's site includes a [PDF](https://psref.lenovo.com/syspool/Sys/PDF/Lenovo/Lenovo_V15_G2_ALC/Lenovo_V15_G2_ALC_Spec.pdf) listing the hardware of this model as well as its variations, it might help you out on finding out what your own laptop requires.

Here is what i worked with:
* **CPU:** AMD Ryzen 3 5300U
* **iGPU:** AMD Radeon Graphics
* **Audio:** High Definition (HD) Audio, Realtek® ALC3287 codec
* **Storage:** KBG50ZNS512G NVMe KIOXIA 512GB
* **WiFi and Bluetooth:** Realtek 8822CE 802.11ac 2x2 Wi-Fi® and Bluetooth 5.1, M.2 card
* **Ethernet:** Realtek RTL8111H-CG
* **TouchPad:** HID Elan (MSFT0001) TouchPad
* **Memory:** Micron Technology 8 GB 3200MHz DDR4
* **Others:** Fujitsu PS/2 Integrated Keyboard, Line-Out, USB-C and HDMI ports...

## Working
* iGPU Acceleration
* HDMI
* Bluetooth
* ALC3287 Audio
* All USB ports
* LAN and Ethernet
* Sleep and WakeUp
* Microphone
* Integrated Camera
* Line-Out port
* USB-C port
* Battery percentage and charging status (aka Battery Readouts)
* Display brightness
* Function Keys!
* Elan HID Touchpad and the Fujitsu PS/2 Keyboard

## Not Working
* WiFi

## Bios Configuration:
Secure Boot is off.

Virtualization is on, it didn't cause me any issues.

## Notes:
For USB, please try mapping them out yourself on Windows (or Linux if you use that), because im not a expert, and they may not work for you (although they work perfectly for me).

Same goes for ACPI patches, i really recommend you try generating them yourself--because your SSDT might not be the same as the one in here.

This EFI folder was made based on a completely unmodified (minus the NVMe drive) laptop, hence the non-working WiFi & Bluetooth due to this machine not having a compatible WiFi card - you can buy one online on eBay or AliExpress, but at that point you might as well just buy a new computer that's compatible with hackintosh or a affordable macbook (although cheap macbooks just kinda suck) that can run latest OS X.

## I have an issue.
I HIGHLY recommend you visit the friendly folks of [AMD OS X](https://amd-osx.com/) on their Discord and ask for help there.

Don't get me wrong, i don't hate helping people, it's just im not active at all on github and don't check often in here.

But if i do check GitHub and see your issue, i'll try to fix it as soon as possible!

So really, it's up to you if you want to leave your issue on Issues.

## Thanks
to:
[chefkiss's guide for amd hackintosh](https://chefkissinc.github.io/guide/)
[dortania's opencore guide](https://dortania.github.io/OpenCore-Install-Guide/)
[OS X on AMD discord](https://amd-osx.com/)
I really really appreciate all these people who made it possible to run OS X on my laptop.
