# Credits — Rune Warden (`vikings-horned-knotwork`)

These map onto `assetCreditSchema` for the import credit gate. The app stamps `id`,
`recordedAt` and `attestation`; you type `signedName` at import.

The textures are **embedded** in the GLBs, and `manifest.credits` refuses two records that claim
the same path. So each GLB gets **one** `own-work` record, and the third-party attribution goes
in `notes`, the only field that survives on `own-work`. (Shipping the textures as separate
files would allow a clean `third-party` record per texture set, at the cost of more files.)

Authors were re-queried from the exact assets shipped (by `assetBaseId`) at credit-writing time,
and every `asset-gallery-detail` URL returned 200.

## Credit 1 — the model

| Field | Value |
| --- | --- |
| `origin` | `own-work` |
| `paths` | `bots/vikings-horned-knotwork/vikings-horned-knotwork.glb`, `bots/vikings-horned-knotwork/vikings-horned-knotwork.web.glb` |
| `title` | Rune Warden bot model |
| `notes` | Modelled procedurally in Blender 5.2 (build_vikings-horned-knotwork.py). The knotwork, rune and serpent carvings, plank shading, paint wear and glow mask are own work, painted by make_textures_vikings-horned-knotwork.py; the runes are Elder Futhark signs from Noto Sans Runic (Google, SIL Open Font License 1.1, https://fonts.google.com/noto/specimen/Noto+Sans+Runic), rendered into the textures (the font is not shipped). Contains re-tinted texture maps from six BlenderKit materials, all under the BlenderKit Royalty Free licence: "Antique Bronze Metal" by KID (https://www.blenderkit.com/asset-gallery-detail/befa6fa2-4400-46dd-8fbf-1ef26f2fac0b/), "White painted scratched metal" by ydd 3D (https://www.blenderkit.com/asset-gallery-detail/04aa72d5-0bf4-4e4a-88d4-a6be9c423830/), "Rusty Dark Metal" by Sebastian Joseph (https://www.blenderkit.com/asset-gallery-detail/42b16482-a05b-497a-b7cb-373e69c02f3c/), "Polished Walnut Wood" by Vaishakh Vinod (https://www.blenderkit.com/asset-gallery-detail/46de7336-6072-4b85-8b99-ac2438829a08/), "Dark Gunmetal" by KID (https://www.blenderkit.com/asset-gallery-detail/a0963816-297c-4988-b4f6-92dfaf662efe/) and "Dark Brushed Silver Metal" by KID (https://www.blenderkit.com/asset-gallery-detail/8b1ca640-26af-4261-bf78-14415d0ed99b/). |
| `signedName` | *(typed at import)* |

> **Rune Warden bot model — original work by the mod author**

## Third-party materials (for reference)

| Material | Creator | Licence | Used on | Maps |
| --- | --- | --- | --- | --- |
| [Antique Bronze Metal](https://www.blenderkit.com/asset-gallery-detail/befa6fa2-4400-46dd-8fbf-1ef26f2fac0b/) | KID | Royalty Free (BlenderKit) | `Bot_Bronze` | base colour (re-tinted darker), roughness, normal — 512 px |
| [White painted scratched metal](https://www.blenderkit.com/asset-gallery-detail/04aa72d5-0bf4-4e4a-88d4-a6be9c423830/) | ydd 3D | Royalty Free (BlenderKit) | `Bot_Ivory` | base colour (re-tinted off-white), roughness, under the own-work engraving atlas |
| [Rusty Dark Metal](https://www.blenderkit.com/asset-gallery-detail/42b16482-a05b-497a-b7cb-373e69c02f3c/) | Sebastian Joseph | Royalty Free (BlenderKit) | `Bot_Strap` | base colour (re-tinted brown), roughness, normal — 512 px |
| [Polished Walnut Wood](https://www.blenderkit.com/asset-gallery-detail/46de7336-6072-4b85-8b99-ac2438829a08/) | Vaishakh Vinod | Royalty Free (BlenderKit) | `Bot_Wood` | base colour (re-tinted, rotated along the planks), roughness, under the own-work carving |
| [Dark Gunmetal](https://www.blenderkit.com/asset-gallery-detail/a0963816-297c-4988-b4f6-92dfaf662efe/) | KID | Royalty Free (BlenderKit) | `Bot_Iron` | base colour (re-tinted charcoal), roughness, normal — 512 px |
| [Dark Brushed Silver Metal](https://www.blenderkit.com/asset-gallery-detail/8b1ca640-26af-4261-bf78-14415d0ed99b/) | KID | Royalty Free (BlenderKit) | `Bot_Steel` | base colour (re-tinted pewter), roughness, normal — 512 px |
| [Noto Sans Runic](https://fonts.google.com/noto/specimen/Noto+Sans+Runic) | Google (Noto project) | SIL OFL 1.1 | `Bot_Ivory`, `Bot_Glow_Primary` | rune signs rendered into the atlases |

The store renders were lit with Poly Haven's `studio_small_09` HDRI (CC0). It is not shipped.
