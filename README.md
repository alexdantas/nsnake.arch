# nsnake.arch

This repository contains the **Arch Linux packaging files** for the game nsnake (_classic snake game on the terminal_).

If you're after the game itself, [go to it's homepage][home].

![screen](http://nsnake.alexdantas.net/images/large-maze-with-lots-of-fruits.png)

## Arch Linux packaging

* [**nsnake on AUR**][aur]

Unlike [other systems](https://github.com/alexdantas/nsnake.debian), packaging for
Arch Linux is fairly easy.

All you need is inside the file PKGBUILD.

## Getting Started

Here's a regular workflow...

```bash
# Retrieves the latest package files
$ git clone https://github.com/alexdantas/nsnake.arch
$ cd nsnake.arch

# Work on your changes...

# If the source file changed, this updates
# the PKGBUILD with new checksums
$ updpkgsums

# This command does the following:
# 1. Gets the source code;
# 2. Validates it with sha256sums;
# 3. Compiles it on the current dir;
$ makepkg

# Creates an AUR ball (.src.tar.gz), ready to uploaded
# to AUR via their web interface
$ mkaurball
```

[home]: http://nsnake.alexdantas.net/
[aur]: https://aur.archlinux.org/packages/nsnake/

