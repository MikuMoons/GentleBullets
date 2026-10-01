# GentleBullets for 7 Days to Die

A small server-side XML mod that greatly reduces firearm damage to blocks, helping prevent stray bullets from tearing up your base.

Ordinary supported bullet impacts are intended to deal the engine minimum of **1 HP per impact**. Shotgun pellets count individually. Damage to enemies is unchanged.

## Install

1. Download `Miku-GentleBullets-1.0.0.zip` from this repository.
2. Extract it into your server's `Mods` directory.
3. Check the resulting path is `Mods/ZZZZZ_Miku_GentleBullets/ModInfo.xml`, with `Config/items.xml` beside it in the Config folder.
4. Save the world and restart the server. Reconnect clients after the restart.

No client download or DLL is required. For single-player, use the game's local Mods directory and restart the game.

## Compatibility and scope

- Built for 7 Days to Die V3.2 (b10), with Project Z 3.2.1 / AEC compatibility checks.
- Checked against 48 vanilla and Project Z firearm actions, including Eraser and legendary variants.
- The mod loaded on a dedicated server without XML patch errors. Exact in-game damage has not yet been independently verified.
- Explosions, launchers, melee weapons, mining tools and secondary fire effects are not changed.
- Placed robotic turret behaviour has not been verified separately.
- Other mods that replace firing actions or alter damage calculations may affect the result.

## How it works

The XML patch sets material-specific `DamageBonus` multipliers to zero for supported ranged firearm actions. In the checked game version, ordinary eligible block impacts are then clamped to the engine minimum of 1 HP. This is not a general player block-damage setting and does not edit base game or modpack files.

## Remove

Remove the `ZZZZZ_Miku_GentleBullets` folder and restart the server.

Version: 1.0.0
