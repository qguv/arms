# ARMS: The Archlinux Regular Maintainence Script

## Usage

    arms [-p] <options for reflector>
    arms --help

Pass `-p` as the first option to use `less -R` as a pager.

## Installing

Install [`arms-git`](https://aur4.archlinux.org/packages/arms-git/) from [the AUR](https://wiki.archlinux.org/index.php/Arch_User_Repository).

Alternatively:

    sudo install arms /usr/local/bin
    arms

## Optional dependencies

If [`reflector`](https://www.archlinux.org/packages/community/any/reflector/) is installed, the mirrorlist will update with the fastest HTTPS mirrors (by default) every time you run ARMS. You can also pass arguments to reflector by simply specifying them as arguments when you run `arms`.

If [`lostfiles`](https://aur4.archlinux.org/packages/lostfiles/)<sup>AUR</sup> is installed, ARMS will scan for files not owned by any pacman package.

## Known bugs

`util-linux` doesn't get excluded like it should from the "installed packages" output; instead, `util-` is printed. Feel free to PR and fix.
