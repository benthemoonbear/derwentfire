# Derwent Fire Compliance website

Static website for [Derwent Fire Compliance](https://www.derwentfirecompliance.co.uk), independent fire risk assessors based in Belper, Derbyshire.

## Pages

| Path | Page |
|---|---|
| `/` | Homepage |
| `/fire-warden-training/` | Fire warden training |
| `/hmo-fire-risk-assessment/` | HMO fire risk assessments |
| `/holiday-let-fire-risk-assessment/` | Holiday let fire risk assessments |
| `/fire-risk-assessment-derbyshire/` | Derbyshire |
| `/fire-risk-assessment-staffordshire/` | Staffordshire |
| `/fire-risk-assessment-nottinghamshire/` | Nottinghamshire |

## Structure

- `fonts/` – self-hosted Inter subsets (SIL Open Font License)
- `images/` – photo slots; see `images/README.txt` for the file names. A slot stays hidden until its photo is added.
- `logo/` – logo files (SVG) for light and dark backgrounds
- `badges/` – IOSH, IFSM and NFRAR accreditation badges (PNG + WebP), shown unaltered as supplied
- `og-image.jpg` – image shown when the site is shared on social media
- `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `site.webmanifest` – browser and phone icons
- `robots.txt`, `sitemap.xml` – for search engines
- `.htaccess` – compression, caching and the `/home-1` redirect on Apache hosting
- `_headers`, `_redirects` – the same for Netlify

No build step: upload the files as they are to any static host.

## Before launch

- Point `derwentfirecompliance.co.uk` at the new host and keep the `/home-1` → `/` redirect.
- Submit `sitemap.xml` in Google Search Console (the verification tag from the old site is already included).
- Run [PageSpeed Insights](https://pagespeed.web.dev) and the [Rich Results Test](https://search.google.com/test/rich-results) on the live site.
- The quote form opens the visitor's email app; connect a form service (e.g. Formspree) to send it directly.
