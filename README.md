
macOS 10.15.5 - OpenCore 0.5.9

# Hardware

- ASRock B360M/ac-itx
- Intel i7 9700
- AMD Radeon Pro WX 5100
- 32GB DDR4-2400 RAM
- 1TB Samsung 970 EVO NVMe M.2 SSD
- Native Wifi&BT via BCM94360CD (works OOB using a NGFF Adapter)
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

You only need to complete the `PlatformInfo/Generic` part inside the
`config.plist`:

1. Download [genSMBIOS.command](https://github.com/corpnewt/GenSMBIOS)
2. Run genSMBIOS.command, choose the `config.efi` and use iMacPro1,1 SMBIOS.  
3. We are ready to use the EFI :).
