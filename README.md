# True Match Coatings — Website

This repo holds the public website only — no business documents, formulas, or
trade-secret content. That stays in the separate private `TrueMatchCoatings`
repo. Keeping this one public and clean is intentional: it's what lets GitHub
Pages host it for free.

## Deploying

1. Push this repo's contents to a **new public** GitHub repo (e.g.
   `true-match-coatings-website`).
2. On GitHub: Settings → Pages → Source → "Deploy from a branch" → `main` /
   `/ (root)` → Save.
3. Still on that page, under "Custom domain," enter `truematchcoatings.com`
   and Save. (The `CNAME` file in this repo already has this domain in it,
   which GitHub reads automatically — the Settings field just needs to match.)
4. At Namecheap, in the domain's Advanced DNS panel, add:
   - Four **A** records, Host `@`, pointing to:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME** record, Host `www`, pointing to `jrosiere.github.io`
5. DNS can take up to 24 hours to propagate. Once GitHub shows the domain as
   verified, check "Enforce HTTPS" in the Pages settings — the SSL
   certificate can take a bit to provision after that, so don't panic if it's
   not instant.

## Updating content

Edit `index.html` directly, or hand new content/design direction to Claude
to rebuild it — this is a plain static HTML/CSS file, no build step required.
