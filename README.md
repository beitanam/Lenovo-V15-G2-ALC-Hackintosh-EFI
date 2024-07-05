# Lenovo V15 G2 ALC Hackintosh OpenCore EFI Folder
Hackintosh **OpenCore** EFI folder for Lenovo's V15 G2 ALC laptop.

Tested on Mac OS X Ventura 13.6.7 and OpenCore 1.0.0.
# Information
This is a OpenCore EFI folder for Lenovo's V15 G2 ALC laptop, read what works and what doesn't before using this as well as the hardware specs.

HoRNDIS has also been included due to the lack of compatible WiFi hardware.

***This comes with NootedRed enabled, YOU MUST DISABLE IT IF YOU WILL USE THIS FOLDER FOR SETUP!***

***NootedRed is NOT compatible with the recovery or setup system!***

Please, generate a ***NEW*** SMBios before using this, the one in here is a INVALID one.
# Hardware Specifications
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

# Untested
* HDMI

# Working
* iGPU Acceleration
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
* Elan Touchpad and the Fujitsu Keyboard

# Not Working
* Bluetooth
* WiFi

# Bios Configuration:
Secure Boot is off.

Virtualization is on, it didn't cause me any issues.

# Notes:
I couldn't find any other options on the BIOS as mentioned on the dortania guide except for Secure Boot.

As for USB, please try mapping them out yourself on Windows, because im not a expert, and they may not work for you (although they work perfectly for me).

Same goes for ACPI patches, i really recommend you try generating them yourself.

This EFI folder was made based on a completely unmodified* laptop, hence the missing WiFi due to this machine originally not having a compatible WiFi card - you can buy one online on eBay or AliExpress, but at that point you might as well just buy a new computer that's compatible with hackintosh or a affordable macbook that can run latest OS X.

* (The laptop's storage and ram have been modified, but i did not deal or touch any Kexts or options relating to Memory or Storage - mine however did not come with a SATA drive, so i can't help you if you have problems there.)
