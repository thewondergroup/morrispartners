# morris.partners

Static landing page for Morris Partners, served by GitHub Pages.

## Files

- `index.html` — the whole page (styles and scripts inline; fonts from Google Fonts)
- `assets/` — project photos, the Shard video loop and its poster frame
- `CNAME` — tells GitHub Pages to serve the site at `morris.partners`
- `.nojekyll` — serve files as-is

## Deploy

1. Create a new repository (e.g. `thewondergroup/morris-partners`) and upload everything in this folder to the root of the `main` branch — including the hidden `.nojekyll` file.
2. Repository → Settings → Pages → Source: **Deploy from a branch**, Branch: **main**, folder **/ (root)** → Save.
3. Settings → Pages → Custom domain: `morris.partners` → Save (the CNAME file pre-fills this).
4. Set the DNS records below at the domain's DNS provider.
5. Once the DNS check passes, tick **Enforce HTTPS** (can take up to an hour or so to become available).

## DNS records for morris.partners

| Type  | Host / Name | Value                  |
|-------|-------------|------------------------|
| A     | @           | 185.199.108.153        |
| A     | @           | 185.199.109.153        |
| A     | @           | 185.199.110.153        |
| A     | @           | 185.199.111.153        |
| AAAA  | @           | 2606:50c0:8000::153    |
| AAAA  | @           | 2606:50c0:8001::153    |
| AAAA  | @           | 2606:50c0:8002::153    |
| AAAA  | @           | 2606:50c0:8003::153    |
| CNAME | www         | thewondergroup.github.io |

Remove any existing A / AAAA records on `@` and any `www` record pointing at Wix.
**Do not touch MX, SPF/DKIM (TXT) or other mail records** — they keep contact@morris.partners working.

## Editing

Text lives directly in `index.html`. Search for the line you want to change, edit, commit — GitHub Pages republishes in about a minute.
