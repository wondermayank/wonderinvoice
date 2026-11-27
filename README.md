# Wonder Invoice

Free GST invoices, quotations, credit notes and payment receipts for Indian freelancers, creators
and small businesses. Live at **https://invoice.wondermayank.in**.

All data stays in the visitor's browser (IndexedDB). There is no backend, no database and no sign-up.

## What is in this folder

This is a **static site** (a compiled build). There is nothing to install or build.

```
index.html                 entry page, meta tags, links the files below
assets/index-wi1.js        the whole app (compiled)
assets/index-DymxpHNi.css  base styles
assets/wonder-1.css        Wonder Invoice theme: dock, header, footer, FAQ
favicon.svg, manifest.webmanifest, robots.txt, sitemap.xml
vercel.json                headers + caching for Vercel
_headers                   headers + caching for Cloudflare Pages
```

The app uses hash routing (`/#/invoices`), so every page works on a plain static host with no
rewrite rules.

## Deploy on Cloudflare Pages

1. Push this folder to a GitHub repo.
2. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → connect the repo.
3. Framework preset: **None**. Build command: *(leave empty)*. Build output directory: `/`
4. Deploy, then **Custom domains** → add `invoice.wondermayank.in`.

## Deploy on Vercel

1. Push this folder to a GitHub repo.
2. Vercel → **Add New** → **Project** → import the repo.
3. Framework preset: **Other**. Build command: *(empty)*. Output directory: `.`
4. Deploy, then **Settings → Domains** → add `invoice.wondermayank.in`.

## Editing

The app is compiled, so most copy lives inside `assets/index-wi1.js` as plain strings. Search for the
text you want to change and edit it in place. If you change the file's contents, rename it
(for example `index-wi2.js`) and update `index.html`, because `/assets/*` is cached for a year.
Colours and layout live in `assets/wonder-1.css`.

## Cloud sync is switched off

The original build shipped with another person's Supabase project baked in. That has been removed, so
nothing leaves the visitor's device and the privacy policy is accurate. If you ever want accounts and
sync, create your own Supabase project and wire in your own URL and key.

## Licence

See `NOTICE.md`.
