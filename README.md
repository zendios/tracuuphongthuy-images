# tra cứu PHONG THỦY — images

Image assets for the Zendios app *tra cứu PHONG THỦY* (Android / iOS / web).
The app bundles only the small thumbnails; full-size images are loaded on demand from this repository via jsDelivr.

## Layout

| Folder | Content | Size |
|---|---|---|
| `articles/full/` | Full-size article images (Knowledge, Tips, Vietnamese feng shui history) | 1200 px on the long side, JPEG |
| `articles/thumb/` | Thumbnails, also bundled inside the app as offline fallback | 432 × 270, JPEG |

File names are shared with the app (`src/data/anh.js`), e.g. `52-am-duong-trong-kien-truc.jpg`.

## URLs used by the app

- Primary: `https://cdn.jsdelivr.net/gh/zendios/tracuuphongthuy-images@<tag>/articles/full/<file>`
- Fallback: `https://raw.githubusercontent.com/zendios/tracuuphongthuy-images/<tag>/articles/full/<file>`

Every change is published under a new tag (`v1`, `v2`, …) so old app versions keep working and caches stay correct.
Never rename or delete a file inside a published tag.

## Licenses

- Images marked "Zendios · AI" in `ATTRIBUTION.md` are AI-generated illustrations, © Zendios, for use in the app.
- Real photos come from Wikimedia Commons and keep their original licenses (CC BY, CC BY-SA, CC0, public domain);
  author, license and source page for each file are listed in `ATTRIBUTION.md`.
