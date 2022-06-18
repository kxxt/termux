# Termux

This repo contains my various files related to termux.

## R

The package `r-base` in its-pointless repo is outdated and incompatible with the latest  version of termux.

So I built it myself. I hope you enjoy it.

Download: link

Usage: (You'll need to setup its-pointless repo to install `libgfortran5`)

```shell
wget ...
tar xJf R-4.2.0-termux-arm64.tar.xz $PREFIX
pkg install libgfortran5
# Start R
$PREFIX/R-4.2.0/bin/R
```

You can append `$PREFIX/R-4.2.0/bin/` to PATH  in your `.bashrc` or `.zshrc` so that you can execute `R` directly.