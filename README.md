# sbdiff

![sbdiff output](sbdiff.png)

sbdiff is a frontend for (GNU) `diff`.

It compares files and directories line by line, outputs the files side-by-side in two columns and colorizes the differences.
For it is a console application, no GUI is necessary.

## Install

In order to use it, you need [Lua](http://lua.org/) 5.2 or newer and the `diff` command in your `PATH`. 

Then just copy the file `sbdiff` e.g. to `/usr/local/bin/`.

## Usage

Type `sbdiff file1 file2` to see the differences between file1 and file2.

## Integration with Mercurial

Append the file `hgrc` to your `$HOME/.hgrc` or copy it to `/etc/mercurial/hgrc.d/sbdiff`

Then you can use sbdiff within Mercurial as external diff command:

    hg sbdiff ...

## Integration with Git

Run the following commands: (This will change `$HOME/.gitconfig`)

    git config --global diff.tool sbdiff
    git config --global difftool.sbdiff.cmd 'sbdiff $LOCAL $REMOTE'
    git config --global difftool.prompt false

Then you can use sbdiff within Git as external diff command:

    git difftool ...
