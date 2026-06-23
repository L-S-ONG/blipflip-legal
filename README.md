# Blipflip — public legal site

This folder is a tiny, self-contained GitHub Pages site that hosts **only** the
public legal pages (privacy policy + terms). It exists so the main `blipflip`
app repo can stay **private** while these pages are reachable at a public URL for
the Google Play listing.

## Publish it (one time)

Create a new **public** repo named `blipflip-legal`, then push this folder's
contents to it:

```sh
# from a copy of this folder (not nested inside the private repo)
git init
git add .
git commit -m "Blipflip legal pages"
git branch -M main
git remote add origin https://github.com/L-S-ONG/blipflip-legal.git
git push -u origin main
```

Then enable Pages: repo **Settings → Pages → Source: Deploy from a branch →
Branch `main`, folder `/ (root)` → Save**.

Your URLs (after ~1 min):

- `https://l-s-ong.github.io/blipflip-legal/PRIVACY_POLICY.html` ← paste into Play
- `https://l-s-ong.github.io/blipflip-legal/TERMS_OF_SERVICE.html`

## Keep in sync

The canonical copies live in the private repo at `docs/PRIVACY_POLICY.md` and
`docs/TERMS_OF_SERVICE.md`. When you change a policy there, copy the new body into
the matching file here (keep the `---` front matter at the top) and push.
