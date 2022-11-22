# BIOS

> Stands for *Basic Input Output System*


- Stored in **EPROM** (Electronically Programmable Read Only Memory)
- Used by the CPU immediately after computer startup
- Responsible for loading and verifying integrity of peripherals, device drivers and other firmware, as well as loading the OS into memory.

**BIOS Boot Process**
1) Execute Core Root of Trust
	- A specific block of firmware is executed.
	- It verifies the integrity of other firmware.
	- Also known as the **BIOS Boot Block**.
2) Initialize & Test Low Level Hardware
	- The BIOS initializes and tests vital hardware components.
3) Load & Execute additional Firmware
	- The BIOS runs additional firmware.
	- This firmware could be for the GPU, Sound Card, Network Adapter, etc.
	- These components are not vital, but greatly enhance the functionality of the system.
4) Select Boot Device
	- The BIOS Locates a drive containing the OS and bootloader.
	- It executes the bootloader to prepare for the next step.
5) Load OS
	- The bootloader loads and initializes the Kernel.
	- Once the Kernel is fully active, the BIOS's role is over.
	- The Operating System takes full control.


*The BIOS also loads SMI (System Management Interrupt) handlers and  initializes Advanced Configuration and Power Interfaces for power and thermal management.*