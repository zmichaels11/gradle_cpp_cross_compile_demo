# Gradle C++ Cross-Compile Demo
Minimal project required to demonstrate Cross-Compiling to Windows and ARM Linux from x86 Linux

# Requirements
* g++-arm-linux-gnueabi
* g++-aarch64-linux-gnu
* g++-mingw-w64-x86_64
* g++-mingw-w64-i686
* g++-multilib

# Optional
* qemu
* wine

# Testing on linux
All executables are compiled with -static to reduce dependencies.

## Run armv7 linux executable on x86 linux
``` bash
$ qemu-arm the_executable
```

## Run arm64 linux executable on x86 linux
``` bash
$ qemu-aarch64 the_executable
```

## Run windows executable on x86 linux
``` bash
$ wine the_executable
```
