# ARMS: The Arch Regular Maintainence Script

## Usage

    arms <options for reflector>

## Installing

You really ought to use the AUR. Alternatively:

    sudo install arms /usr/local/bin
    arms

## Known bugs

`util-linux` doesn't get excluded like it should from the "installed packages" output; instead, `util-` is printed. Feel free to PR and fix.
