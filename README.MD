# BSFORK Kernel 3.18 for LeEco Le Max 2 (X820/821/829)

This is a fork of BS Kernel 7.3 with patches and backports for Le Max 2.

Works for Android 10 and 11. Android 9 not tested but they has to work also

## To build

- Have a aarch64 linux kernel toolchain (From GCC 4.9 to GCC 10, clang seems to not work)

Ex: https://github.com/kprkpr/android_prebuilts_gcc_linux-x86_aarch64_gcc-10.1-nolibc


    $ export ARCH=arm64 && SUBARCH=arm64
    $ export CROSS_COMPILE=/path/to/aarch64-linux-android-10.1/bin/aarch64-linux-
    $ make O=out mrproper
    $ make O=out lineage_x2_defconfig
    $ make O=out -j8
