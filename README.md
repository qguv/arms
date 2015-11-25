# ARMS: The Arch Regular Maintainence Script

## Installing

    sudo install arms /usr/local/bin
    arms

## Running without installing

    git clone https://github.com/qguv/arms.git
    arms/arms

A PKGBUILD is on its way.

## Known bugs

`util-linux` doesn't get excluded like it should from the "installed packages" output; instead, `util-` is printed.
