mac-toolchain-build
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
mac-toolchain-build [install-dir]
```

Where:

- `-f, --force` force installation even if adequate versions of tools are installed

Default installation directory is `/usr/local`.

Following successful building of the toolchain components, the script provides instructions for adding the output binaries directory to your `PATH`.

Full usage:

```
mingw-w64-build -h
```

Components
----------

- autoconf
- automake
- cmake
- libtool
- meson
- nasm
- ninja
- pkg-config


License
-------

Copyright 2019 Bradley Sepos  
Released under the MIT License. See [LICENSE](LICENSE) for details.
