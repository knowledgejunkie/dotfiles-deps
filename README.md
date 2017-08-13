# knowledgejunkie-dotfiles-deps

## Description

A [Debian GNU/Linux][debian] metapackage to install applications and dependencies
for use with knowledgejunkie's [dotfiles][dotfiles].

Packages installed with this metapackage include:

- i3
- rxvt-unicode-256color
- zsh
- tmux
- git
- ack-grep
- exuberant-ctags
- vim-gtk
- build-essential
- libclang1
- cmake


## Building the metapackage

A simple way to build the binary package is to change to the checkout directory and run:

    $ debuild -uc -us -b

This will generate the binary .deb file in the checkout's parent directory.

To clean the build directory afterwards, run:

    $ debuild clean
    $ git clean -fd


## Installing the metapackage

We can install the local package using gdebi, which will pull in missing dependencies
automatically as necessary:

    # gdebi /path/to/knowledgejunkie-dotfiles-deps_0.x_all.deb

Alternatively, we can use dpkg and apt-get to satisfy missing dependencies manually:

    # dpkg --install /path/to/knowledgejunkie-dotfiles-deps_0.x_all.deb
    # apt-get -f install


## License

GPL-2+


## TODO

- port to gbp


## Thanks

I hope you find this metapackage useful. Feel free to follow me on [GitHub][github] and [Twitter][twitter].

[debian]: https://www.debian.org/
[dotfiles]: https://github.com/knowledgejunkie/dotfiles
[github]: https://github.com/knowledgejunkie
[twitter]: https://twitter.com/nickmorrott
