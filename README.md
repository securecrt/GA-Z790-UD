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


### BIOS [F5](https://download.gigabyte.cn/FileList/BIOS/mb_bios_z790-ud_f5.zip?v=e5544dab810c13aa9a1e302ef062f745)
Use Q-Flash Update the latest BIOS and Load Optimized Defaults
* Settings
	* Tweaker
		*  Extreme Memory Profile (X.M.P.) → **XMP1** (Enable DDR5 6000MHz)
	* Boot
		*  Fast Boot → **Disabled**
		*  CSM Support → **Disabled**
	* Settings → Platform Power
		* ErP → **Enabled**
	* Settings → IO Ports
		* Initial Display Output → **PCIe 1 Slot**
		* Internal Graphics → **Disabled**	
		* Above 4G Decoding → **Enabled**
		* Re-Size BAR Support → **Enabled** 
		* IOAPIC 24-119 Entries → **Disabled** (fixed Wakeup issue)
	* Settings → Miscellaneous
		* VT-d → **Enabled**


### Not working
* Can't wakeup from auto sleep. 
* But if manually press the sleep button, it can wakeup normally. The issue is also reproduced in win11.
* It should be the BIOS issue. 
* currently disabled IOAPIC 24-119 Entries can fix this issue.
* some links related to the wakeup / sleep issues  
https://forums.guru3d.com/threads/windows-line-based-vs-message-signaled-based-interrupts-msi-tool.378044/page-90
https://www.reddit.com/r/Fedora/comments/v8o6l8/b660m_mobo_not_able_to_wakeup_from_sleep/

### macOS Support
| Version   | macOS | Download |
| --------: | :---- | :------- |
| 13.2.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |


### Thanks

[@rursache](https://github.com/rursache/Hackintosh-13900k-Z690-AORUS-ELITE-AX-DDR5-AMD-6900XT)