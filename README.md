# GIGABYTE GA-Z790-UD

OpenCore EFI for Gigabyte Z790 UD DDR5


```text
                    'c.          iMac-Pro 
                 ,xNMM.          ------------------------ 
               .OMMMMo           OS: macOS 13.3 22E252 x86_64 
               OMMM0,            Host: Hackintosh (SMBIOS: iMacPro1,1) 
     .;loddo:' loolloddol;.      Kernel: 22.4.0 
   cKMMMMMMMMMMNWMMMMMMMMMM0:    Uptime: 11 mins 
 .KMMMMMMMMMMMMMMMMMMMMMMMWd.    Packages: 93 (brew) 
 XMMMMMMMMMMMMMMMMMMMMMMMX.      Shell: bash 5.2.15 
;MMMMMMMMMMMMMMMMMMMMMMMM:       Resolution: 2560x1440@2x 
:MMMMMMMMMMMMMMMMMMMMMMMM:       DE: Aqua 
.MMMMMMMMMMMMMMMMMMMMMMMMX.      WM: Quartz Compositor 
 kMMMMMMMMMMMMMMMMMMMMMMMMWd.    WM Theme: Blue (Dark) 
 .XMMMMMMMMMMMMMMMMMMMMMMMMMMk   Terminal: Apple_Terminal 
  .XMMMMMMMMMMMMMMMMMMMMMMMMK.   Terminal Font: SFMono-Regular 
    kMMMMMMMMMMMMMMMMMMMMMMd     CPU: 13th Gen Intel i9-13900 
     ;KMMMMMMMWXXWMMMMMMMk.      GPU: AMD Radeon RX 6900 XT 
       .cooc,.    .,coo:.        Memory: 12025MiB / 65536MiB 
```

### OpenCore 
* **Version:** 0.9.0

### Hardware

* **MOBO:** Gigabyte GA-Z790-UD
* **RAM:** Kingbank DDR5-6000 64GB (32*2GB)
* **CPU:** 13th Gen Intel i9-13900
* **GPU:** AMD Radeon RX 6900 XT
* **WIFI/BT:** BCM934602CS
* **SSD:** WD_BLACK SN850X 2000GB


### BIOS Settings [F5](https://download.gigabyte.cn/FileList/BIOS/mb_bios_z790-ud_f5.zip?v=e5544dab810c13aa9a1e302ef062f745)
* Settings
	* BIOS
		*  Fast Boot → **Disabled**
		*  CSM Support → **Disabled**
	* Settings
		* Initial Display Output → **PCIe 1 Slot**
		* Above 4G Decoding → **Enabled**
		* Re-Size BAR Support → **Enabled**
		

### Not working
* Can't read out the fan RPM after wakeup from sleep and the fan became noisy.
* The issue can be reproduced in Win11 also, need to wait the bios update from gigabyte.

### macOS Support
| Version   | macOS | Download |
| --------: | :---- | :------- |
| 13.2.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |


### Thanks

[@rursache](https://github.com/rursache/Hackintosh-13900k-Z690-AORUS-ELITE-AX-DDR5-AMD-6900XT)