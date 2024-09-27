# OrinFlash
This is a fork from JetsonHacks to Flash JetPack5.1.3 to a Jetson Orin Nano board.

## NOTES: 
- The modified scripts were only tested on a [Jetson Orin Nano Developer Kit \[SUB\] 8GB](https://category.yahboom.net/products/jetson-orin-nano) for installing the Jetson Linux 36.3.0 on an NVMe SSD. The original scripts may work on other versions of Jetson Linux and different Jetson modules with various storage media.  
- For more instructions and details, please check JetsonHacks original [repo](https://github.com/jetsonhacks/bootFromExternalStorage).
- Need a video guide? Check this out: [https://youtu.be/q4fGac-nrTI?si=SsojJljABo3sRYVr](https://youtu.be/q4fGac-nrTI?si=SsojJljABo3sRYVr). 

## Quick Start
**NOTE: execute ALL the following commands on the host machine**
**Host machine requirements:**
- x86_64 CPU
- Ubuntu 20.04 or Ubuntu 22.04

1. Clone this repo
   ```bash
   cd ~
   git clone git@github.com:linzhangUCA/OrinFlash.git
   cd OrinFlash
   ```
2. Download files
   ```bash
   ./get_jetson_files.sh
   ```
3. Flash JetPack to the target (Orin Nano board)
Put your Orin to `force_recovery` mode, then remove the jumper
   ```bash
   ./flash_jetson_external_storage.sh
   ```
