# Many Many Many Mods Modularized - Rebalances - Traits

Trait rebalances, and which traits ideoligion memes like or dislike.

Split out of Too Many Mods (Wara.toomanymods) via the single MMMM_Rebalances project on 2026-10-13. Values are the original
author's tuning; nothing here is a compatibility fix (see Convergence) or a cross-mod content join (see Integrations).

## Layout
- `1.7/` is a copy of `1.6/` and `<v1.7>` mirrors `<v1.6>` in `loadFolders.xml`; change both when editing a patch.
- `1.6/Patches`, `1.6/Defs`: always loaded; each block is gated inside on the mods it touches (`MayRequire`).
- `1.6/Mods/<Name>`: loads only when that mod is active (`loadFolders.xml`).
- `1.6/Without/<Name>` and `1.6/Mods/<X>_Without<Y>`: load only while the named mod is NOT active.

## Always-loaded files
- `Patches/AgreeingMemes.xml`
- `Patches/TraitRebalance.xml`

## Gated folders
- `AlteredCarbon`
- `BigAndSmallGenesAndMore`
- `RimpsycheDisposition`
- `VanillaIdeologyExpandedMemesAndStructures`
