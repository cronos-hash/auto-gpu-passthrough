# auto gpu passthrough 

## What this program does?
This program will perform a automatic gpu passthrough on arch systems

## How does it work? auto-mode
It works by utilising two scripts. The first scripts (auto mode) will add a script as a hook within the kernel configuration (mkinitcpio.conf) so that any additional GPU's on the system will be used. THis excludes the current GPU that is being used for the main system.

## How does it work? manual-mode
The second script (manual mode) adds a script as a hook within the kernel configuration. However, it displays all GPU devices on the system, and allows the user to select that GPU for passthrough.

## How does enabling iommu work automatically?
The program comes with two seperate config files for grub, one for intel CPUs, and the other for AMD CPU's. THe program will autodetect the type of vendor used, then change the configuration depending on this vendor.

## What are these other options?
The other options are specific towards the machine i use, i put a secret password on this installer and its totally impossible to hack. NOTE: my configurations may break your system proceed with caution
