# Credits — Pebble (`generic-smooth-minimal`)

These map onto `assetCreditSchema` for the import credit gate. The app stamps `id`,
`recordedAt` and `attestation`; you type `signedName` at import.

The textures are **embedded** in the GLBs, and `manifest.credits` refuses two records that claim
the same path. So each GLB gets **one** `own-work` record, and the third-party attribution goes
in `notes`, the only field that survives on `own-work`.

## Credit 1 — the model

| Field | Value |
| --- | --- |
| `origin` | `own-work` |
| `paths` | `bots/generic-smooth-minimal/generic-smooth-minimal.glb`, `bots/generic-smooth-minimal/generic-smooth-minimal.web.glb` |
| `title` | Pebble bot model |
| `notes` | Modelled procedurally in Blender 5.2 (build_generic-smooth-minimal.py). Contains roughness maps baked from "Off White Plastic Glossy" and "Black Plastic Glossy", both by L Carter, BlenderKit Royalty Free licence: https://www.blenderkit.com/asset-gallery-detail/0e142031-72c0-4113-abd7-e59d8fa4c45f/ and https://www.blenderkit.com/asset-gallery-detail/d62f4845-174a-42a4-88d4-a3e09d788877/ . Base colours are hand-set factors. |
| `signedName` | *(typed at import)* |

> **Pebble bot model — original work by the mod author**

The preview renders were lit with Poly Haven's `studio_small_09` HDRI (CC0). It is not shipped.
