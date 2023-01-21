# OS Boot Up Process

Date: October 5, 2022 3:43 PM
Status: Done

- **Power On**
    
    Power is goes to PSU which than gives power to different components.
    
- CPU initialise itself:
    
    It looks for BIOS (Basic input output system) stored in BIOS chip in Modern CPU, **UEFI (Unified Extensible Firmware Interface)**
    
- **BIOS** or **UEFI** tests and initialise system hardware
    
    BIOS loads configuration settings. If something is not appropriate like RAM error is thrown and boot process is stopped.
    
    This test is known as **POST (Power On Self Test)**
    
- BIOS/UEFI hand off responsibility to OS Bootloader
    
    **Bootloader is a program which is used to start the OS.**
    
    1. Loads Kernel
    2. Loads UserSpace
    3. Loads other important process required by OS
    
    In BIOS system Bootloader is stored in **MBR(master boot record)**
    
    In UEFI systems Bootloader is stored in **EFI Partitions** 
    
    Example: Windows Boot Manager, Grub, boot.efi