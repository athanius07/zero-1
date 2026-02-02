
# Zero/Low-Emissions Equipment Site — Drop-in Update

This package contains the updated **blue/white UI**, **power-type color badges**, **top summary**, **pagination**, and **CSV export (filtered/full)**, plus a **seed dataset**. Replace the files in your repo and commit.

## Quick install

1. Extract this ZIP.
2. Copy **all files** into your repo root (e.g., `zero-1/`), overwriting existing files:
   - `index.html`
   - `assets/css/styles.css`
   - `assets/js/app.js`
   - `data/equipment.json` (contains seed entries — you can replace later with 100+)
   - `netlify.toml`, `404.html`
3. Commit and push a branch, then open a PR.

```bash
git checkout -b feat/ui-and-seed
cp -R ./zero1-package/* ./
git add -A
git commit -m "feat(ui): blue theme, power badges, summary, pagination; csv filtered/full; seed data"
git push -u origin feat/ui-and-seed
```

## Notes
- Add more machines by editing `data/equipment.json`.
- Fields: `Machine Name`, `Power Type`, `OEM`, `Country of Origin`, `Class (tons)`, `Engine / Motor Power`, `Bucket Size (excavator/wheel loader)`, booleans for machine types, `Year of Release`, `Status`, `Source Link`, `Source Date`, `Notes`.
- Power badges support **Battery Electric**, **Hydrogen Fuel Cell**, **Hydrogen ICE**, **Diesel Hybrid**, **Methanol**, and **Other** (multi-valued supported).

## Next
- I will follow up with a PR to expand `data/equipment.json` to **100+ machines** with citations and consistent statuses.
