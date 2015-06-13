# Dotfiles

Based on TotempaaltJ's dotfiles, with some modifications.

I have dotfiles (as every Linux user does) and I like them the same
everywhere. I also like low setup times, and highly customized settings.

## All files

I use a somewhat complicated directory structure, but it makes a lot of
sense when you know exactly what's happening:

* `files/`  
  These files aren't linked or copied at all. They're only
  utilized.
  * `bashrc`  
    The bash config file. I love changing my PS1 around.
  * `vimrc`  
    The vim configuration file. I like weird things like `;` instead of `:`
    and disabling all arrow keys. Zenburn too.
  * `gitconfig`  
    Instead of setting up my name and email address for git on every single
    machine I use, I figured I should just dump it in my dotfiles. It also has
    some aliases and shorthand URIs.
  * `screenrc`  
    Screen is amazing but it requires some minor customization to reach its
    full potential.

* `links/`  
  Files to be symlinked to (these are usually directories).
  * `bash/`  
    Saving any extensions for my bash configuration file. Most importantly
    the colours file and the Git script, showing what branch you're in
    inside your PS1.
  * `vim/`  
    This is the vim config directory (obviously). Just some scripts that I
    wanted to include directly instead of using Vundle.

* `templates/`  
  These files are copied to the home directory and have any
  occurrence of {{dotfiles}} replaced by the path to the dotfiles
  repository. This is so you can add any machine-specific configuration to the
  actual files.

## How to use

Please Note: *I do not recommend, nor disapprove of or discourage using
these files without modification.* If you have the exact same desires as I
do, feel free to use it. I do recommend though to look into the files and
change things to how you like them best. Fork this on Github. Have fun!

Apart from that, the installation steps are currently quite easy:

1. Run `./install`, this will walk you through the required steps for installing
  and configuring these dotfiles.
2. Modify to your liking.

Uninstalling is as simple as running `./install -r` which will remove all
symlinks in your home directory to files and folders in the files
directory. It won't, however, remove the copied template files!
