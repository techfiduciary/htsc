# Highest Tribunal Supreme Court — highesttribunal.site

Static rebuild of the highesttribunal.site website (originally built on imcreator), prepared for Cloudflare Pages deployment from this repository.

## Pages

| Path | Source | Notes |
|---|---|---|
| `/` | Wayback capture 2025-01-20 | Patched to live content as of 2026-09-20 (hero wording, "Our Purpose", EO 292, contact block) |
| `/highesttribunal/` | Same document as `/` | Alias served by the original site |
| `/history-and-role/` | Wayback capture 2025-01-20 | Verified identical to live (2026-09-20) |
| `/international-law/` | Wayback capture 2025-03-17 | |
| `/ownership/` | Wayback capture 2025-03-17 | |
| `/peoples-initiative/` | Wayback capture 2025-01-20 | |
| `/royal-decrees/` | Wayback capture 2025-03-17 | |
| `/transition/` | Wayback capture 2025-03-17 | |
| `/west-philippine-sea/` | Wayback capture 2025-01-20 | |
| `/wps/` | Same document as `/west-philippine-sea/` | Alias |

## Asset strategy (same as the actual site)

- **Images**: hotlinked from `lh3.googleusercontent.com` — the exact URLs the live site uses. All 170 unique image URLs verified HTTP 200 on 2026-09-20.
- **CSS/JS**: hotlinked from `www.imcreator.com` (versioned `v=1.6.0f2-noimos`, includes per-page `static_style` sheets). All 16 asset URLs verified HTTP 200 on 2026-09-20.

## Deploy

Cloudflare Pages → connect this repository → build command: none → output directory: `/` (repo root).

## Open items

- `/charter-change` and `/highesttribunalsupremecourt` are referenced by older site artifacts but could not be verified live; neither is linked from current navigation. If either exists on the live site, capture and add a folder for it.
- The homepage rebuild is a faithful reconstruction from rendered live content (the live server blocks raw fetches from this network); compare against the live homepage after deploy and adjust wording/sections as needed.

## Working files

Archived source captures and text extractions live outside this repo in `_source/` (not deployed).
