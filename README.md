```bash
mkdir output
cd buildroot-2022.02.9
make defconfig BR2_DEFCONFIG=../buildroot-external/configs/idl4k/idl4k_defconfig O=../output
cd ../output
make
```

TODO:

* build cpio, include as initramfs
* try resulting uImage as satip-axe.fw
* add missing tools (iperf3, ntp etc.)
* add package for minisatip
* add axe_fe.ko and axe_dmxts_std.ko to /lib/modules/axe
* add axe device initializaton
