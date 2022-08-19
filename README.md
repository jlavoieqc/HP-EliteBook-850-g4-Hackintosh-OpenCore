# HP EliteBook 850 G4 Hackintosh OpenCore
-- Running Monterey 12.5.1 and might be compatible with others versions

Working
-
- Wifi
- Bluetooth
- Audio
- Trackpad
- Webcam
- Microphone

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
- Boot opencore
- Select Your Drive That contain mac recovery that you can download with macrecovery (https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html#downloading-macos) (WARNING:If you dont see your drive, press space)
- Go to disk utilities and format your partition that you want macOS in afps
- Go to reinstall (Your macOS version)
- Agree terms
- Select your drive and let it install
- After it will reboot and you will have to boot your usb drive and you might see install macOS (Dont forget to press space bar if you dont see it)

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
