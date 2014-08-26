---
layout: default
title: "Resources"
---

This page contains links to useful resources.

-   [Visual Studio 2013](http://e5.onthehub.com/WebStore/ProductsByMajorVersionList.aspx?ws=5d805b88-ce9b-e011-969d-0030487d8897&vsro=8&JSEnabled=1) is available through MSDNAA.
-   [FreeGLUT](http://freeglut.sourceforge.net/) the OpenGL window management package we will be using. The package is targetted to Linux, but you can get a distribution for [Windows](http://www.transmissionzero.co.uk/software/freeglut-devel/) (this package will also work on VS 2013).
-   [SOIL](http://www.lonesock.net/soil.html) the Simple OpenGL Image Library package we will be using. I have precompiled libraries for Windows and Mac OSX that can be downloaded in the corresponding installation section below.
-   [GLEW](http://glew.sourceforge.net/) the OpenGL Extension Wrangler Library package we will be using for shaders (since Windows contains an old version of OpenGL). NOTE: OSX contains a current version of OpenGL and thus does not require GLEW.

**FreeGLUT Installation Instructions**

*Windows 7 (Visual Studio 2013)*

1.  Download and extract [freeglut 2.8.1-1 for MSVC](http://www.transmissionzero.co.uk/software/freeglut-devel/).

2.  Copy the contents of the *include\\GL* directory to:
> -   (32-bit) C:\\Program Files\\Windows Kits\\8.1\\Include\\um\\gl
> -   (64-bit) C:\\Program Files (x86)\\Windows Kits\\8.1\\Include\\um\\gl

3.  Copy **freeglut.lib** from the *lib* directory (**NOT** the x64 subdirectory) to:
> -   (32-bit) C:\\Program Files\\Windows Kits\\8.1\\Lib\\win8\\um\\x86
> -   (64-bit) C:\\Program Files (x86)\\Windows Kits\\8.1\\Lib\\win8\\um\\x86

4.  Copy **freeglut.dll** from the *bin* directory (**NOT** the x64 subdirectory) to:
> -   (32-bit) C:\\Windows\\System32
> -   (64-bit) C:\\Windows\\SysWOW64

*Windows 8.1 (Visual Studio 2013)*

1.  Download and extract [freeglut 2.8.1-1 for MSVC](http://www.transmissionzero.co.uk/software/freeglut-devel/).

2.  Copy the contents of the *include\\GL* directory to:
> -   C:\\Program Files (x86)\\Windows Kits\\8.1\\Include\\um\\gl

3.  Copy **freeglut.lib** from the *lib* directory (**NOT** the x64 subdirectory) to:
> -   C:\\Program Files (x86)\\Windows Kits\\8.1\\Lib\\winv6.3\\um\\x86

4.  Copy **freeglut.dll** from the *bin* directory (**NOT** the x64 subdirectory) to:
> -   C:\\Windows\\SysWOW64

*Linux (\*ubuntu)*

From a terminal window

	$ sudo apt-get install freeglut3-dev

*Mac OSX*

Install [XCode](https://developer.apple.com/xcode/downloads/) which includes OSX GLUT libraries.


