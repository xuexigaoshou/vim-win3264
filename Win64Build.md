# Introduction #

What you need to build a Win64 binary for Vim.


# Details #

First, get the Vim source from [Subversion](http://www.vim.org/subversion.php) or [CVS](http://www.vim.org/cvs.php).

I use [8win64.bat](http://vim-win3264.googlecode.com/files/8win64.bat) to set up environment variables for VS 2005 (VC 8), and [9win64.bat](http://vim-win3264.googlecode.com/files/9win64.bat) for VS 2008 (VC 9). Run the appropriate batchfile once.

Then follow the instructions in `src/INSTALLpc.txt`. Essentially,
```
nmake -f Make_mvc.mak GUI=yes
```
with other optional arguments.