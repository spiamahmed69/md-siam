# Md Siam — SP Siam Ahmed | Portfolio Website

Personal portfolio website for **Md Siam**, known on social media as **SP Siam Ahmed** — Full Stack Web Developer from Bangladesh.

Live: https://spiamahmed69.github.io/md-siam/

## Files

- `index.html` — the whole site: hero, about, skills, 12 real projects, experience, education, services, contact
- `assets/mdsiam.jpg` — portrait photo (29 KB JPEG)
- `robots.txt`, `sitemap.xml`, `llms.txt` — SEO files

## Design

Built with two skills (2026-11-26):

- **UI/UX Pro Max** (`design-system/md-siam/MASTER.md`) — Brutalism style,
  monochrome + blue accent (#2563EB), Archivo headings / Space Grotesk body,
  scroll progress bar, chapter mini-CTAs, visible focus states,
  `prefers-reduced-motion` support, all text contrast ≥ 4.5:1.
- **Claude SEO** — static HTML (all content in the first response), meta
  description (154 chars), Open Graph + Twitter cards with image dimensions,
  canonical URL, Person JSON-LD, robots.txt, sitemap.xml, llms.txt, and a
  plain-text FAQ section (no FAQPage schema — Google retired FAQ rich
  results in May 2026).

## SEO — better than the reference site (mdsiam.pro.bd)

That site is a client-rendered React SPA: its first HTML is 477 bytes with an
empty `#root`, it has no meta description, no Open Graph tags, no canonical,
no JSON-LD schema, no robots.txt and no sitemap.xml. This site fixes all of
that:

- Plain static HTML — all content is in the first HTML response, no JavaScript needed to read it
- Meta description, Open Graph + Twitter cards, canonical URL
- Person JSON-LD schema (name, jobTitle, sameAs profiles)
- robots.txt + sitemap.xml (submit the sitemap in Google Search Console)
- llms.txt for AI search
- Small and fast: one 29 KB photo, no framework JS bundle, no web fonts to download

## Deploy (GitHub Pages)

1. Push this folder to a GitHub repo named `md-siam` (branch `main`).
2. In the repo: Settings → Pages → Deploy from a branch → `main` / `/ (root)` → Save.
3. The site goes live at `https://<username>.github.io/md-siam/`.
4. If the site is hosted on a different domain, update the canonical URL,
   the Open Graph URLs, the JSON-LD `url`/`image`, `robots.txt` and
   `sitemap.xml` to that domain.
