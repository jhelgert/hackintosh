
macOS 10.15.5 - OpenCore 0.5.9

# Hardware

- ASRock B360M/ac-itx
- Intel i7 9700
- AMD Radeon Pro WX 4100 (cheapest and smallest OOB working GPU with 4x DP1.4 btw)
- 32GB DDR4-2400 RAM
- 1TB Samsung 970 EVO NVMe M.2 SSD
- Native Wifi&BT via BCM94360CD (works OOB using a NGFF Adapter)
- 2x LG Ultrafine 27" 5K (i.e. LG LM270QQ2 panel but with a [Dual DP driver board](https://www.aliexpress.com/wholesale?SearchText=lm270qq2&opensearch=true)) 

# BIOS Settings

See [here](https://dortania.github.io/OpenCore-Desktop-Guide/config.plist/coffee-lake.html#intel-bios-settings).

# What works

- Audio
- All USBPorts (inclusive the internal ones)
- HEVC Hardware Decoding
- DRM (Amazon, Netflix, AppleTV+)
- Facetime/iMessage
- (Deep) Sleep

# What doesn't work so far

Haven't noticed anything up to now.

# How to use?

You only need to complete the `PlatformInfo/Generic` part inside the
`config.plist`:

1. Download [genSMBIOS.command](https://github.com/corpnewt/GenSMBIOS)
2. Run genSMBIOS.command, choose the `config.efi` and use iMacPro1,1 SMBIOS.  
3. We are ready to use the EFI :).
