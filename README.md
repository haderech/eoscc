# SiO<sub>4</sub>.CDT (Contract Development Toolkit)
## Version : 1.6.3

SIO4.CDT is a toolchain for WebAssembly (WASM) and set of tools to facilitate contract writing for the EOSIO platform.  In addition to being a general purpose WebAssembly toolchain, [EOSIO](https://github.com/eosio/eos) specific optimizations are available to support building EOSIO smart contracts.  This new toolchain is built around [Clang 7](https://github.com/eosio/llvm), which means that SIO4.CDT has the most currently available optimizations and analyses from LLVM, but as the WASM target is still considered experimental, some optimizations are not available or incomplete.

## Installation

SIO4.CDT currently supports Linux x86_64 Debian packages and Mac OS X brew.

**If you have previously installed SIO4.CDT (or EOSIO.CDT), please run the `uninstall` script (it is in the directory where you cloned SIO4.CDT) before downloading and using the binary releases.**

#### Debian Package Install
```sh
$ wget https://github.com/3osio/sio4.cdt/releases/download/v1.6.3-pre.1/sio4.cdt_1.6.3-pre.1-ubuntu-18.04_amd64.deb
$ sudo apt install ./sio4.cdt_1.6.3-pre.1-ubuntu-18.04_amd64.deb
```
#### Debian Package Uninstall
```sh
$ sudo apt remove sio4.cdt
```

#### Mac OS X Brew Install
```sh
$ brew tap 3osio/sio4.cdt
$ brew install sio4.cdt
```
#### Mac OS X Brew Uninstall
```sh
$ brew remove sio4.cdt
```

### Guided Installation (Building from Scratch)
```sh
$ git clone --recursive https://github.com/3osio/sio4.cdt
$ cd sio4.cdt
$ ./build.sh
$ sudo ./install.sh
```

### Installed Tools
---
* eosio-cpp
* eosio-cc
* eosio-ld
* eosio-init
* eosio-abidiff
* eosio-wasm2wast
* eosio-wast2wasm
* eosio-ranlib
* eosio-ar
* eosio-objdump
* eosio-readelf
