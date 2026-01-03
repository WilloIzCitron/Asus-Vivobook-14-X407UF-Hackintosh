https://github.com/theluqqass/ASUS-A407UF-OPENCORE# Asus Vivobook 14 X407UF (Kaby Lake Intel Core i3) Hackintosh (OpenCore)

## Device Information
| Component   | Name                        | Comment                                                                                             |
|-------------|-----------------------------|----------------------------------------------------------------------------------------------------|
| CPU         | Intel Core i3-7020U         |                                                                                                   |
| iGPU+dGPU   | UHD 620 + NVidia MX130      | iGPU only after macOS 10.14 (Mojave), use macOS 10.13 (High Siera) or older for dGPU support.      |
| Audio Codec | High Definition Audio (HDA) | For macOS 26 (Tahoe) you need VoodooHDA.  For macOS 15 (Sequoia) or older, You might use AppleHDA. |
| Wi-FI       | Atheros QCA9377             |                                                                                                   |
| RAM         | 12GB 2133MHz DDR4           | You need 8GB minimum of RAM to run "last" macOS.                                                   |
| Trackpad    | ELAN Touchpad               |                                                                                                   |

## Summary (Only tested on macOS 26 Tahoe)
[![macOS 26 Tahoe screenshot](https://github.com/WilloIzCitron/Asus-Vivobook-14-X407UF-Hackintosh/blob/main/.docs/image.png?raw=true)](https://github.com/WilloIzCitron/Asus-Vivobook-14-X407UF-Hackintosh/blob/main/.docs/image.png)
<details>
  <summary>
    What's still functional?
  </summary>
  
  - iGPU
  - Trackpad
  - Audio
  - Camera
  - Display
  - ...and more!
</details>

<details>
<summary>
   Issues
  </summary>
  
  - Wi-Fi, You need USB Wi-Fi Adapter or USB Ethernet Adapter to work. (need to install certain drivers)
  - Airdrop
  - Fingerprint
  - Sleep and Wake (it crashes EFI after sleep wake). if you managed to fix that, you shall read [Fixing Sleep Guide](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html).
</details>
<details>
  <summary>
    Post-installation
  </summary>
  
  - For audio, you need to install [Voodoo HDA driver for Tahoe by chris1111](https://github.com/chris1111/VoodooHDA-Tahoe)
  - For USB Wifi Adapter, Follow [this guide](https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter/blob/master/Usage-macOS-Tahoe.md)
</details>

### Bios Settings (Fully Mandatory!!)

The proper BIOS settings for Hackintosh are:
- Advanced Mode > Advanced > Storage/SATA Configuration > SATA Mode = AHCI
- Advanced Mode > Boot Configuration > CSM = Disabled
- Advanced Mode > Boot Configuration > Fast Boot = Disabled 
- Advanced Mode > Security > Secure Boot > Secure Boot Control = Disabled

## Credits
- https://dortania.github.io/OpenCore-Install-Guide/
- https://github.com/acidanthera
- https://github.com/chris1111
- https://github.com/theluqqass
