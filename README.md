### RISC-V

I'm learning RISC-V and adding resources in here. 
RISC-V - Reduced Instruction Set 

Qemu is being used as an emulator for RISC-V aarch.
Given the device with SMP of 9 simultaneous processors.
File `ubuntu-24.04.1-preinstalled-server-riscv64.img.xz` to be extracted 
for the image of preinstalled server for qemu. Following is the command 
Extend the filesystem for further storage purpose give upto 20GB.
```
unxz < ubuntu-24.04.1-preinstalled-server-riscv64.img.xz > ubunturv.img

## Resizing the image to specified needs

sudo qemu-img resize ubunturv.img +20G

```

Following this use `run_script.sh` for booting up the RISC-V system in qemu.
Initial Login & Password is ubuntu which is to be changed as you login to the 
prompt.
