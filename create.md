---
title: Essential Tools
description: A list of common tools needed for mod creation.
published: true
date: 2025-04-30T21:41:52.500Z
tags: 
editor: markdown
dateCreated: 2025-04-30T21:41:52.500Z
---

# Essential Tools

This list covers the basics you'll likely need for mod creation.

## Oblivion Remastered

You’ll need the game installed to access its assets and test your mods. Both the Steam and Game Pass versions work for modding, but some tools may require specific configuration depending on your install type.

## Oblivion Construction Set

The original Oblivion Construction Set was built for classic Oblivion, but much of the legacy game data is still editable with this tool. Many past modding tutorials will still partially apply to *Oblivion Remastered*. As a general rule, mods affecting UI and graphics will also need work done on the Unreal Engine side.

## FModel

FModel is used to browse and extract assets from Unreal Engine PAK files. Since *Oblivion Remastered* uses Unreal for many of its new systems, FModel is essential for viewing textures, models, UI elements, and other packaged content.

## UE4SS (Unreal Engine 4 Script Suite)

UE4SS is both a script loader and runtime injector for the Unreal Engine side of the game. It enables Lua-based scripting and allows modders to hook into menus, logic, and behaviors on the UE side.

## OBSE64 (Oblivion Remastered Script Extender)

While not a direct port of the original OBSE, it serves a similar purpose by enabling engine-level mod enhancements. 

## UE4SS TesSyncMapInjector

This allows `.esp` form IDs (such as items, weapons, or placed objects) to be synced with the engine’s runtime systems, without needing to pack them into a `.pak` file.

## TES4Edit

TES4Edit is used to inspect, clean, and manage plugin files. It helps detect conflicts, clean unnecessary edits, and keep your load order stable. It remains a vital tool for working with `.esp`/`.esm` files even in the remastered version.

## Text Editor (Notepad++ or Visual Studio Code)

A good text editor is essential for writing Lua scripts (for UE4SS) and editing config files. Notepad++ and VS Code are common options.
