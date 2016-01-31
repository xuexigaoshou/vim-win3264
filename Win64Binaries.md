Installing Vim Binaries on Win64

# Introduction #

I have ported Vim to run natively on Win64, the 64-bit flavor of Windows.
The Win32 vim.exe and gvim.exe have always run on Win64,
but things like the "Edit with Vim" shell extension didn't work.

There is no nice installer for the Win64 binaries yet.

The 7.2 build of Vim supports the Python interface.
You must install the Win64 build of
[Python 2.5.2](http://www.python.org/download/releases/2.5.2/)
to use it.

# Installation #

To install Vim, first download [vim72.zip](http://vim-win3264.googlecode.com/files/vim72.zip).
This 18MB file contains all the files you need for a full installation,
including the latest Vim runtime.

Unzip the zipfile into a directory whose name ends in `vim`,
such as `C:\Program Files\Vim`, `D:\vim`, or
`C:\mytools\vim`. This will create a `vim72`
subdirectory, containing all the files. Start a `cmd.exe`
window, `cd ...\vim\vim72`, then run `install.exe`,
the command-line installer. This will offer you a series of choices.
You can probably just type `d` to "do it".`

On Vista and Windows 7, you must run the cmd window as an Administrator.
(Most users run as administrators on earlier versions of Windows.)

  * In Windows Explorer, go to c:\windows\system32, select cmd.exe, and right-click. Choose Run as Administrator.

  * In the new Administrator cmd window, `cd` to the directory where you unzipped the Vim binaries and run `install.exe`. You should now be able to successfully create the batch files and register "Edit with Vim".

To uninstall, use `uninstall.exe` in the same directory.

Note: The message translations (`:help win32-gettext`)
do not yet work, because I have not been able to locate
a Win64 version of `libintl.dll`.