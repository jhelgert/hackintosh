
macOS 12.4 - OpenCore 0.8.1

# Hardware

- ASRock B360M/ac-itx
- Intel i7 9700
- AMD Radeon Pro WX 5100
- 32GB DDR4-2400 RAM
- 1TB Samsung 970 EVO NVMe M.2 SSD
- BCM94360NG WiFi & Bluetooth (works OOB)
- 2x LG Ultrafine 27" 5K (i.e. LG LM270QQ2 panel but with a [Dual DP driver board](https://www.aliexpress.com/wholesale?SearchText=lm270qq2&opensearch=true)) 

# BIOS Settings

See [here](https://dortania.github.io/OpenCore-Desktop-Guide/config.plist/coffee-lake.html#intel-bios-settings).

# What works

- Audio
- All external and internal USB Ports 
- HEVC Hardware Decoding
- DRM (Amazon, Netflix, AppleTV+)
- Facetime
- iMessage
- Airdrop
- (Deep) Sleep
- Wake on Lan (WOL)

# How to use?

You only need to change the `prev-lang:kbd` key acoording to your keyboard's language (A full list can be found [here](https://github.com/acidanthera/OpenCorePkg/blob/master/Utilities/AppleKeyboardLayouts/AppleKeyboardLayouts.txt)) inside the `config.plist` and complete the `PlatformInfo/Generic` part:

1. Download [genSMBIOS.command](https://github.com/corpnewt/GenSMBIOS)
2. Run genSMBIOS.command, choose the `config.plist` and use `iMacPro1,1` SMBIOS.  
3. You are ready to use the EFI :).
