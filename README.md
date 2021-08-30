# unattendInstall
Placing this file in a normal windows installation usb will make the installer run with some defaulted values,
*NOTE the usb must be in UEFI mode it will not work in Legacy.

**NOTE THE ENTIRETY OF DISK 0 WILL BE COMPLETELY ERASED, MAKE SURE YOU BACKUP ANY DATA YOU DO NOT WANT TO LOSE**

Default values:
  Language: en-US //American English
  Install Setup:
    Erase entirety of Disk 0 (99% of the time this is the internal HDD or SSD and is usually where windows is usually installed by default) 
    -> create and modify partition labeled WinRE (Recovery) (not seen) 500MB
    -> create and modify partition labeled System booter (EFI windows boot manager) (not seen) 100MB
    -> create and modify partition with format MSR (not seen) 16MB
    -> create and modify partition labeled Windows and has drive letter C (where windows is actually installed) Whatever is left in GB 
  
  Each folder specifies which version of windows gets installed
