# Ideapad-S340-15API-Hackintosh
[![OpenCore](https://img.shields.io/badge/OpenCore-v1.0.1-blue)](https://github.com/acidanthera/OpenCorePkg)
[![MacOS-Stable](https://img.shields.io/badge/MacOS-13.6.9-blueviolet)](https://www.apple.com/macos/)
![STATUS](https://img.shields.io/badge/STABLE-v0.3-blueviolet.svg)

# Introduction
After crying and searching though Internet no one have try this freeking nugget run macOS, I think its will be a fun experience to try out. This hackintosh configuration is built for Lenovo Ideapad S340-15API (Ryzen). Also this is my first hackintosh project for educational purpose because all my money goes to ~~relearn calculus~~ fund the university campus rebuild, so... yeah we have this

# Disclaimer
Please read entire guide from [Dortania OpenCore Guides](https://dortania.github.io/OpenCore-Install-Guide/), [Noot AMD Hackintosh Guide](https://chefkissinc.github.io/) and this ReadMe before you using this config. I am not responsible for any damage. If you want to improve this repo, please make issue or pull request. Any help would be greatly appreciated.

# Laptop Configuration
#### SMBIOS: MacBookPro16,3
 ### Hardware
| Category      | Component       |
|---------------|-----------------|
| CPU           | AMD Ryzen 3500U |
| GPU           | Radeon™ Vega 8  |
| NVME          | WD SN520        |
| Wireless Card | BCM94352Z       |

 ### BIOS Configuration
AMCN25WW(v1.08)

Configuration 
| Settings                       | Value     |
|--------------------------------|-----------|
| Integrated Graphics Controller | forces    |

Security
| Settings                                    | Value     |
|---------------------------------------------|-----------|
| Secure Boot                                 | disabled  |
| AMD Platform Security Processor             | enabled   |

Boot
| Settings          | Value           |
|-------------------|-----------------|
| Boot Mode         | UEFI            |
| Fast Boot         | disabled        |
| USB Boot          | enabled         |

### Advanced BIOS Menu

Not recommend, but if u want to tweek more. Fully power off the laptop. Enter the BIOS by pressing F2 at boot. Power off the laptop again. Quickly enter the following code:
```
     F1 → 1 → Q → A → Z
     
     F2 → 2 → W → S → X
     
     F3 → 3 → E → D → C
     
     F4 → 4 → R → F → V
     
     F5 → 5 → T → G → B
     
     F6 → 6 → Y → H → N
```

### ACPI
Advanced Configuration and Power Interface (ACPI) is an open standard that operating systems can use to discover and configure computer hardware components, perform power management (e.g. putting unused hardware components to sleep), auto configuration (e.g. Plug and Play and hot swapping), and status monitoring.

I recommend you should remake this on your own with [SSDTTime](https://github.com/corpnewt/SSDTTime)
The full guide do dump this file can go though [here](https://github.com/iamthaoly/amd-laptop-hackintosh) or [Getting Started With ACPI and Troubleshooting](https://dortania.github.io/Getting-Started-With-ACPI/)


### Kext
I'm gonna update this back soon

# Credits
This build wouldn't happen without these amazing people/community:
- [RieGan](https://github.com/RieGan) and [Bingus Studios](https://youtube.com/@BringusStudios?si=9GDnu6Q0GCMPNQc1) inspired me to make this project possible
- [Acidanthera](https://github.com/acidanthera) for OpenCorePkg, Lilu, etc...
- [corpnewt](https://github.com/corpnewt) for all powertools
- [Noot](https://chefkissinc.github.io/) for NootedRed, RadeonSensor and AMD Hackintosh Guide
- [IamThaoLy](https://github.com/iamthaoly) for the general ACPI debug AMD Hackintosh guide
- [Tạp Hoá PC](https://shopee.vn/lvthu93?categoryId=100644&entryPoint=ShopByPDP&itemId=12203249664&upstream=search) for BCM94352Z, with out this the project can't go smooth
- [Dortania](https://github.com/dortania) for OpenCore Guide
- [OpenCore project](https://github.com/OpenCorePkg) for the bootloader
- [EliteMacX86 Forum](https://elitemacx86.com/feeds/)

# Issues
- Chromium application run unstable like Brave, Discord (Gif open),...
- Trackpad
- iService like icloud, imess,...

# Update, recommendation
WIP
