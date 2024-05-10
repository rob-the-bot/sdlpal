# sdlpal
Build file for cross-compiling sdlpal for Linux aarch64.

## Build

- For the official instruction from [SDLPAL](https://github.com/sdlpal/sdlpal?tab=readme-ov-file#building-the-game)
- Download build toolchain from [knulli-cfw](https://github.com/knulli-cfw/toolchains/releases/tag/rg35xx-plush-sdk-20240421)
- Move the [`Makefile`](Makefile) in this repo to the `unix` folder. Note that this Makefile assumes the build toolchain is in $HOME.
- `make`

Tested for build a native aarch64 executable for ANBERNIC RG35XX Plus running muOS (muOS-RG35XX-2405-BEANS.img).

## Runtime

- `cd` to the directory which contains the data files
- set the library path with `export LD_LIBRARY_PATH=/usr/lib64/gl4es`
