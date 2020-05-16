# ROXE.CDT (Contract Development Toolkit)
## Version : 1.6.3

ROXE.CDT is a toolchain for WebAssembly (WASM) and set of tools to facilitate contract writing for the ROXE platform.  In addition to being a general purpose WebAssembly toolchain, [ROXE](https://github.com/roxe/eos) specific optimizations are available to support building ROXE smart contracts.  This new toolchain is built around [Clang 7](https://github.com/roxe/llvm), which means that ROXE.CDT has the most currently available optimizations and analyses from LLVM, but as the WASM target is still considered experimental, some optimizations are not available or incomplete.

### Attention
ROXE.CDT Version 1.3.x introduced quite a few breaking changes.  To have binary releases we needed to remove the concept of a core symbol from ROXE.CDT. This meant drastic changes to symbol, asset and other types/functions that were connected to them. Since these changes would be disruptive, we decided to add as many disruptive changes needed for future contract writing, so that disruption should only occur once. Please read the **_Differences between Version 1.2.x and Version 1.3.x_** section of this readme.

### Binary Releases
ROXE.CDT currently supports Mac OS X brew, Linux x86_64 Debian packages, and Linux x86_64 RPM packages.

**If you have previously installed ROXE.CDT, please run the `uninstall` script (it is in the directory where you cloned ROXE.CDT) before downloading and using the binary releases.**

#### Mac OS X Brew Install
```sh
$ brew tap roxe/roxe.cdt
$ brew install roxe.cdt
```

#### Mac OS X Brew Uninstall
```sh
$ brew remove roxe.cdt
```

#### Debian Package Install
```sh
$ wget https://github.com/roxe/roxe.cdt/releases/download/v1.6.3/roxe.cdt_1.6.3-1-ubuntu-18.04_amd64.deb
$ sudo apt install ./roxe.cdt_1.6.3-1-ubuntu-18.04_amd64.deb
```

#### Debian Package Uninstall
```sh
$ sudo apt remove roxe.cdt
```

#### RPM Package Install
```sh
$ wget https://github.com/roxe/roxe.cdt/releases/download/v1.6.3/roxe.cdt-1.6.3-1.el7.x86_64.rpm
$ sudo yum install ./roxe.cdt-1.6.3-1.el7.x86_64.rpm
```

#### RPM Package Uninstall
```sh
$ sudo yum remove roxe.cdt
```

### Guided Installation (Building from Scratch)
```sh
$ git clone --recursive https://github.com/roxe/roxe.cdt
$ cd roxe.cdt
$ ./build.sh
$ sudo ./install.sh
```

### Installed Tools
---
* roxe-cpp
* roxe-cc
* roxe-ld
* roxe-init
* roxe-abidiff
* roxe-wasm2wast
* roxe-wast2wasm
* roxe-ranlib
* roxe-ar
* roxe-objdump
* roxe-readelf

## Contributing

[Contributing Guide](./CONTRIBUTING.md)

[Code of Conduct](./CONTRIBUTING.md#conduct)

## License

[MIT](./LICENSE)

## Important

See [LICENSE](./LICENSE) for copyright and license terms.

All repositories and other materials are provided subject to the terms of this [IMPORTANT](./IMPORTANT.md) notice and you must familiarize yourself with its terms.  The notice contains important information, limitations and restrictions relating to our software, publications, trademarks, third-party resources, and forward-looking statements.  By accessing any of our repositories and other materials, you accept and agree to the terms of the notice.
