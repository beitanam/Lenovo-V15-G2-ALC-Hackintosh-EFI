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
Lenovo's site includes a [PDF](https://psref.lenovo.com/syspool/Sys/PDF/Lenovo/Lenovo_V15_G2_ALC/Lenovo_V15_G2_ALC_Spec.pdf) listing this, it might help you out.

Here is what i worked with:
* **CPU:** AMD Ryzen 3 5300U
* **iGPU:** AMD Radeon Graphics
* **Audio:** High Definition (HD) Audio, Realtek® ALC3287 codec
* **Storage:** KBG50ZNS512G NVMe KIOXIA 512GB
* **WiFi and Bluetooth:** Realtek 8822CE 802.11ac 2x2 Wi-Fi® and Bluetooth 5.1, M.2 card
* **Ethernet:** Realtek RTL8111H-CG
* **TouchPad:** HID Elan (MSFT0001) TouchPad
* **Memory:** Micron Technology 8 GB 3200MHz DDR4
* **Others:** Fujitsu PS/2 Integrated Keyboard, Line-In, USB-C and HDMI ports...

# Untested
* HDMI

# Working
* iGPU Acceleration
* ALC3287 Audio
* All USB ports
* LAN
* Sleep and WakeUp
* Microphone
* Integrated Camera
* Line-In ports
* USB-C ports
* Battery percentage and charging status
* Display brightness
* Function Keys!
* Elan Touchpad and the Fujitsu Keyboard

# Not Working
* Bluetooth
* WiFi

# Bios Configuration:
Secure Boot on Disabled.
Virtualization is on, it didn't cause me any issues.

# Notes:
I couldn't find any other options on the BIOS as mentioned on the dortania guide except for Secure Boot.
As for USB, please try mapping them out yourself on Windows, because im not a expert, and they may not work for you (although they work perfectly for me).
