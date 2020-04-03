# knowledgejunkie-dotfiles-deps

## Description

A [Debian GNU/Linux][debian] metapackage to install applications and
dependencies for use with knowledgejunkie's [dotfiles][dotfiles].

Packages installed with this metapackage include:

- i3, i3blocks, rofi, compton, lightdm, light-locker, udiskie, connman-ui
- tmux, tmuxinator
- rxvt-unicode
- zsh
- vim-gtk
- git
- ripgrep
- exuberant-ctags
- build-essential, cmake, libclang1
- ranger, sxiv, zathura


## Building the metapackage

Build the binary package using git-buildpackge:

    $ gbp buildpackage

This will generate the binary .deb in gbp's configured output directory.


## Installing the metapackage

We can install the package using gdebi, which will automatically install
any missing dependencies

    # gdebi knowledgejunkie-dotfiles-deps_<version>_all.deb


## License

Copyright: 2016-20, Nick Morrott <nickm@debian.org>
License: GPL-2+


## Thanks

I hope you find this metapackage useful. Feel free to follow me on [GitHub][github] and [Twitter][twitter].

[debian]: https://www.debian.org/
[dotfiles]: https://github.com/knowledgejunkie/dotfiles
[github]: https://github.com/knowledgejunkie
[twitter]: https://twitter.com/nickmorrott
