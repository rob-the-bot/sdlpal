# sdlpal
Build file for cross-compiling sdlpal for Linux aarch64.

For ANBERNIC RG35XX Plus running muOS (muOS-RG35XX-2405-BEANS.img), native aarch64 executable can be built using [`Makefile`](Makefile),
with build toolchain from [knulli-cfw](https://github.com/knulli-cfw/toolchains/releases/tag/rg35xx-plush-sdk-20240421).

During runtime (of the executable file `sdlpal`),
it's important to `cd` to the directory which contains the data files,
and set the library path with `export LD_LIBRARY_PATH=/usr/lib64/gl4es`.
