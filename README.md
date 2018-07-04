setgit python script
==================================
Overview
--------

I found myself juggling a couple of gitconfigs (my personal one linked to my github account and one for my employer's Enterprise git server) and wanted an easy solution to switching between configs. So, here we are. This may not be the most elegant solution but it works for me.

Installation
------------

Clone this repo or download the setgit bash script to a folder in your path.

Copy your current ~/.gitconfig to ~/.gitconfig-me
Copy your current ~/.ssh/config to ~/.ssh/config-me

Then create your different git and ssh config files appending the name with -sourcename.
For example ~/.gitconfig-work and ~/.ssh/config-work


Running
------------
From the command line run:
$ setgit sourcename

The contents of ~/.gitconfig-sourcename will overwrite the ~/.gitconfig contents.
The contents of ~/.ssh/config-sourcename will overwrite the ~/.ssh/config contents.

When you want to switchback to your original config run:
$ setgit me
