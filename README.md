# Xlib

X is an open source C++ library for creative coding. This library contains a variety of toolkits for portable and multi-function libraries. It constantly improves to provide the latest, coolest and most practical technology for multilingual and full functionality.

It's an abstraction in which software providing generic functionality can be selectively changed by additional user-written code, thus providing application-specific software. Provides a standard way to build and deploy applications. Include support programs, compilers, code libraries, tool sets, and application programming interfaces (APIs) that bring together all the different components to enable development of a project or system.

# Enviroment

It's strongly recommended that each developer should checkout the [VirtualIDE](https://github.com/VirtualLib/VirtualIDE.git) which providing the full depends of Xlib. You could select the submodules to update which you realy needed.

```
$ git checkout https://github.com/VirtualLib/VirtualIDE.git
$ git submodule update --remote --init --recursive --force -- "sub-items"
```

This project for VisualStudio depends of the macro of **ROOT**. You can set the *User Macros* var in *Microsoft.Cpp.Win32.user.props*.

```
$ where Microsoft.Cpp.Win32.user.props
$ %LOCALAPPDATA%\Microsoft\MSBuild\v4.0\Microsoft.Cpp.Win32.user.props
$ Set **Comon Property Pages->User Macros**
# ROOT = $([MSBuild]::GetDirectoryNameOfFileAbove($(ProjectDir), .root))
```

# Download and 🔠

Official binary distributions are available at [VirtualIDE]((https://github.com/VirtualLib/VirtualIDE.git).

After downloading a binary release, visit [WIKI](https://github.com/VirtualLib/Xlib/wiki) in your web browser for installation instructions.

## Install From Source

If a binary distribution is not available for your combination of operating system and architecture, visit [WIKI](https://github.com/VirtualLib/Xlib/wiki) in your web browser for source installation instructions.

# Getting Strted

## How to Contribute

**Xlib** is created by users for users and we welcome very contribution. There are no highly paid developers or poorly paid support personnel on the phones ready to take your call. There are only users who have seen a problem and done their best to fix it. This means **Xlib** will always need the contributions of users like you. 

## Requirements

* Recommended: Configure at least one target platform.
* Git
* Cmake
* Ninja(or other build tools)
* Recommended: Python, for fetching dependencies.

## CodeMap

```
├── console               <- provides access to the debugging console.
├── docs                  <- Some documentation around Xlib usage, per platform things to consider, etc
├── extensions            <- extend and modify the capability of xlib.
├── LICENSES              <- MIT license and third_party licenses.
├── scripts               <- Templates and small scripts for automating Xlib per platform
├── xlib                  <- Root directory for Source code
│   ├── ...               <- project source code
│   ├── base              <- the basic function code.
│   └── core              <- the core code.
├── testing               <- Unit tests and bug reports
├── tools                 <- Delivery Tools (e.g. Windows binaries, scripts, dockers)
├── .gitmodules           <- Top-level .gitmodules
├── README.md             <- Top-level README.md
```

## Building

**Xlib** uses CMake and Ninja as its building system but instructions are highly dependent on your operating system and target platform.

```
#!/bin/bash
$ cd generator/depot_tools/
$ gclient
$ gclient --v
$ where python
```

# Acknowledgements

**Xlib** couldn't exist without:

* All the contributors. Big or small a change, it does make a difference.
* All the developers that write the fantastic **software and libraries** that Xlib uses. We stand on the shoulders of giants.
* Our **fantastic community** for the never ending support, inspiration, feedback, and for keeping us on our toes when we screw up!
* **Our sponsors**. Without them, keeping a huge project like this alive would be next to impossible.

## Dependencies

One of our design goals is that **Xlib** itself should have no dependencies or as few dependencies as possible. The current external dependencies of the runtime library include:

* [7-Zip](https://www.7-zip.org/)
* [Boost](https://www.boost.org/)
* [Duilib](https://github.com/duilib/duilib)
* [RapidJson](http://rapidjson.org/zh-cn/)
* [STLPort](http://www.stlport.org/)

When building with *windows* enabled, we have a few additional small dependencies:

* [ATL](https://msdn.microsoft.com/zh-CN/library/t9adwcde.aspx)
* [WTL](http://wtl.sourceforge.net/)

The birth of **Xlib** is inseparable from the [github](https://www.github.com/) open source projects and other open source software. 

Thank you to every open source worker. I was unbelievably proud of you that you had made great and selfless contributions to the betterment of the world.

# License

**Xlib** is [MIT licensed](https://mit-license.org/). You may use, distribute and copy it under the license terms.
