# Dressmaker Automation - Windows version

Windows installer for **Dressmaker Automation 1.1.0**, a mod for Dressmaker.

Original mod, patcher and `DressmakerAutomation.Core.dll` by **buchongfuname**.
The Windows scripts (`install.bat/ps1`, `uninstall.bat/ps1`) are by **DearSweetele**.
Uploaded with the original author's permission. The original files and the MIT license are included unchanged.

## What it does
- Auto grain alignment
- Find valid position (no overlapping pieces)
- Auto mannequin sizing from the customer's body
- Infinite money (optional)

## Requirements
- Dressmaker 0.7.0 (Steam, Windows)
- .NET Runtime 6 or newer (the normal one, not "Desktop"): `winget install Microsoft.DotNet.Runtime.8`
- No BepInEx needed. The mod patches `Assembly-CSharp.dll`.

## Install
1. Close the game. Download the ZIP from Releases and extract it fully.
2. Double-click `install.bat` and follow the window.

It finds the game in Steam, patches a temporary copy first, and backs up your original `Assembly-CSharp.dll` to `%LOCALAPPDATA%\DressmakerAutomation\backups`.

## Uninstall
Close the game and run `uninstall.bat`, or use "Verify integrity of game files" in Steam.

## Settings
`DressmakerAutomation.cfg` is created on first start in
`%USERPROFILE%\AppData\LocalLow\Unity Technologies\com.unity.template.urp-blank`.
Set to `false` and restart: `InfiniteMoney`, `AutoGrainAlignment`, `AutoMannequinSizing`, `FindValidPosition`.
