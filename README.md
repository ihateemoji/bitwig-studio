# Bitwig Studio XBPS Package

This repository contains files for packaging Bitwig Studio for Void Linux using the XBPS package manager.

## Files

1. `template`: XBPS template file for Bitwig Studio

## Template File

The `template` file is an XBPS template for Bitwig Studio.

- Architecture: x86_64 only
- Build style: precompiled binaries

The template file handles the installation of precompiled binaries and sets up the necessary package metadata.

### Installation

To install the Bitwig Studio package:

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
6. Enjoy!

* You can also install using `vpsm` instead of (3) and (4):
   ```sh
   vpsm install bitwig-studio
   ```

## Contributing

If you want to contribute to this package, please make sure to test your changes thoroughly before submitting a pull request.

## Issues

If you encounter any issues with the package or the update script, please open an issue in this repository.
