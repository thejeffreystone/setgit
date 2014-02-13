==================================
setgit python script
==================================
Overview
--------

I found myself juggling a couple of gitconfigs (my personal one linked to my github account and one for my employer's internal git server) and wanted an easy solution to switching between configs. Thus I wrote this really simple python script

Installation
------------

Clone this repo or download the setgit bash script to a folder in your path.

Copy your current gitconfig to gitconfig-me.  

Then create your different .gitconfigs appending the name with -sourcename. For example .gitconfig-work


Running
------------
From the command line run:
$ setgit -l sourcename

The contents of .gitconfig-sourcename will overwrite the .gitconfig contents. 

When you want to switchback to your original config run:
$ setgit -l me










