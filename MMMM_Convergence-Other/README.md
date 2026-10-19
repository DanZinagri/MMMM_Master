# Many Many Many Mods Modularized - Convergence - Other

The Other part of MMMM Convergence: everything that is not genetics, factions, buildings or items (traits, ideology, thoughts, animals, plants). Split from the single MMMM_Convergence mod (2026-09-29); the one-op Traits and Ideology parts were folded in here.

Overlap removal lifted out of Too Many Mods (Wara.toomanymods): when two mods provide the same thing, one mod's copy is
swapped for the other's and the retired duplicate is handed to Cherry Picker.

## Conventions
- One folder per overlapping pair under `1.6/Mods/<Name>`, gated in `loadFolders.xml` with `IfModActiveAll` on both
  mods. Patches therefore contain **no `PatchOperationFindMod`** checks.
- DLC-only operations carry `MayRequire="Ludeon.RimWorld.<DLC>"` on the `<li>` inside a `PatchOperationSequence`.
- Retired defs are appended to `MMMM_ConvergenceOther_CherryPicker_Basics` (this mod's own list, `1.6/Defs/CherryPicker.xml`)
  and listed in `MMMM_ConvergenceOther_CherryPicker_All` for revival. Cherry Picker itself is optional.

## Contents
| Folder | Overlap | Resolution |
|---|---|---|
| AlphaBiomes | Alpha Biomes glowstool vs vanilla Glowstool | Mycotic Jungle spawns vanilla Glowstool (made to grow in light); AB_Glowstool and, with Progression: Agriculture, its seed bundle and recipes cherry-picked |
| DragonsDescent | Dragons Descent vs vanilla benches / VTE / Ideology | Crown and scale helm stop inheriting recipe benches; hard-scale chemfuel moves to the biofuel refinery; VTE animal haters ignore dragon nuzzles; its rituals use the theist ritual sound |
| TsSamuraiFaction | T's Samurai sake vs Alpha Crafts sake; VIE Bushido vs vanilla Raider | Alpha Crafts' sake and its process removed, every reference moved to T's sake (incl. VFE Factory and FrozenSnowFox fixes); the savage clan requires Bushido instead of Raider |
| BigAndSmallGenesAndMore | B&S giant weapon wielder vs Alpha Genes tough sinews | Trait relabelled and a shared exclusion tag added to the B&S gene and the large body frames |

## To decide
- packageId is a placeholder: `DanZinagri.MMMM.Convergence`.
