This document describes a comparison of technologies to develop a Desktop application on Windows which will lead to a choice to develop the project. Only technologies based on dotNet will be considered here.

# Frameworks for the UI
Here it will be discussed the choice of the framework used for the graphical interface

## Deprecated Frameworks

### WinForms
[WinForms](https://learn.microsoft.com/en-us/dotnet/desktop/winforms/?view=netdesktop-6.0) (or Windows Forms) has long been the default technology for Windows dotNET development. However, the project has been in maintenance mode since 2014, so no features have been added since. It was therefore decided to use more modern technologies.

## Current frameworks
Windows offers several dotNet development solutions for a Desktop app now. The main ones being WPF, WinUI and MAUI.

### WPF
[WPF](https://learn.microsoft.com/en-us/dotnet/desktop/wpf/?view=netdesktop-6.0) (Windows Presentation Forms) is currently the most used library for Desktop apps. It is a framework with a lot of resources available, the framework being available since 2006. The way of creating user interface is similar to the classic way of developing the UI in Android which consists of a file in a language of markup (here XAML) describing the structure of the UI and a code file allowing to link the graphic elements to the data.

### WinUI

[WinUI](https://learn.microsoft.com/en-us/windows/apps/winui/) (Windows UI) is an alternative framework to WPF. It works in a relatively similar way to WPF but offers more modern designs than WPF because it follows the [Fluent Design System](https://www.microsoft.com/design/fluent/) which are design rules applicable to Windows apps. However, being newer than WPF, it has fewer resources available than the latter in terms of libraries and support.

### MAUI
[.NET Multi-platform App UI](https://learn.microsoft.com/en-us/dotnet/maui/?view=net-maui-7.0) (MAUI) is Microsoft's modern solution for cross-platform apps (PC, Mac, Android, IOS). It can be considered Microsoft's Flutter. In the case of Windows applications because it is the target of the project, MAUI relies on WinUI.


# Choice of the framework

It was decided to discard MAUI because within the scope of the project, there is no need to have cross-platform which would add unnecessary constraints. The choice therefore had to be made between WPF and WinUI. Both are relatively similar but the choice was to go with WPF for the reason that due to its age, more resources are available than for WinUI, also the project interface being relatively simple, there is not necessarily a need to have a state-of-the-art UI.

WPF will therefore be the UI framework used.

# Languages

With the choice of WPF, this necessarily restricts the choice of the programming language used. The two main choices are C# and F#. C# is the classic dotNet object-oriented language while F# is its functional counterpart.
C# was chosen purely out of personal preference as I'm more comfortable with object oriented than functional and because it has more resources than F#.
