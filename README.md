mkdir build
cd buildroot-2022.02.9
make defconfig BR2_DEFCONFIG=../buildroot-external/configs/idl4k/idl4k_defconfig O=../output
cd ../output
make
