# OS (Operating System)

A lightweight and customizable operating system project for cloud ENV from Scratch[Kernel+rootfs+busybox_userspace].

## Overview

This repository contains the source code for a custom operating system. The project aims to provide a minimal, efficient, and customizable OS environment.

## Getting Started

### Prerequisites

- GCC compiler
- Make
- NASM (Netwide Assembler)
- QEMU (for testing in virtual environment)

### Building

To build the project:

```bash
# Install Dependancies
./bin/system-setup
# Create Cloud Image
./bin/build-release daily
```

This command will compile the source code and generate the necessary output files.

### Running

After building, you can run the OS in a virtual environment using QEMU:

```bash
qemu-system-x86_64 -kernel build/kernel.bin
```

## Download
[![Download Pooya OS](https://img.shields.io/github/v/release/MohammadPooyaMalek/OS?include_prereleases&label=Download%20Latest%20Build&style=for-the-badge)](https://github.com/MohammadPooyaMalek/OS/releases/download/latest-build/Pooya-latest-x86_64.img)

[View all releases](https://github.com/MohammadPooyaMalek/OS/releases)

## Project Structure

```
.
├── bin/              # Build scripts and utilities
├── src/              # Source code
│   ├── kernel/       # Kernel source files
│   ├── drivers/      # Hardware drivers
│   ├── fs/           # File system implementation
│   └── lib/          # Common libraries and utilities
├── include/          # Header files
└── tests/            # Test cases
```

## Features

- Minimal bootloader
- Basic kernel functionality
- Memory management
- Process scheduling
- Device drivers
- File system support

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the GNU License - see the LICENSE file for details.

## Acknowledgements

- Thanks to all contributors who have helped develop this project
- Inspired by various open-source OS projects and educational resources