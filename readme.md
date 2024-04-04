# Ideapad-S340-15API-Hackintosh
[![OpenCore](https://img.shields.io/badge/OpenCore-v0.9.9-blue)](https://github.com/acidanthera/OpenCorePkg)
[![MacOS-Stable](https://img.shields.io/badge/MacOS-13.6.6-blueviolet)](https://www.apple.com/macos/)
![STATUS](https://img.shields.io/badge/STATUS-BETA0.2-blueviolet.svg)

# The full rebuild its in deverlopment, you can check v0.1 (unstable) in main branch

# Introduction
After crying and searching though Internet no one have try this freeking nugget run macOS, I think its will be a fun experience to try out. This hackintosh configuration is built for Lenovo Ideapad S340-15API (Ryzen). Also this is my first hackintosh project for educational purpose because all my money goes to ~~relearn calculus~~ fund the university campus rebuild, so you know it > ¯\_(ツ)_/¯

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

 ### BIOS Configuration (testing new config soon, something may change in v0.3)
AMCN25WW(v1.08)

Configuration 
| Settings                       | Value     |
|--------------------------------|-----------|
| USB Legacy                     | enabled   |
| Integrated Graphics Controller | forces    |

Security
| Settings                                    | Value     |
|---------------------------------------------|-----------|
| Secure Boot (Already turn off due to Legacy)| disabled  |
| AMD Platform Security Processor             | enabled   |

Boot
| Settings          | Value           |
|-------------------|-----------------|
| Boot Mode         | Legacy Support  |
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
*Shout out to [RieGan](https://github.com/RieGan) for this bios cheat code, if you want to do this on IdeaPad s340 Intel version, check out his [GitHub Project](https://github.com/RieGan/Ideapad-S340-15iwl-Hackintosh)*

### ACPI
Advanced Configuration and Power Interface (ACPI) is an open standard that operating systems can use to discover and configure computer hardware components, perform power management (e.g. putting unused hardware components to sleep), auto configuration (e.g. Plug and Play and hot swapping), and status monitoring.

I recommend you should remake this on your own with [SSDTTime](https://github.com/corpnewt/SSDTTime)
The full guide do dump this file can go though [here](https://github.com/iamthaoly/amd-laptop-hackintosh) or [Getting Started With ACPI and Troubleshooting](https://dortania.github.io/Getting-Started-With-ACPI/)


### Kext
| Name                                                                                                                  | Version   |
|-----------------------------------------------------------------------------------------------------------------------|-----------|
| [AppleALC](https://github.com/acidanthera/AppleALC/releases)                                                          | 1.8.9     |
| [AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip) | 1.0       |
| [BrightnessKeys](https://github.com/acidanthera/BrightnessKeys/releases)                                              | 1.0.3     |
| [Lilu](https://github.com/acidanthera/Lilu)                                                                           | 1.6.7     |
| [RealtekRTL8111 for Ethernet Hub](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)                          | 2.4.2     |
| [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)                                                    | 0.7.2     |
| [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)                                                           | 2.6.8     |
| [NVMeFix](https://github.com/acidanthera/NVMeFix)                                                                     | 1.1.1     |
| [VoodooI2C](https://github.com/VoodooI2C/VoodooI2C)                                                                   | 2.8       |
| [VoodooPS2](https://github.com/acidanthera/VoodooPS2)                                                                 | 2.3.5     |
| [NootedRed](https://github.com/ChefKissInc/NootedRed)                                                                 | 24.04.03  |

# Licence
The Ideapad-S340-15api-Hackintosh project is licensed under the `@hust_lin.all.day for education use, non-profit for life`. See `LICENSE`.

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

# Update, recommendation
WIP
