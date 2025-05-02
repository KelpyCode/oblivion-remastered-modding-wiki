---
title: Setting up Unreal Engine
description: 
published: true
date: 2025-05-02T05:31:12.394Z
tags: modding, unreal-engine, tool
editor: markdown
dateCreated: 2025-04-27T22:19:03.979Z
---

# Setting up Unreal Engine 5.3 project (old version)
## 🛠️ You Need:
- [Oblivion Remastered Project](https://www.nexusmods.com/oblivionremastered/mods/880)
- **Unreal Engine 5.3+** (built from source)
- **Visual Studio 2022** (C++ workload)
- ~250GB free space

---

## 📋 Setup Steps:
0. **Link your GitHub to your Epic account**
	 - Follow [this guide](https://dev.epicgames.com/documentation/en-us/unreal-engine/downloading-source-code-in-unreal-engine#accessingunrealenginesourcecodeongithub).
  
1. **Download Unreal Source**  
   - From [Epic Games GitHub](https://github.com/EpicGames/UnrealEngine) (link Epic account)
   - From [Community Maintained Fork](https://github.com/C0bra5/UnrealEngine) (link Epic account)

2. **Extract and Set Up**  
   - Extract (e.g., `D:\UnrealEngine5.3`)  
   - Run `Setup.bat` and `GenerateProjectFiles.bat`

3. **Build Unreal Engine**  
   - Open `UE5.sln` in Visual Studio  
   - Config: **Development Editor** / Platform: **Win64**  
   - Build the **UE5** project (1–3 hrs) *make sure to click the arrow next to the folder `Engine` and only build **UE5** from there and not the whole solution*

4. **Launch Unreal**  
   - Run `UnrealEditor.exe` from `Engine\Binaries\Win64`

5. **Open the Project**  
   - Right-click `OblivionRemastered.uproject` → "Switch Unreal Version" if needed  
   - Double-click to open  
   - First load compiles shaders (5–30 min)

---

## 🚫 Common Problems:
| Problem | Fix |
|:---|:---|
| Overflow in constant arithmetic | Replace `INFINITY` with `FLT_MAX` |
| Metadata file missing | Ignore if Editor runs |
| "Open With" clutter | Use NirSoft's OpenWithView

---

## 🔥 FAQ:
- **Can I share this?**  
  ✅ If you package/cook the project or share uncooked assets.  
  ❗ Needs source-built UE5 to mod.

---

# ✅ In Short:
**Build UE5 ➔ Launch ➔ Open Project ➔ Mod Away**


----
__Credit @karmirith (Discord)__ 