# Bitwig Studio 5 XBPS Package

This repository contains files for packaging Bitwig Studio 5 for Void Linux using the XBPS package manager.

## Files

1. `template`: XBPS template file for Bitwig Studio 5

## Template File

The `template` file is an XBPS template for Bitwig Studio 5.

- Architecture: x86_64 only
- Build style: precompiled binaries

### Installation

To install the Bitwig Studio 5 package:

1. Clone the Void Packages repository:
   ```sh
   git clone https://github.com/ihateemoji/bitwig-studio.git
   ```
2. Copy the directory to the `srcpkgs/bitwig-studio` directory in your Void Packages repository:
   ```sh
   cp -rf bitwig-studio /path/to/void-packages/srcpkgs/
   ```
3. Build the package:
   ```sh
   ./xbps-src pkg bitwig-studio
   ```
4. Install the package:
   ```sh
   sudo xbps-install --repository=hostdir/binpkgs bitwig-studio
   ```
5. Run Bitwig Studio:
   ```sh
   bitwig-studio
   ```
