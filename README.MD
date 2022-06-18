# Termux

This repo contains my various files related to termux.

## R

The package `r-base` in its-pointless repo is outdated and incompatible with the latest  version of termux.

So I built it myself. I hope you enjoy it.

Download: https://github.com/kxxt/termux/releases/download/R-4.2.0-1/R-4.2.0-1-termux-arm64.tar.xz

Usage: (You'll need to setup its-pointless repo to install `libgfortran5`)

```shell
wget https://github.com/kxxt/termux/releases/download/R-4.2.0-1/R-4.2.0-1-termux-arm64.tar.xz
tar xJf R-4.2.0-1-termux-arm64.tar.xz $PREFIX
pkg install libgfortran5
# Start R
$PREFIX/local/R-4.2.0/bin/R
```

You can append `$PREFIX/local/R-4.2.0/bin/` to `$PATH` in your `.bashrc` or `.zshrc` so that you can execute `R` directly.
