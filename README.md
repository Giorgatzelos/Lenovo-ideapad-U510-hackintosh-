# Lenovo-ideapad-U510

hackintosh
Lenovo U510 Opencore

BigSur
Monterey

For Monterey use Monterey EFI, for BigSur use BigSur EFI
Before using this EFI, make a copy of your EFI.
Specs:
Intel Core i3-3227u
Intel HD4000 integrated GPU
NVIDIA GeForce GT 625M 1GB (Unsupported)
8GB DDR4 Ram
Broadcom BCM94352Z (Network card)


What works & what doesn't:
==========================

√ Built-in keyboard

√ Built-in trackpad (multi gestures)

√ HDMI Video/Audio with hotplug

√ AirPlay mirroring to AppleTV

√ Native WiFi & Bluetooth via BCM94352Z

√ Native USB3

√ Native audio with AppleHDA

X built-in mic [never really worked ok from MacOsX 10.6 up to macOS 12.6]

√ Built-in camera

X Native power management [Broken after Yosemite IDKW]

√ Battery status

√ Backlight controls with smooth transitions, save/restore across restart

√ Accelerated graphics for HD4000.

√ wired Ethernet

X retina scaling

X Sleep/Wake [Broken After Yosemite]

√ iMessage & Facetime

√ Brightness keys on keyboard

√ Built in Card Reader


Setup SMBIOS:
Download [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
Do the following:
cd GenSMBIOS
chmod +x GenSMBIOS.command
./GenSMBIOS.command
Install MacSerial
Generate SMBIOS
Type MacBookPro12,1
You will get your SMBIOS: Type, Serial, Board Serial and SmUUID.
Edit your Config.plist either with OCC or Xcode or TextEdit:
i. Type to Generic -> SystemProductName
ii. Serial to Generic -> SystemSerialNumber
iii. Board Serial to Generic -> MLB
iv. SmUUID to Generic -> SystemUUID

Thanks
