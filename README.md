# Cat Set Go — Website

The website for [catsetgo.co.uk](https://catsetgo.co.uk) — cat sitting in West London. 🐾

One static page, no build step, no frameworks. `index.html` is the whole site.

## What's in here

| File | What it is |
|---|---|
| `index.html` | The entire website (HTML + CSS + a little JS, all in one file) |
| `CNAME` | Tells GitHub Pages to serve the site at catsetgo.co.uk |
| `.gitignore` | Keeps junk files out of the repo |

## First-time deployment (one-off, ~20 minutes)

### 1. Put the site on GitHub
1. Create a free account at [github.com](https://github.com) (if you don't have one).
2. Click **New repository** → name it `catsetgo-website` → set it to **Public** → Create.
3. On the empty repo page, click **uploading an existing file** and drag in
   `index.html`, `CNAME` and `.gitignore` from this folder. Commit.

### 2. Turn on GitHub Pages
1. In the repo: **Settings → Pages**.
2. Under *Build and deployment*, set Source to **Deploy from a branch**,
   branch **main**, folder **/ (root)**. Save.
3. After a minute the site is live at `https://YOUR-USERNAME.github.io/catsetgo-website/`.

### 3. Point catsetgo.co.uk at it
1. Still in **Settings → Pages**, under *Custom domain* type `catsetgo.co.uk` and Save.
   (The CNAME file in the repo does the same thing — keep them matching.)
2. Log in at your **domain registrar** (where you bought catsetgo.co.uk) and open its
   DNS settings. Add these records:

   | Type | Name/Host | Value |
   |---|---|---|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | YOUR-USERNAME.github.io |

3. Wait for DNS to update (usually under an hour, can take up to 24h).
4. Back in **Settings → Pages**, tick **Enforce HTTPS** once it becomes available.

Done — https://catsetgo.co.uk is live, free, with a padlock. 🎉

## Making updates later

Small edits can be done entirely in the browser:

1. Open `index.html` in the GitHub repo.
2. Click the ✏️ pencil icon, make your change.
3. Scroll down, write a one-line note about what changed, **Commit changes**.
4. The live site updates itself in about a minute.

Every commit is saved forever, so you can always see what changed when,
and roll anything back.

## House rules (privacy)

- No personal phone number or personal email in this site — contact goes via
  the booking form and Instagram only.
- When `hello@catsetgo.co.uk` exists, there's a ready-made commented-out
  "Email me" button in `index.html` — search for `hello@` and uncomment it.
