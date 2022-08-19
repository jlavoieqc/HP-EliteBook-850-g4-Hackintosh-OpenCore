# HP EliteBook 850 G4 Hackintosh OpenCore
-- Running Monterey 12.5.1 and might be compatible with others versions

Working
-
- Wifi
- Bluetooth
- Audio
- Trackpad

Not Working
-
- Nothing that I know, I just installed it and wanted to share it

Not Tested
-
- Hdmi

Installation
-
- Generate smbios with GenSMBIOS
- I used MacBookPro14,1

# BIOS Settings
Disable
-
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- VT-d
- Compatibility Support Module (CSM) (Must be off in most cases, GPU errors/stalls like gIO are common when this option is enabled)
- Thunderbolt(For initial install, as Thunderbolt can cause issues if not setup correctly)
- Intel SGX
- Intel Platform Trust
- CFG Lock
Enable
-
- VT-x
- Above 4G Decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- DVMT Pre-Allocated(iGPU Memory): 64MB or higher
- SATA Mode: AHCI
