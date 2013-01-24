# Totem's dotfiles

I have dotfiles (as every Linux user does) and I like them the same
everywhere. I also like low setup times, and highly customized settings.

## Files

Here's a short list of the dotfiles I have, and a description of what
they're for (d means directory):

* `bashrc`  
  The bash config file. I love changing my PS1 around. I rarely ever use
  any of the aliases I set up. Probably haven't customized this enough
  yet, could get more out of it.
* `bash` *(d)*  
  Saving any extensions for my bash configuration file. Most importantly
  the colours file and the Git script, showing what branch you're in
  inside your PS1.
* `vimrc`  
  The vim configuration file. I like weird things like `;` instead of `:`
  and disabling all arrow keys. Zenburn too.
* `vim` *(d)*  
  This is the vim config directory (obviously). Just some scripts that I
  wanted to include directly instead of using Vundle.

## How to use

Please Note: *I do not recommend, nor disapprove of or discourage using
these files without modification.* If you have the exact same desires as I
do, feel free to use it. I do recommend though to look into the files and
change things to how you like them best. Fork this on Github. Have fun!

Apart from that, the installation steps are currently quite easy:

1. Run `./linking`, this will automatically create symlinks to all files
  and folders in the files directory in your home directory (so that file
  is linked to by ~/.file).
2. Modify to your liking.

Uninstalling is as simple as running `./linking -r` which will remove all
symlinks in your home directory to files and folders in the files
directory.
