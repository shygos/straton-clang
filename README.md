## Straton Clang

This toolchain targets the ARM, AArch64, and x86 architectures built with Clang + LLD.
Polly, LLVM's polyhedral loop optimizer, is also included for users who want to experiment with additional optimization.
Build will always be based on the stable release of LLVM Project.

## Host compatibility

This toolchain is built on Ubuntu 20.04, which uses glibc 2.31. Compatibility with older distributions cannot be guaranteed.

## Other notes

* `CLANG_TRIPLE` does not need to be set because we don't use AOSP binutils.
* `LD_LIBRARY_PATH` does not need to be set because we set library load paths in the toolchain.
* Binary Utilities are not included, so you have to bring your own. The quickest way to get it is by downloading from Ubuntu repository:
```
sudo apt install binutils-aarch64-linux-gnu
sudo apt install binutils-arm-linux-gnueabi
sudo apt install binutils-x86-64-linux-gnu
```
