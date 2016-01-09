stevemoser dotfiles
===============

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
stevemoser/dotfiles together using [the `*.local` convention][dot-local].

[dot-local]:
http://robots.thoughtbot.com/manage-team-and-personal-dotfiles-together-with-rcm

Requirements
------------

Set zsh as my login shell.

    chsh -s /bin/zsh

Install [rcm](https://github.com/mike-burns/rcm).

    brew tap thoughtbot/formulae
    brew install rcm

Install
-------

Clone onto my laptop:

    git clone git://github.com/stevemoser/dotfiles.git

Install:

    env RCRC=$HOME/stevemoser/dotfiles/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[lldb](http://lldb.llvm.org) configuration:

* [Fix Console `po frame` Printing](https://gist.github.com/natecook1000/151d8de423eb77fc87bf#gistcomment-1656670)