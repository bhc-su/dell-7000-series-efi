# dell-7000-series-efi
Hackintosh EFI for Dell 7000 series laptops     --opencore


   If you have any questions, you can ask in the communication group

   Communication Group（qq）：112526282


After entering the system, run /efi/OC/ComboJack Fix/ComboJack_Installer/install.sh in the terminal


BIOS settings：


Most of these options may not be present in your firmware, we recommend matching up as closely as possible but don't be too concerned if many of these options are not available in your BIOS

Disable：


Fast Boot

Secure Boot

Serial/COM Port

Parallel Port

VT-d (can be enabled if you set DisableIoMapper to YES)

Compatibility Support Module (CSM) (Must be off in most cases, GPU errors/stalls like gIO are common 
when this option is enabled)

Thunderbolt(For initial install, as Thunderbolt can cause issues if not setup correctly)

Intel SGX

Intel Platform Trust

CFG Lock (MSR 0xE2 write protection)(This must be off, if you can't find the option then enable AppleXcpmCfgLock under Kernel -> Quirks. Your hack will not boot with CFG-Lock enabled)


Enable：

VT-x

Above 4G Decoding

Hyper-Threading

Execute Disable Bit

EHCI/XHCI Hand-off

OS type: Windows 8.1/10 UEFI Mode (some motherboards may require "Other OS" instead)

DVMT Pre-Allocated(iGPU Memory): 64MB or higher

SATA Mode: AHCI
