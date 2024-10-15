# hackintosh-ideapad-3-14ABA7
## Intro

|          | Version                 |
|----------|-------------------------|
| OpenCore | 1.0.1                   |
| macOS    | Sonoma 14  |

- my friend asked me to build this (and I don't even have access to the physical laptop) so **no support will be given**, use at your own risk.
- Supported macOS versions: Only Sonoma has been tested

## Info / Disclaimer
### Info
- `boot-args` used: `keepsyms=1 debug=0x100 swd_panic=1 forceRenderStandby=0 revpatch=sbvmm PCIRootUID=1 npci=0x2000`
- `alcid`: `71`
- SMBIOS: `MacBookPro15,2`
### Usage
- You can use it however you like, except for commercial purposes (such as work environments and reselling your Hackintosh), refer to the [Psystar case](https://en.wikipedia.org/wiki/Psystar_Corporation). TLDR, you'll get your ass sued if you do so.
- Reminder that this is only a base for your OpenCore setup and should always be viewed as incomplete, and it is strongly recommended that you follow the entire OpenCore guide [here](https://dortania.github.io/OpenCore-Install-Guide/). 
- **DO NOT USE ANY INSTALLER NOT FROM APPLE**, no one knows if/how they've been tampered with, and they *always* break the APFS system volume seal, which breaks OTA updates, and are generally not trustworthy at all.
### Issues
- Sleep does not work.
- not my machine so you tell me
### Notes
- Don't use case-sensitive APFS if you want to use Steam or Adobe tools.
- After installation, open System Preferences and go to Displays -> Color, uncheck `Show profiles for this display only`, then select `sRGB IEC61966-2.1`, this will make your colors look *somewhat* right (definitely not calibrated or anything but yeah, not an 
oversaturated mess)
 
![color](https://media.discordapp.net/attachments/885809091459575828/966112499487346718/unknown.png)
## Hardware

|                                           | Specifications                                                                | macOS Compatibility                                                                                                                   |
| ----------------------------------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| ``CPU``                                   | Intel Core i5-8250U, 4 Cores / 8 Threads, 1.6GHz / 3.4GHz, 6MB L3 Cache | With native power management|
| ``Memory``                                | 8GB DDR4-3200MHz                                  |                                                                                                                                               |
| ``GPU``                                   | Intel UHD Graphics 620                                                       | With full QE/CI (Graphics accleration)|
| ``Storage``                               | Toshiba 	KBG30ZMV256G                                              |                                                                                                                                              |
| ``Screen``                                | 13.2" 768p 60Hz, TN                                            |                                                                                                                                               |
| ``Webcam``                                | Integrated HD Webcam                                                          | Works!|
| ``WiFi``                                  | Intel(R) Dual Band Wireless AC 8265                                                        | Works with Airportitlwm.kext                                                                |
| ``Bluetooth``                             | Intel                                                                         | Works. |
| ``Input & Output``                        |                     | USB map provided. |
| ``Audio``                            | Realtek ALC285                                                      |                                                                                                                                               |
| ``Battery``                               | 41Wh Lithium-ion                                                                  | Battery readout works.|
| ``Keyboard``                              | -||
| ``Touchpad``                              | I2C Precision Touchpad                                                                | No issues.                                                                                            |

Special thanks to:
- [acidanthera](https://github.com/acidanthera) - the maker of OpenCore and your favourite kexts, for making this Hackintosh possible in the first place
- [dortania people](https://github.com/orgs/dortania/people) for the OpenCore Install Guide

readme prouldly ~~stolen from~~ inspired by [beerpiss](https://github.com/beerpiss/dell-vostro-15-3568-hackintosh)'s

