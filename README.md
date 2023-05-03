# GIGABYTE GA-Z790-UD

OpenCore EFI for Gigabyte Z790 UD DDR5


```text
                    'c.          iMac-Pro 
                 ,xNMM.          ------------------------ 
               .OMMMMo           OS: macOS 13.3.1 22E261 x86_64
               OMMM0,            Host: Hackintosh (SMBIOS: iMacPro1,1) 
     .;loddo:' loolloddol;.      Kernel: 22.4.0 
   cKMMMMMMMMMMNWMMMMMMMMMM0:    Uptime: 19 hours, 53 mins
 .KMMMMMMMMMMMMMMMMMMMMMMMWd.    Packages: 101 (brew)
 XMMMMMMMMMMMMMMMMMMMMMMMX.      Shell: bash 5.2.15 
;MMMMMMMMMMMMMMMMMMMMMMMM:       Resolution: 2560x1440@2x 
:MMMMMMMMMMMMMMMMMMMMMMMM:       DE: Aqua 
.MMMMMMMMMMMMMMMMMMMMMMMMX.      WM: Quartz Compositor 
 kMMMMMMMMMMMMMMMMMMMMMMMMWd.    WM Theme: Blue (Dark) 
 .XMMMMMMMMMMMMMMMMMMMMMMMMMMk   Terminal: Apple_Terminal 
  .XMMMMMMMMMMMMMMMMMMMMMMMMK.   Terminal Font: SFMono-Regular 
    kMMMMMMMMMMMMMMMMMMMMMMd     CPU: 13th Gen Intel i9-13900 
     ;KMMMMMMMWXXWMMMMMMMk.      GPU: AMD Radeon RX 6900 XT 
       .cooc,.    .,coo:.        Memory: 13247MiB / 65536MiB
```

### OpenCore 
* **Version:** 0.9.1

### Hardware

* **MOBO:** Gigabyte GA-Z790-UD
* **RAM:** Kingbank DDR5-6000 64GB (32*2GB)
* **CPU:** 13th Gen Intel i9-13900
* **GPU:** AMD Radeon RX 6900 XT
* **WIFI/BT:** BCM934602CS
* **SSD:** WD_BLACK SN850X 2000GB


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

### macOS Support
| Version   | macOS | Download |
| --------: | :---- | :------- |
| 13.2.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |
| 13.3.1 | Ventura | [Mac App Store](https://apps.apple.com/us/app/macos-ventura/id1638787999?mt=12) |


### Thanks

[@rursache](https://github.com/rursache/Hackintosh-13900k-Z690-AORUS-ELITE-AX-DDR5-AMD-6900XT)
