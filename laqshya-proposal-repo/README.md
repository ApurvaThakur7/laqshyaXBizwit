# Laqshya × Bizwit AI — Proposal Site

A static, versioned proposal site. `index.html` is the version hub; each version lives in its own folder (`/v1`, `/v2`, ...). Deployed on Netlify with continuous deploy: **every push to `main` updates the live link automatically.**

---

## One-time setup (about 10 minutes)

### 1. Put this on GitHub

From inside this folder:

```bash
git init
git add .
git commit -m "v1.0 — first draft"
git branch -M main
```

Create an empty repo on GitHub (no README), then:

```bash
git remote add origin https://github.com/<you>/laqshya-proposal.git
git push -u origin main
```

### 2. Connect Netlify (continuous deploy)

1. app.netlify.com → **Add new site → Import an existing project → GitHub**
2. Pick the `laqshya-proposal` repo.
3. Build settings come from `netlify.toml` (no build command, publish = repo root). Just click **Deploy**.
4. You get a live URL like `laqshya-proposal.netlify.app`. Rename it under **Site configuration → Change site name** if you want something cleaner.

That's it. From now on, any push to `main` redeploys the same URL in ~30–60s.

### 3. Install Claude Code

```bash
npm install -g @anthropic-ai/claude-code   # needs Node 18+
```

Then, inside this folder:

```bash
claude
```

Sign in with your Claude account on first run.

---

## Daily loop (the part you wanted)

Inside this folder, run `claude` and just say what to change, for example:

> "Make the hero headline smaller, change the brand red to #E4002B, then commit and push."

Claude Code edits the files and runs the git commit + push itself. Netlify sees the push and redeploys the live link automatically. Refresh the URL to see it.

If you prefer to push manually:

```bash
git add . && git commit -m "tweak hero" && git push
```

---

## Making a new version

Keep old versions viewable while iterating:

1. Copy the latest version folder: `cp -r v1 v2`
2. Edit `v2/index.html` (bump the footer to `v2.0`).
3. Update `index.html` (the hub) — mark v2 as **Latest**, move v1 down.
4. Add a `CHANGELOG.md` entry at the top.
5. Commit and push.

Both `/v1` and `/v2` stay live at the same site. Netlify also keeps a permalink for every past deploy automatically, so nothing is ever lost.

(See `CLAUDE.md` — Claude Code reads it and will follow these conventions for you, so you can just say "cut a v2 with these changes".)

---

## Files

```
index.html      Version hub (links to every version)
v1/index.html   Proposal, v1.0
CHANGELOG.md     What changed per version
netlify.toml     Netlify build config (no build, publish root)
CLAUDE.md        Project conventions for Claude Code
.gitignore
```
