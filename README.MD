# Termux

This repo contains my various files related to termux.

## R

The package `r-base` in its-pointless repo is now incompatible with the latest version of termux.

So I built it myself. I hope you enjoy it.

Download: https://github.com/kxxt/termux/releases/download/R-4.2.0-1/R-4.2.0-1-termux-arm64.tar.xz

Usage: (You'll need to [setup its-pointless repo](https://github.com/its-pointless/gcc_termux) to install `libgfortran5`)

```shell
wget https://github.com/kxxt/termux/releases/download/R-4.2.0-1/R-4.2.0-1-termux-arm64.tar.xz
tar xJf R-4.2.0-1-termux-arm64.tar.xz $PREFIX
pkg install libgfortran5
# Start R
$PREFIX/local/R-4.2.0/bin/R
```

You can append `$PREFIX/local/R-4.2.0/bin/` to `$PATH` in your `.bashrc` or `.zshrc` so that you can execute `R` directly.

More info about this build:
```
R is now configured for aarch64-unknown-linux-gnu

  Source directory:            .
  Installation directory:      /data/data/com.termux/files/usr/local/R-4.2.0

  C compiler:                  gcc  -g -O2
  Fortran fixed-form compiler: gfortran -fno-optimize-sibling-calls -g -O2

  Default C++ compiler:        g++ -std=gnu++14  -g -O2
  C++11 compiler:              g++ -std=gnu++11  -g -O2
  C++14 compiler:              g++ -std=gnu++14  -g -O2
  C++17 compiler:              g++ -std=gnu++17  -g -O2
  C++20 compiler:              g++ -std=gnu++20  -g -O2
  Fortran free-form compiler:  gfortran -fno-optimize-sibling-calls -g -O2
  Obj-C compiler:              gcc -g -O2 -fobjc-exceptions

  Interfaces supported:        X11
  External libraries:          pcre2, readline, curl
  Additional capabilities:     PNG, JPEG, TIFF, NLS, cairo, ICU
  Options enabled:             shared R library, shared BLAS, R profiling

  Capabilities skipped:
  Options not enabled:         memory profiling

  Recommended packages:        yes
```

## Cling

A partially working cling. See https://github.com/kxxt/prebuilt-cling-for-android
