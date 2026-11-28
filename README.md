<div align="center">

<img src="favicon.svg" alt="Wonder Invoice logo" width="96" height="96" />

# 🧾 Wonder Invoice

### Create. Send. Get Paid.

**Free GST invoices, quotations, credit notes and payment receipts for Indian freelancers, creators and small businesses.**

<br />

[![Live Demo](https://img.shields.io/badge/🚀_LIVE_DEMO-invoice.wondermayank.in-573AFC?style=for-the-badge)](https://invoice.wondermayank.in/)
[![No Sign-up](https://img.shields.io/badge/NO_SIGN--UP-REQUIRED-2ea44f?style=for-the-badge)](https://invoice.wondermayank.in/)
[![Privacy](https://img.shields.io/badge/DATA_STAYS-ON_YOUR_DEVICE-0A84FF?style=for-the-badge)](#-privacy)

[![Website](https://img.shields.io/badge/🌐_WONDERMAYANK.IN-1f2937?style=for-the-badge)](https://wondermayank.in/)
[![Contact](https://img.shields.io/badge/✉️_CONTACT-1f2937?style=for-the-badge)](https://wondermayank.in/contact)
[![GitHub](https://img.shields.io/badge/GITHUB-wondermayank-181717?style=for-the-badge&logo=github)](https://github.com/wondermayank)

<br />

⭐ **If this helps you, please star the repo!** ⭐

</div>

---

## ✨ What you can create

| | Document | Use it for |
| :-: | --- | --- |
| 🧾 | **GST Tax Invoice** | Bill clients with GST details in minutes |
| 📝 | **Quotation** | Send a price offer before the work starts |
| ↩️ | **Credit Note** | Adjust or cancel a previous invoice |
| 💵 | **Payment Receipt** | Confirm that you got paid |

## 🔒 Privacy

- 🧠 All data is saved in your own browser (**IndexedDB**)
- 🚫 **No backend, no database, no sign-up** on the live site
- ☁️ Hosting your own copy? You can add your own Supabase for cloud sync (see below)

## 🗂️ What is in this repo

This is a **static site** (a compiled build). There is nothing to install or build.

```text
index.html                 entry page, meta tags, links the files below
assets/index-wi1.js        the whole app (compiled)
assets/index-DymxpHNi.css  base styles
assets/wonder-1.css        Wonder Invoice theme: dock, header, footer, FAQ
favicon.svg, manifest.webmanifest, robots.txt, sitemap.xml
vercel.json                headers + caching for Vercel
_headers                   headers + caching for Cloudflare Pages
```

The app uses hash routing (`/#/invoices`), so every page works on a plain static host with no rewrite rules.

## 🖥️ Run it locally

```bash
git clone https://github.com/wondermayank/wonderinvoice.git
cd wonderinvoice
python -m http.server 8000
```

Then open `http://localhost:8000`. Any static file server works.

## 🚀 Deploy

<details>
<summary><b>☁️ Cloudflare Pages</b></summary>

1. Push this folder to a GitHub repo.
2. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → connect the repo.
3. Framework preset: **None**. Build command: *(leave empty)*. Build output directory: `/`
4. Deploy, then **Custom domains** → add your domain.

</details>

<details>
<summary><b>▲ Vercel</b></summary>

1. Push this folder to a GitHub repo.
2. Vercel → **Add New** → **Project** → import the repo.
3. Framework preset: **Other**. Build command: *(empty)*. Output directory: `.`
4. Deploy, then **Settings → Domains** → add your domain.

</details>

## ✏️ Editing

The app is compiled, so most text lives inside `assets/index-wi1.js` as plain strings. Search for the text you want to change and edit it in place. If you change that file, rename it (for example `index-wi2.js`) and update `index.html`, because `/assets/*` is cached for a year. Colours and layout live in `assets/wonder-1.css`.

## ☁️ Host it yourself and add your own Supabase

Want accounts and cloud sync on your own copy? Use **your own** Supabase project:

1. Create a free project at [supabase.com](https://supabase.com/).
2. Copy your **Project URL** and **anon (public) key** from *Project Settings → API*.
3. Put them in the app where the Supabase URL and key are set (search for `supabase` in `assets/index-wi1.js`).
4. Turn on **Row Level Security** for your tables so users can only see their own data.
5. Redeploy your site.

> ⚠️ Only use the **anon public key** in this app. Never put your `service_role` key in a public repo or in browser code.

## 📜 License

Dual-licensed under either of:

- [MIT License](LICENSE-MIT)
- [Apache License 2.0](LICENSE-APACHE)

at your option. You must **keep the copyright notice and license** in every copy, and the [NOTICE](NOTICE.md) file if you use Apache-2.0.

If you use or fork this project, please give credit:

> Based on [Wonder Invoice](https://github.com/wondermayank/wonderinvoice) by [Wondermayank](https://wondermayank.in/)

## 📬 Contact

[![Website](https://img.shields.io/badge/WEBSITE-wondermayank.in-573AFC?style=for-the-badge)](https://wondermayank.in/)
[![Contact](https://img.shields.io/badge/CONTACT-wondermayank.in/contact-1f2937?style=for-the-badge)](https://wondermayank.in/contact)

<div align="center">

Made with ❤️ in India by **[Wondermayank](https://wondermayank.in/)**

</div>
