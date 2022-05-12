## Straton Clang

This toolchain targets the ARM, AArch64, and x86 architectures.
It is built with LTO to reduce compile time.
Polly, LLVM's polyhedral loop optimizer, is also included for users who want to experiment with additional optimization.
Build will always be based on the stable release of LLVM Project.

## Host compatibility

This toolchain is built on Ubuntu 22.04, which uses glibc 2.34. Compatibility with older distributions cannot be guaranteed.
