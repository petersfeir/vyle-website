# VYLE website

Static one-page site for vylelb.com. No build step: the repository root is the public folder.

## Updating content

- **Brands counter:** change `data-to` on `#helped` in `index.html`.
- **Portfolio:** each piece has four files in `assets/work/`: `pNN.mp4` (full video with sound, 720x1280), `pNN-p.mp4` (6 s silent preview, 540x960), `pNN.webp` (cover, 540x960) and `pNN-s.webp` (small cover, 300 wide). Add a row to `WORK` in the script: id, title, service, short line, filter (`products`, `worlds`, `ads` or `edits`). Mark pieces made with other brands' products as "Concept".
- **Deploy:** pushing to `main` publishes the site through `.github/workflows/static.yml`.
