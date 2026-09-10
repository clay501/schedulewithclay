# schedulewithclay

Static booking pages for Clay Klaus-Wade, served with GitHub Pages.

- `/` — all booking links
- `/meet/` — virtual meetings
- `/therapy/` — therapy sessions (existing clients)
- `/medicare/` — Medicare consultations

## Deploy

Copy the contents of this folder to the repository root on `main`, then in
**Settings → Pages** set Source to *Deploy from a branch*, branch `main`, folder `/ (root)`.

Everything is plain HTML plus one stylesheet (`styles.css`); no build step.

## Custom domain (schedulewithclay.link, registered at Porkbun)

1. Push these files to the repo root on `main` (including `CNAME`).
2. **Settings → Pages** → Source: *Deploy from a branch*, `main`, `/ (root)`.
3. **Settings → Pages → Custom domain**: `schedulewithclay.link` → Save.
4. In Porkbun DNS, delete the parking/ALIAS records, then add:
   - A  @  185.199.108.153
   - A  @  185.199.109.153
   - A  @  185.199.110.153
   - A  @  185.199.111.153
   - CNAME  www  clay501.github.io
5. Wait for DNS to propagate (minutes to a few hours), then tick **Enforce HTTPS**.
