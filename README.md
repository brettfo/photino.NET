# Build native, cross-platform desktop apps

Photino is a lightweight open-source framework for building native,  
cross-platform desktop applications with Web UI technology.

Photino enables developers to use fast, natively compiled languages like C#, C++, Java and more. Use your favorite development frameworks like .NET 5, and build desktop apps with Web UI frameworks, like Blazor, React, Angular, Vue, etc.!

Photino uses the OSs built-in WebKit-based browser control for Windows, macOS and Linux.
Photino is the lightest cross-platform framework. Compared to Electron, a Photino app is up to 110 times smaller! And it uses far less system memory too!


# Photino.NET

This project represents the .NET 5 wrapper for the Photino.Native project, which makes it available for all operating systems (Windows, macOS, Linux).
This library is used for all the sample projects provided by Photino, which include Blazor, Vue.JS, Angular, React, or the basic HTML app: 
https://github.com/tryphotino/photino.Samples

If you made changes to the Photino.Native project, or added new features to it, you will likely need this repo to hook it all up and expose the new system calls to the .NET wrapper.
In all other cases, you can just grab the nuget package for your projects:
https://www.nuget.org/packages/Photino.NET

# How to build this repo

If you want to build this library itself, you will need:
 * Windows, Mac, or Linux
 * Make sure the Photino.Native Nuget package is added and up to date.
 * If you're on Windows:
   * Use Visual Studio with C++ support enabled. You *must* build in x64 configuration (*not* AnyCPU, which is the default).
   * Install Microsoft Edge Dev: https://www.microsoftedgeinsider.com/en-us/download
 * If you're on macOS:
   * Install Xcode so that you have the whole `gcc` toolchain available on the command line.
   * Inspect the repo .yml file for the exact build command for macOS
 * If you're on Linux (tested with Ubuntu):
   * Inspect the repo .yml file for the exact build command for Linux
 * If you're on Windows Subsystem for Linux (WSL), then as well as the above, you will need a local X server ([example setup](https://virtualizationreview.com/articles/2017/02/08/graphical-programs-on-windows-subsystem-on-linux.aspx)).
