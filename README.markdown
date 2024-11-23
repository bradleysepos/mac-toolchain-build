mac-toolchain-build ![Build](https://github.com/bradleysepos/mac-toolchain-build/workflows/Build/badge.svg)
===================

mac-toolchain-build is a Bash script for downloading and building common macOS toolchain components.


Requirements
------------

- macOS/Darwin
- Xcode and Command Line Tools for Xcode


Installation
------------

Copy `mac-toolchain-build` to a directory in your `PATH` such as `/usr/local/bin` and make it executable.


Usage
-----

The basic syntax is:

```
mac-toolchain-build [-f | --force] [-j # | --jobs #] [install-dir]
```

Where:

- `-f, --force` force installation even if adequate versions of tools are installed
- `-j, --jobs` number of concurrent build jobs to run, default: 0 (automatic)

Default installation directory is `/usr/local`.

Following successful building of the toolchain components, the script provides instructions for adding the output binaries directory to your `PATH`.

Full usage:

```
mac-toolchain-build --help
```


Components
----------

- autoconf
- automake
- cmake
- libtool
- m4
- meson
- nasm
- ninja
- openssl
- pkg-config

Display components list with version information:

```
mac-toolchain-build --list
```


License
-------

Copyright 2024 Bradley Sepos
Released under the MIT License. See [LICENSE](LICENSE) for details.
