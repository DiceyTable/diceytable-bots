# Credits — Sakura Sentinel (`japanese-white-samurai-sakura`)

These map onto `assetCreditSchema` for the import credit gate. The app stamps `id`,
`recordedAt` and `attestation`; you type `signedName` at import.

The textures are **embedded** in the GLBs, and `manifest.credits` refuses two records that claim
the same path. So each GLB gets **one** `own-work` record, and the third-party attribution goes
in `notes`, the only field that survives on `own-work`. (Shipping the textures as separate
files would allow a clean `third-party` record per texture set, at the cost of more files.)

Authors were re-queried from the exact assets shipped (by `assetBaseId`) on 2026-09-27, and every
`asset-gallery-detail` URL returned 200.

## Credit 1 — the model

| Field | Value |
| --- | --- |
| `origin` | `own-work` |
| `paths` | `bots/japanese-white-samurai-sakura/japanese-white-samurai-sakura.glb`, `bots/japanese-white-samurai-sakura/japanese-white-samurai-sakura.web.glb` |
| `title` | Sakura Sentinel bot model |
| `notes` | Modelled procedurally in Blender 5.2 (build_japanese-white-samurai-sakura.py). The per-plate lacquer atlas (seigaiha engraving, hairline seams, edge wear, the painted plum branches) and the honeycomb glow mask are own work, painted by make_textures_japanese-white-samurai-sakura.py. Contains re-tinted texture maps from four BlenderKit materials, all under the BlenderKit Royalty Free licence: "White painted scratched metal" by ydd 3D (https://www.blenderkit.com/asset-gallery-detail/04aa72d5-0bf4-4e4a-88d4-a6be9c423830/), "Antique Bronze Metal" by KID (https://www.blenderkit.com/asset-gallery-detail/befa6fa2-4400-46dd-8fbf-1ef26f2fac0b/), "Dark Gunmetal" by KID (https://www.blenderkit.com/asset-gallery-detail/a0963816-297c-4988-b4f6-92dfaf662efe/) and "Dark Brushed Silver Metal" by KID (https://www.blenderkit.com/asset-gallery-detail/8b1ca640-26af-4261-bf78-14415d0ed99b/). |
| `signedName` | *(typed at import)* |

> **Sakura Sentinel bot model — original work by the mod author**

## Third-party materials (for reference)

| Material | Creator | Licence | Used on | Maps |
| --- | --- | --- | --- | --- |
| [White painted scratched metal](https://www.blenderkit.com/asset-gallery-detail/04aa72d5-0bf4-4e4a-88d4-a6be9c423830/) | ydd 3D | Royalty Free (BlenderKit) | `Bot_Lacquer` | base colour (re-tinted warm white), roughness, under the own-work lacquer atlas |
| [Antique Bronze Metal](https://www.blenderkit.com/asset-gallery-detail/befa6fa2-4400-46dd-8fbf-1ef26f2fac0b/) | KID | Royalty Free (BlenderKit) | `Bot_Brass` | base colour (re-tinted champagne), roughness, normal — 512 px |
| [Dark Gunmetal](https://www.blenderkit.com/asset-gallery-detail/a0963816-297c-4988-b4f6-92dfaf662efe/) | KID | Royalty Free (BlenderKit) | `Bot_Graphite` | base colour (re-tinted graphite), roughness, normal — 512 px |
| [Dark Brushed Silver Metal](https://www.blenderkit.com/asset-gallery-detail/8b1ca640-26af-4261-bf78-14415d0ed99b/) | KID | Royalty Free (BlenderKit) | `Bot_DarkSteel` | base colour (re-tinted dark steel), roughness, normal — 512 px |

`Bot_RedLacquer`, `Bot_BlackLacquer`, `Bot_Cord` and `Bot_Glow_Primary` are hand-authored (flat
colours, or the own-work glow mask); they carry no third-party content.

The store renders were lit with Poly Haven's `studio_small_09` HDRI (CC0). It is not shipped.
