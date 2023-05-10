# GIGABYTE GA-Z790-UD

OpenCore EFI for Gigabyte Z790 UD DDR5


```text
                    'c.          MacPro7,1
                 ,xNMM.          ----------------- 
               .OMMMMo           OS: macOS 13.3.1 22E261 x86_64 
               OMMM0,            Host: Hackintosh (SMBIOS: MacPro7,1) 
     .;loddo:' loolloddol;.      Kernel: 22.4.0 
   cKMMMMMMMMMMNWMMMMMMMMMM0:    Uptime: 18 mins 
 .KMMMMMMMMMMMMMMMMMMMMMMMWd.    Packages: 205 (brew) 
 XMMMMMMMMMMMMMMMMMMMMMMMX.      Shell: zsh 5.9 
;MMMMMMMMMMMMMMMMMMMMMMMM:       Resolution: 1920x1080@2x 
:MMMMMMMMMMMMMMMMMMMMMMMM:       DE: Aqua 
.MMMMMMMMMMMMMMMMMMMMMMMMX.      WM: Quartz Compositor 
 kMMMMMMMMMMMMMMMMMMMMMMMMWd.    WM Theme: Blue (Light) 
 .XMMMMMMMMMMMMMMMMMMMMMMMMMMk   Terminal: Apple_Terminal 
  .XMMMMMMMMMMMMMMMMMMMMMMMMK.   Terminal Font: SFMono-Regular 
    kMMMMMMMMMMMMMMMMMMMMMMd     CPU: 13th Gen Intel i9-13900K 
     ;KMMMMMMMWXXWMMMMMMMk.      GPU: AMD Radeon RX 6800 XT 
       .cooc,.    .,coo:.        Memory: 14256MiB / 32768MiB 

                                                         
                                                         
```

### OpenCore 
* **Version:** 0.9.2

### Hardware

* **MOBO:** Gigabyte GA-Z790-UD
* **RAM:** Kingbank DDR5-6400 64GB (16*2GB)
* **CPU:** 13th Gen Intel i9-13900K
* **GPU:** AMD Radeon RX 6800 XT
* **WIFI/BT:** BCM946360CS
* **SSD:** TOPMORE ARIES 2TB


### BIOS [F6c](https://download.gigabyte.com/FileList/BIOS/mb_bios_z790-ud_f6c.zip)
Use Q-Flash Update the latest BIOS and Load Optimized Defaults
* Settings
	* Tweaker
		*  Extreme Memory Profile (X.M.P.) → **XMP1** (Enable DDR5 6000MHz)
	* Boot
		*  Fast Boot → **Disabled**
		*  CSM Support → **Disabled**
        *  Secure Boot → **Disabled**
	* Settings → Platform Power
		* ErP → **Enabled**
	* Settings → IO Ports
		* Initial Display Output → **PCIe 1 Slot**
		* Internal Graphics → **Disabled**	
		* Above 4G Decoding → **Enabled**
		* Re-Size BAR Support → **Enabled** 
		* IOAPIC 24-119 Entries → **Enabled**
	* Settings → Miscellaneous
		* VT-d → **Enabled**


### Not working
* wakeup / sleep issue is fixed in bios F6c
* second sleep crash issue has been fixed by add **npci=0x2000** in **boot-args**
* keyboard wake issue has been fixed by **Add Wake Type Property**

### macOS Support
| Version   | macOS | Download |
| --------: | :---- | :------- |
| 13.2.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |


### Thanks

[@rursache](https://github.com/rursache/Hackintosh-13900k-Z690-AORUS-ELITE-AX-DDR5-AMD-6900XT)
