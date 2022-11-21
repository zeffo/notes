# Introduction

> What is an Operating System?

*An Operating System is a System Software which acts as an interface between the computer hardware, software and the user.*


## Core Functions

- Hardware Management
- Process Management
- File System Management
- Security
- Error Handling
- User Interface

## Modes

1. User Mode
	- Friendly Interface (usually a **GUI**)
	- Operations restricted by privileges given to the user.
2. Kernel Mode
	- Faster and Minimal Interface (usually a **CLI**)
	- Operations not restricted. Any section of memory can be accessed and the processor(s) can execute any given instructions.

## Types (overview)

- Batch
- Multiprogramming
- Multitasking
- Multiprocessing
- Real-time
- Distributed
- Clustered
- Embedded

## Structures

1. Simple
	- Do not have a well-defined structure.
	- Small, simple, limited.
	- No bloat. Trades off functionality for speed.
2. Layered
	- Broken into layers.
	- **Layer 0** is the innermost layer, the Hardware.
	- **Layer N** is the outermost layer, generally the UI.
	- Each Layer can only utilize the functions of layers underneath it.
	- Simplifies debugging in exchange of performance.
3. Micro-Kernel
	- The Kernel only contains vital software resources.
	- All non-essential softwares are implemented as applications.
	- The kernel is portable and platform-agnostic.
	- System performance is degraded due to inter-module communication.
4. Modular
	- The Kernel only has core, vital components.
	- Other modules can be dynamically loaded/unloaded during runtime.
	- Very flexible, and hence considered the best approach for an OS.





