## Straton Clang

This toolchain targets the ARM, AArch64, and x86 architectures.
It is built with Clang + LTO + LLD.
Polly, LLVM's polyhedral loop optimizer, is also included for users who want to experiment with additional optimization.
Build will always be based on the stable release of LLVM Project.

## Host compatibility

This toolchain is built on Ubuntu 22.04, which uses glibc 2.35. Compatibility with older distributions cannot be guaranteed.

## Other notes

* `CLANG_TRIPLE` does not need to be set because we don't use AOSP binutils.
* `LD_LIBRARY_PATH` does not need to be set because we set library load paths in the toolchain.
* No separate GCC/binutils toolchains are necessary; all tools are bundled.
