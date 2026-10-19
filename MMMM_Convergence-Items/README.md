# Many Many Many Mods Modularized - Convergence - Items

The Items part of MMMM Convergence: items: apparel, weapons, food, drugs and loot. Split from the single MMMM_Convergence mod (2026-09-29).

Overlap removal lifted out of Too Many Mods (Wara.toomanymods): when two mods provide the same thing, one mod's copy is
swapped for the other's and the retired duplicate is handed to Cherry Picker.

## Conventions
- One folder per overlapping pair under `1.6/Mods/<Name>`, gated in `loadFolders.xml` with `IfModActiveAll` on both
  mods. Patches therefore contain **no `PatchOperationFindMod`** checks.
- DLC-only operations carry `MayRequire="Ludeon.RimWorld.<DLC>"` on the `<li>` inside a `PatchOperationSequence`.
- Retired defs are appended to `MMMM_ConvergenceItems_CherryPicker_Basics` (this mod's own list, `1.6/Defs/CherryPicker.xml`)
  and listed in `MMMM_ConvergenceItems_CherryPicker_All` for revival. Cherry Picker itself is optional.

## Contents
| Folder | Overlap | Resolution |
|---|---|---|
| BigAndSmallGeneTools | B&S gene tools listed in two item categories | The seven tools sit only in the Alpha Genes gene tools category, not also in vanilla miscellaneous items |
| RoosMinotaur | Roo's Herculean gene and weapon class vs Big and Small's giant weapon system | The xenotype, eight weapons and the Harrier pawn kind all move to the B&S gene, weapon class and tags; the Herculean gene is cherry-picked |
| AlphaCrafts | Alpha Crafts mayonnaise and oil vs VCE mayo and deep frier fuel | VCE mayo cherry-picked; Alpha Crafts mayos become VCE condiments with ingredient effects; the deep frier burns Alpha Crafts oil |
| TsSamuraiFaction | T's Samurai sake vs Alpha Crafts sake; VIE Bushido vs vanilla Raider | Alpha Crafts' sake and its process removed, every reference moved to T's sake (incl. VFE Factory and FrozenSnowFox fixes); the savage clan requires Bushido instead of Raider |
| DragonsDescent | Dragons Descent vs vanilla benches / VTE / Ideology | Crown and scale helm stop inheriting recipe benches; hard-scale chemfuel moves to the biofuel refinery; VTE animal haters ignore dragon nuzzles; its rituals use the theist ritual sound |
| VanillaGeneticsExpanded | VGE single-tier excavators vs the alpha genome excavator | Dino, megafauna and dragon excavators and recipes cherry-picked once the alpha excavator covers their tiers |

## To decide
- packageId is a placeholder: `DanZinagri.MMMM.Convergence`.
