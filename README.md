# EOSCC
## Version : 1.6.3

The EOSIO Compiler Collection (EOSCC) is a toolchain for WebAssembly (WASM) and set of tools to facilitate contract writing for the EOSIO platform.  In addition to being a general purpose WebAssembly toolchain, [EOSIO](https://github.com/eosio/eos) specific optimizations are available to support building EOSIO smart contracts.  This new toolchain is built around [Clang 7](https://github.com/eosio/llvm), which means that EOSCC has the most currently available optimizations and analyses from LLVM, but as the WASM target is still considered experimental, some optimizations are not available or incomplete.

### Attention
EOSIO.CDT Version 1.3.x introduced quite a few breaking changes.  To have binary releases we needed to remove the concept of a core symbol from EOSIO.CDT. This meant drastic changes to symbol, asset and other types/functions that were connected to them. Since these changes would be disruptive, we decided to add as many disruptive changes needed for future contract writing, so that disruption should only occur once. Please read the **_Differences between Version 1.2.x and Version 1.3.x_** section of this readme.

### Binary Releases
EOSCC currently supports Linux x86_64 Debian packages and Mac OS X brew.

**If you have previously installed EOSCC (or EOSIO.CDT), please run the `uninstall` script (it is in the directory where you cloned EOSCC) before downloading and using the binary releases.**

#### Debian Package Install
```sh
$ wget https://github.com/b1ockchain/eoscc/releases/download/v1.6.3/eoscc_1.6.3-1-ubuntu-18.04_amd64.deb
$ sudo apt install ./eoscc_1.6.3-1-ubuntu-18.04_amd64.deb
```
#### Debian Package Uninstall
```sh
$ sudo apt remove eoscc
```

#### Mac OS X Brew Install
```sh
$ brew tap b1ockchain/eoscc
$ brew install eoscc
```
#### Mac OS X Brew Uninstall
```sh
$ brew remove eoscc
```

### Guided Installation (Building from Scratch)
```sh
$ git clone --recursive https://github.com/b1ockchain/eoscc
$ cd eoscc
$ ./build.sh
$ sudo ./install.sh
```

### Installed Tools
---
* eosc++
* eoscc
* eosld
* eosranlib
* eosar

## Contributing

[Contributing Guide](./CONTRIBUTING.md)

[Code of Conduct](./CONTRIBUTING.md#conduct)

## License

[MIT](./LICENSE)

## Important

See [LICENSE](./LICENSE) for copyright and license terms.

All repositories and other materials are provided subject to the terms of this [IMPORTANT](./IMPORTANT) notice and you must familiarize yourself with its terms.  The notice contains important information, limitations and restrictions relating to our software, publications, trademarks, third-party resources, and forward-looking statements.  By accessing any of our repositories and other materials, you accept and agree to the terms of the notice.
