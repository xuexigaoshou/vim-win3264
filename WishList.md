# Introduction #

What would you like to see in Vim for Windows?


# Details #

## Win64 ##

  * Support for Ruby, TCL, MzScheme, etc interfaces. This requires the owners of these languages to produce 64-bit builds.
  * Compile with [mingw-w64](http://mingw-w64.sourceforge.net/) in addition to MSVC.

## Visuals ##

  * Bigger Vim icon that don't look like crap on Vista; i.e., 64x64 or better. See [OS X Vim Icon](http://www.cs.princeton.edu/~mtwebb/vim_icon/vim_icons.html).
  * Better toolbar icons, such as the [Tango ones](http://tango.freedesktop.org/Tango_Icon_Library) or the [Silk ones](http://www.famfamfam.com/lab/icons/silk/).

## Console Vim ##

  * Full support for Unicode and UTF-8.
  * Parity with xterm Vim.

## Misc ##

  * Shell/pty support. Look at [VIM-Shell](http://www.wana.at/vimshell/), [PyConsole](http://www.vim.org/scripts/script.php?script_id=1974), [Console](http://sourceforge.net/projects/console/), and [Pexpect](http://www.noah.org/wiki/Pexpect).
  * Visual Studio integration for VS 200x. VisVim only works for VS98 (VC6). Look at [Visual Studio](http://code.google.com/p/vim-visual-studio/) plugin. [ViVim](http://code.google.com/p/vivim/) is a new contender as of Aug 2008.
  * Omni-completion for C# and other .NET languages. Steal intellisense stuff from [SharpDevelop](http://www.icsharpcode.net/OpenSource/SD/)? Look at [JavaComplete](http://www.vim.org/scripts/script.php?script_id=1785) too.
  * Full-screen mode like [MacVim](http://code.google.com/p/macvim/).
  * Incorporate [GVimExt\_Tab](http://www.vim.org/scripts/script.php?script_id=1720) functionality, if it's not already.
  * Play well with [Portable GVim](http://portablegvim.sourceforge.net/).
  * Support proportional fonts, like GTK version.
  * Investigate [CMake](http://lwn.net/Articles/188693/)
  * Play nice with [NTFS streams](http://www.nabble.com/VIM-and-NTFS-streams-to15203542.html).
  * Look at [if\_v8](http://www.vim.org/scripts/script.php?script_id=2375) integration.


## Performance ##

This should be of general benefit to Vim on all platforms.

  * Painting speed of gvim. Noticeably slower than console Vim on old machines.
  * Get rid of the DOS box for shell commands.
  * Profile start-up times, both with `-u NONE` and with a non-trivial set of plugins.
  * Profile heavyweight operations. For example, [VST](http://skawina.eu.org/mikolaj/vst.html) takes about 1 minute to regenerate its own documentation, running at 100% CPU. This case is probably a combination of inefficient script techniques, regexp inefficiencies, and inefficiencies in the core of Vim.

## Tools ##

Address issues with MiscTools.