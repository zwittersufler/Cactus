## Cactus
##### By: Jonathan Vasquez (fearedbliss)
##### Build: 2020-05-25-1030

## Description

Cactus is a C# based application that will help you manage **`Multiple Versions or _Compatible Mods_`**
of Diablo II (Which I will call **`Platforms`**) from a single application. This is a **`File-based
Version Switcher`** and thus it doesn't modify any files. It simply copies files from their respective
**`Platforms`** folder, to the root of your Diablo II folder, while making sure that all of your characters
are properly isolated. This means you can easily install and play every single version of Diablo II
from **`1.00`** to the latest **`1.14d`** (and any other future versions) while maximizing your disk space
(Since you won't have to keep having multiple copies of your MPQs).

## Cactus Repository

The following opt-in modifications are also available in this repository:

#### [Singling](README-SINGLING.md)

A collection of non-gameplay modifications and fixes in
order to improve the Vanilla Diablo II Single Player Experience.

To use Singling, simply copy the Singling files for the version you want to play
from the **`Singling/1. Files`** folder, and replace the ones for the equivalent version
in your Platforms directory. To revert, use the files in **`Singling/2. Stock`** instead.

## License

Released under the [Apache License 2.0](LICENSE.txt).

## Requirements

- .NET Framework 4.6.1 +

## Installation Instructions ([Video](https://youtu.be/j7gyc6jp644))

### Install Cactus And Prepare MPQs

This section will help you install Cactus to the correct location and also help you
fix your MPQs so that they are compatible with the older versions of Diablo II.

1. Copy all of the files in the **`1. Files`** folder into your Diablo II root folder.
2. Run the **`FIX_MPQS_RUN_AS_ADMIN.bat`** inside the **`MpqFixer`** that you copied, as
   **`Administrator`**. This will fix your MPQ files so that they work with the older versions
   of the game.

### Adding/Running A Platform

1. Run **`Cactus.exe`**
2. Click **`Add`**
3. Type in the name of the Platform you want to run. This should match a folder in the **`Platforms`**
   folder. (Example: If you want to run **`1.09b`**, type **`1.09b`**).
4. Enter the path to the executable you want to launch in your Diablo II root folder.
   Cactus copies all of the files from the **`Platforms/[NAME]`** folder to the Diablo II root folder,
   so most of your entries will have identical paths (Example: **`D:\Games\Diablo II\Game.exe`**).
5. Enter the Flags you want (Example: **`-w -ns -3dfx`**)
6. Make sure **`Expansion`** is selected (Unless you are playing **`1.00-1.06b`** or didn't purchase **`Lord of Destruction`**).
7. Click **`Add`**.
8. Select your newly added Platform and press **`Launch`**.

The game should start. If you are having video issues, either make sure you have ran
the **`D2VidTst.exe`** and configured everything properly **`(Pre 1.14)`**, or try configuring
**`GlideWrapper (glide-init.exe)`** and adding the  **`-3dfx`** flag to the end of your path.

## Moving Cactus To A New Computer

If you want to move all of your Platforms, Characters, and Diablo II folder
to another machine, you will need to:

1. Copy your entire Diablo II folder to your new machine.
2. Edit the **`Entries.json`** file and change the **`Path`** for all of your entries
   so that it now has the **`Path`** on your new machine.
   - The **`Base Directory`** for all Paths need to match. The exes can be different.
   		- GOOD: **`D:\Games\Diablo II\Game.exe`** and **`D:\Games\Diablo II\Alpaca.exe`**.
   		- BAD: **`D:\Games\Diablo II\Game.exe`** and **`D:\Diablo Immortal For PC\Game.exe`**.
3. Open **`Cactus`** and edit the **`Last Ran Platform`**.
4. Uncheck the **`Last Ran`** box and Click **`Edit`**.
5. Now **`Launch`** whatever Platform you want.

Unchecking the **`Last Ran`** box will cause Cactus to reconfigure itself (Including registry locations).

## Updating Files In The Platforms folder

If you update any files in your Platforms folder, then uncheck the **`Last Ran`**
box from the corresponding platform, and run it again. This will cause Cactus
to re-install the files with the new ones.
