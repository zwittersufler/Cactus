## Singling
##### By: Jonathan Vasquez (fearedbliss)
##### Build: 2020-05-25-1030

## Description

A collection of non-gameplay modifications and fixes in
order to improve the Vanilla Diablo II Single Player Experience.

## Supported Versions

- **`1.05b`**
- **`1.07`**
- **`1.09b`**
- **`1.14d`**

## Features

- You can now run multiple clients of Diablo II.
- You are now able to quickly join LAN games.
- Fixed CPU usage bug in Main Menu, Single Player, and LAN games.
- The Battle.net button has been disabled for safety reasons.
- The introduction cinematics are now automatically skipped.

- **`[1.05b-1.09b]`** The massive slowdown when the letters on the top left appears is now fixed.
- **`[1.05b-1.09b]`** You no longer need the CD in order to play the game.
- **`[1.05b-1.09b]`** You can now make Hardcore characters without beating Softcore.
- **`[1.05b-1.09b]`** The window will no longer minimize when you click out of it.
- **`[1.05b-1.09b]`** The window will now have Minimize and Close buttons.

- **`[1.14d]`** Battle.net-only Runewords are now enabled on Single Player.

## Notes

- The Main Menu CPU fix will only be applied for **`v1.10+`**, since people not
  using Glide in versions before that would experience massive lag. Most people
  don't spend their time sitting in the Main Menu so this isn't a big deal.

- If you are using Glide, make sure to disable VSYNC in your Glide settings
  or you will still experience high CPU usage in LAN games.

- Due to a Windows bug, the Minimize/Close buttons will not show if you are
  using Glide for versions below **`1.14d`**.
  
- The fix for the massive slowdown when the letters on the top left of the screen appears
  required us to disable the **`/fps`** command.
  
- In order for the **`Prevent Window Minimization`** fix to work, make sure that the game
  was started with **`-w`**. Making the GlideWrapper settings have Window Mode is not enough.

- If you are using **`OBS Studio`**, make sure you use **`Window Capture`** rather than **`Game Capture`**.
  The latter will make the game crash when you exit the game. This is not a bug caused by Singling,
  it also happens with Vanilla D2.

## Patch Rationale

#### Patch 1.05b

This patch was picked over **`1.00`** because it is the most stable version
of the game before **`Lord of Destruction`**, and has the most features and balance
compared to the previous patches. It was also picked over **`1.06`** since the main
reason **`1.06`** was released was to implement anti-duping code. Due to the way
item generation works in these patches, you can legitimately find items that have
the same fingerprint, and the anti-duping code would delete those items.

#### Patch 1.07

This patch was selected because it is the first version of **`Lord of Destruction`**
that was released and was the first massive change to Diablo II. Due to this, it contains
a lot of features, behaviors, and item generation combinations that were immediately
patched out in patches **`1.08`** and **`1.09`**. It also contains some bugs that are fun
to play with such as the Rejuvenation Potion Bug or Mana Per Kill (MPK) rings.

#### Patch 1.09b

This patch was picked over **`1.09d`** because it is the most stable version of Diablo II
before the massive changes implemented in 1.10, and also because it contains **`players 64`**
and working CtC. **`1.09d`** has broken CtC which means that you will see the animation
of your CtC effect, but it actually won't do anything.

#### Patch 1.14d

This patch was selected since it's currently the latest version of the game
that includes all of the latest quality of life improvements, features,
and fixes, such as synergies, 1.10+ runewords, fast merc leveling, respecs,
higher rune drop rates, window improvements, and more.