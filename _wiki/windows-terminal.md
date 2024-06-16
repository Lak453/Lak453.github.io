---
layout: wiki
title: Windows Terminal
cate1: Tools
cate2:
description: Windows Terminal
keywords: Windows Terminal
---

## Customizing Windows Terminal

Windows Terminal is a new console terminal developed by Microsoft. Although it is still in the Preview version, it can already be used quite well with some configuration.

### Custom Themes

You can find suitable themes for Windows Terminal under the windowsterminal section at [iTerm2 Color Schemes](https://github.com/mbadolato/iTerm2-Color-Schemes).

### Custom Configuration File Location

I want to place the configuration file in the HOME directory and manage it with git. This can be achieved with the following method:

First, move the `~/AppData/Local/Packages/Microsoft.WindowsTerminal_8wekyb3d8bbwe/RoamingState/profiles.json` file to `~/Windows-terminal-profiles.json`. Then, open PowerShell with administrator privileges and execute:

```shell
New-Item -ItemType SymbolicLink -Path ~/AppData/Local/Packages/Microsoft.WindowsTerminal_8wekyb3d8bbwe/RoamingState/profiles.json -Target ~/windows-terminal-profiles.json
```

You can see my Windows Terminal configuration file at [my GitHub repository](https://github.com/mzlogin/config-files/blob/master/windows-terminal-profiles.json).

### Managing PowerShell Configuration with Git

Open PowerShell with administrator privileges and execute:

```shell
New-Item -ItemType SymbolicLink -Path ~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1 -Target ~/powershell.ps1
```

If you are using PowerShell 7 Preview, execute:

```shell
New-Item -ItemType SymbolicLink -Path <My Documents>/PowerShell/Microsoft.PowerShell_profile.ps1 -Target <User Directory>/powershell.ps1
```

Note that both directories need to use absolute paths, otherwise, an error will occur.

You can see my PowerShell configuration at [my GitHub repository](https://github.com/mzlogin/config-files/blob/master/powershell.ps1).

### Custom Keyboard Shortcuts

For example, to map copy and paste in Windows Terminal to `ctrl+c` and `ctrl+v` in the JSON configuration file under `globals -- keybindings`, add the following:

*Updated 2020-04-26: These mappings are no longer necessary as the new version provides default mappings.*

```json
{ "command": "copy", "keys": ["ctrl+c"] },
{ "command": "paste", "keys": ["ctrl+v"] }
```

For split pane and move focus within panes:

```json
{ "command" : "splitHorizontal", "keys": [ "alt+-" ] },
{ "command" : "splitVertical", "keys": [ "alt+\\" ] },
{ "command" : "closePane", "keys": [ "alt+w" ] },
{ "command" : "moveFocusLeft", "keys": [ "alt+left" ] },
{ "command" : "moveFocusRight", "keys": [ "alt+right" ] },
{ "command" : "moveFocusUp", "keys": [ "alt+up" ] },
{ "command" : "moveFocusDown", "keys": [ "alt+down" ] }
```

Reference: [Using JSON Settings](https://github.com/microsoft/terminal/blob/master/doc/user-docs/UsingJsonSettings.md)
