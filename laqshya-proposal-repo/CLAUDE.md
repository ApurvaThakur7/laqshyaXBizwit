# Project conventions — for Claude Code

This is a static, versioned proposal site for **Laqshya Media Group**, prepared by **Bizwit AI**. No framework, no build step. Plain HTML/CSS/JS, one self-contained file per version.

## Brand (match exactly — this mirrors laqshyagroup.com)

- Background: pure black `#000000`; surfaces `#0F0F10`; borders `#242427`
- Text: white `#FFFFFF`; muted `#9A9AA0`
- Accent (the single brand colour): red `#ED1C24` (hover `#FF2D35`)
- Display/headline font: **Archivo** (700–900), UPPERCASE, tight letter-spacing
- Logo wordmark font: **Jost**; body font: **Inter**
- Signature motif: a red **target/reticle** (Laqshya = "target/aim"); logo is `LAQSHYA` with a red dot inside the `Q`
- All colours are CSS variables in `:root` — change the brand by editing variables, not scattered values.

## Structure

- `index.html` — the version hub. Lists every version, marks the newest as **Latest**.
- `vN/index.html` — a full, self-contained proposal for version N. Footer shows `vN.0`.
- `CHANGELOG.md` — newest entry on top.

## Content = the 14 requirements

Four pillars: **A** Knowledge & Enablement (R1–R4), **B** Core Operations (R5–R8), **C** Growth & Creative (R9–R11), **D** Enterprise Expansion (R12–R14). Only **R7 (Proof of Play & Client Portal)** is a code-based build; most others are low-code AI automation. Keep the cost-efficient hybrid framing and the reference to Laqshya's existing **SHARP** planner.

## Rules when editing

1. Keep every version file self-contained (inline CSS/JS; no external deps except Google Fonts). No localStorage/sessionStorage.
2. Never break the four-pillar / R1–R14 mapping.
3. Commercials stay as structure only — no rupee figures — unless explicitly told otherwise.

## When asked to "cut a new version" (e.g. v2)

1. `cp -r v<latest> v<new>`
2. In `v<new>/index.html`, bump the footer version number and apply the requested changes.
3. Update `index.html` (hub): new version = **Latest**, previous moves down and stays linkable.
4. Add a `CHANGELOG.md` entry at the top with the date and bullet changes.
5. `git add . && git commit -m "vX.0 — <summary>" && git push` (this triggers the Netlify deploy).

## Deploy

Continuous deploy via Netlify (config in `netlify.toml`). A push to `main` is a deploy. After making changes, commit and push unless told to hold.
