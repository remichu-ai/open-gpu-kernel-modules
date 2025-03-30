# NVIDIA driver 570.133.07 with P2P for 4090

This allows using P2P on 4090 GPUs with the 570.124.04 driver version.
See https://github.com/tinygrad/open-gpu-kernel-modules for more info.

## How to Build

1) Install https://www.nvidia.com/en-us/drivers/details/242273/
2) Run `./install.sh`
3) Reboot

-------------
1) ensure iommu is disabled in bios
2) install https://www.nvidia.com/en-us/drivers/details/242273/ 
3) clone https://github.com/aikitoria/open-gpu-kernel-modules/tree/570.133.07-p2p
4) run install.sh in there
5) reboot
6) run a program that uses nccl with NCCL_P2P_LEVEL=SYS
