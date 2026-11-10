# Desert Vision — operating manual for the site repo

Copy this file to the root of `desertvision-site` as `CLAUDE.md`.

Desert Vision is HUMAN_01's (Andrea's) record label and event brand. This repo is the public site,
**www.desertvision.it**. The working plan and current status live in the POST WORK repo:
`postwork/missions/desert-vision/README.md`. Read it at the start of every session and update it before the end.

## Rules
1. **Publishing is human-only.** Agents work on a branch and show a preview. HUMAN_01 merges to `main`
   (merging publishes the site). DNS, hosting, domain and accounts are his.
2. **Public language is English.** Release copy, meta tags, alt text.
3. **Never break live URLs.** `/` and `/releases/<catalog>/` stay stable; shared links on Instagram,
   Beatport and in press must keep working.
4. **Facts come from HUMAN_01 or the stores.** Catalog numbers, dates, credits, tracklists and store links
   are never invented. Missing data stays a visible TODO, not a guess.
5. **Check before you claim it works.** Build the site and compare screenshots (mobile and desktop) before
   saying a page is done.
6. Desert Vision money is outside the POST WORK ledger. Do not log it there.

## Layout (as of 2026-11-10, before the planned Astro move)
- `index.html`: current release (DV010, *Hollow*, Andy's Echo), with inline CSS/JS, JSON-LD `MusicAlbum` and OG tags.
- `releases/dv009/index.html`: archive release page.
- `assets/dv0xx/`: cover (`cover.webp`, `cover-sm.webp`), hero, `og*.jpg` at 1200×630, per release.
- `assets/outline/`: textures; `assets/logo.svg`, `assets/logo.png`.
- `CNAME`: `www.desertvision.it` (GitHub Pages).

## Visual identity (from the current CSS)
Ink `#141311`, deep ink `#0B0A08`, cream `#E9E3D6`, muted cream `#968F82`, line `#2A2823`,
teal `#4A9C8A`, copper `#D98F52`, violet `#7B5EA7`. Fonts: Space Grotesk, Space Mono, Unbounded 800 (display),
Instrument Serif italic, Martian Mono (data). Dark only (`color-scheme: dark`).

## A new release, until the generator exists
Catalog number `DV0xx`, assets in `assets/dv0xx/`, page in `releases/dv0xx/`, the home switches to the new
release, and the previous home content moves to its own `releases/` page. Update JSON-LD, OG and canonical.
