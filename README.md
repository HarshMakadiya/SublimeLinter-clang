SublimeLinter-clang
=========================

This linter plugin for [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter3) provides an interface to [clang](__linter_homepage__). It will be used with files that have the C/C++/C Improved syntax.

## Installation
SublimeLinter 3 must be installed in order to use this plugin. If SublimeLinter 3 is not installed, please follow the instructions [here](https://github.com/SublimeLinter/SublimeLinter.github.io/wiki/Installation).

### Linter installation
Before using this plugin, you must ensure that `clang` is installed on your system. clang is already bundled on Mac OS X. On Linux, it can be easily installed using most package managers. 

Once `clang` is installed, you must ensure it is in your system PATH so that SublimeLinter can find it. This may not be as straightforward as you think, so please read [How linter executables are located](https://github.com/SublimeLinter/SublimeLinter.github.io/wiki/Usage#how-linter-executables-are-located) in the documentation.

Once you have installed `clang` you can proceed to install the SublimeLinter-clang plugin if it is not yet installed.

### Plugin installation
Please use [Package Control](https://sublime.wbond.net/installation) to install the linter plugin. This will ensure that the plugin will be updated when new versions are available. If you want to install from source so you can modify the source code, you probably know what you are doing so we won’t cover that here.

To install via Package Control, do the following:

1. Within Sublime Text, bring up the [Command Palette](http://docs.sublimetext.info/en/sublime-text-3/extensibility/command_palette.html) and type `install`. Among the commands you should see `Package Control: Install Package`. If that command is not highlighted, use the keyboard or mouse to select it. There will be a pause of a few seconds while Package Control fetches the list of available plugins.

1. When the plugin list appears, type `clang`. Among the entries you should see `SublimeLinter-clang`. If that entry is not highlighted, use the keyboard or mouse to select it.

## Settings
For general information on how SublimeLinter works with settings, please see [Settings](https://github.com/SublimeLinter/SublimeLinter.github.io/wiki/Settings). For information on generic linter settings, please see [Linter Settings](https://github.com/SublimeLinter/SublimeLinter.github.io/wiki/Linter-Settings).

In addition to the standard SublimeLinter settings, SublimeLinter-clang provides its own settings. Those marked as “Inline Setting” or “Inline Override” may also be [used inline](https://github.com/SublimeLinter/SublimeLinter.github.io/wiki/Settings#inline-settings).

|Setting|Description|Inline Setting|Inline Override|
|:------|:----------|:------------:|:-------------:|
|include_dirs|A list of directories to be added to the header search paths (-I is not needed).| | |
|extra_flags|a string with extra flags to pass to clang. These should be used carefully, as they can potentialy break the linter| | |

## Contributing
If you would like to contribute enhancements or fixes, please do the following:

1. Fork the plugin repository.
1. Hack on a separate topic branch created from the latest `master`.
1. Commit and push the topic branch.
1. Make a pull request.
1. Be patient.  ;-)

Please note that modications should follow these coding guidelines:

- Indent is 4 spaces.
- Code should pass flake8 and pep257 linters.
- Vertical whitespace helps readability, don’t be afraid to use it.
- Please use descriptive variable names, no abbrevations unless they are very well known.

Thank you for helping out!
