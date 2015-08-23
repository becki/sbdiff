# sbdiff

sbdiff is a frontend for (GNU) `diff`.

It compares files line by line, outputs the files side-by-side in two columns and colorizes the differences.
For it is a console application, no GUI is necessary.

In order to use it, you need [Lua](http://lua.org/) 5.2 or newer and the `diff` command in your `PATH`. Copy the file `sbdiff` e.g. to `/usr/local/bin/`.

Type `sbdiff file1 file2` to see the differences between file1 and file2.
