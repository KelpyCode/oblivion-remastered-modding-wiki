---
title: Getting Started on Linux
description: 
published: true
date: 2025-08-17T02:03:12.046Z
tags: modding, unreal-engine, tool
editor: markdown
dateCreated: 2025-08-17T02:03:12.046Z
---

# Getting Started on Linux

## Requirements

- dotnet-sdk
- clang
- code (Visual Studio Code)
- protontricks

## Unreal Engine

1. Download Unreal Engine

    - [Downloading Unreal Engine Source Code from GitHub (Epic Games)](https://dev.epicgames.com/documentation/en-us/unreal-engine/downloading-source-code-in-unreal-engine)

    - Select the "5.3" branch then Code \> Download ZIP

        - Extract the archive `~/.local/share/UnrealEngine-5.3/`

1. Build Unreal Engine

    - [Fix UInputDeviceTriggerResistanceProperty (GitHub)](https://github.com/nathtest/UProjOblivionRemastered/tree/master?tab=readme-ov-file#unreal-532-source-fix)
    
        ![UInputDeviceTriggerResistanceProperty](/uinputdevicetriggerresistanceproperty.png)

    - [Building Unreal Engine from Source (Epic Games)](https://dev.epicgames.com/documentation/en-us/unreal-engine/building-unreal-engine-from-source)

1. Download Oblivion Remastered Project

    - [UProjOblivionRemastered (GitHub)](https://github.com/nathtest/UProjOblivionRemastered) then Code \> Download ZIP

        - Extract the archive `~/Documents/Unreal Projects/OblivionRemastered/`

<!-- todo: JsonAsAsset -->

1. Generate Visual Studio Code Workspace

    ```bash
    cd ~/.local/share/UnrealEngine-5.3/Engine/Build/BatchFiles/Linux/
    ./GenerateProjectFiles.sh -vscode -project=/home/<user>/Documents/Unreal\\ Projects/OblivionRemastered/OblivionRemastered.uproject
    ```

1. Launch UnrealEditor `~/.local/share/UnrealEngine-5.3/Engine/Binaries/Linux/UnrealEditor`

1. Open Project `~/Documents/Unreal Projects/OblivionRemastered/OblivionRemastered.uproject`

    - If prompted: Convert Project > More Options > Convert in-place

<!-- todo: link to guide for configuration -->

## FModel

1. [Download .NET 8.0](https://dotnet.microsoft.com/en-us/download/dotnet/8.0) then .NET Desktop Runtime > Windows x64

1. Install `windowsdesktop-runtime-8.0.19-win-x64.exe`

    - Right-Click > Open with Protontricks Launcher > The Elder Scrolls IV: Oblivion Remastered: 2623190 > OK

1. [FModel (GitHub - Fork)](https://github.com/C0bra5/FModel/releases/latest) then Download FModel-WithNaniteExport.exe

    - Move the file `~/.local/share/Steam/steamapps/compatdata/2623190/pfx/drive_c/FModel/`

1. [TES4R Mapping File 1.2 (Nexus)](https://www.nexusmods.com/oblivionremastered/mods/4897) then FILES > Manual download

    - Extract the archive `~/.local/share/Steam/steamapps/compatdata/2623190/pfx/drive_c/FModel/`

1. Launch FModel `~/.local/share/Steam/steamapps/compatdata/2623190/pfx/drive_c/FModel/FModel-WithNaniteExport.exe`

    - Right-Click > Open with Protontricks Launcher > The Elder Scrolls IV: Oblivion Remastered: 2623190 > OK

<!-- todo: link to guide for configuration -->

## Native Tools

- [retoc (GitHub)](https://github.com/trumank/retoc/releases/latest)
- [blender](https://www.blender.org/download/)
