# Dotfiles

## Overview

This repo is a skeleton/template repo for tracking dotfiles.  It contains
a utility ([dfm](https://github.com/justone/dfm)) to help with managing and
updating your dotfiles.

This fork contains a slightly modified version of the original utility:

* Usage of `~/.local/bin` instead of `~/bin` to comply with the XDG specification
* Renamed auxilliary files and folders (`.backup` to `.dotbackup` and 
`.dfminstall` to `.dotinstall`)

## Using this repo

First, fork this repo.

Then, add your dotfiles:

    $ git clone git@github.com:username/dfm.git .dotfiles
    $ cd .dotfiles
    $  # edit files
    $  # edit files
    $ git push origin master

Finally, to install your dotfiles onto a new system:

    $ cd $HOME
    $ git clone git@github.com:username/dfm.git .dotfiles
    $ ./.dotfiles/.local/bin/dfm install # creates symlinks to install files

## Full documentation

For more information, check out the [wiki](http://github.com/justone/dotfiles/wiki).

You can also run <tt>dfm --help</tt>.
