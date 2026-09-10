# getmotodesk.com homepage

Static marketing homepage for MotoDesk (https://getmotodesk.com). The product app
lives separately at https://app.getmotodesk.com/ (repo: motodesk-staging).

## Contents
- `index.html` - the whole page, self-contained (inline CSS, no build step, no JS)
- `favicon.svg` - site icon
- `og.png` - social share image (1200x630), generated from a screenshot of the hero
- `robots.txt`, `sitemap.xml` - crawl basics

## Deploy
Any static host works: upload these files and serve the directory as the site root.
Currently deployed as a Render static site from this repo with publish directory `/`.

Custom domains: `getmotodesk.com` (apex) and `www.getmotodesk.com`. DNS is at Porkbun:
apex uses an ALIAS record to the Render target, `www` uses a CNAME. Do not touch the
MX/TXT records - Google Workspace mail for getmotodesk.com depends on them.

## Editing
Edit `index.html` directly; there is no framework. Keep the workbench identity:
paper #f4efdf, card #fffdf5, ink #111, accent #ef5b24, shadow #aaa28f;
headings Barlow Condensed, body IBM Plex Mono. If the hero changes, regenerate
`og.png` from a fresh 1200x630 screenshot of the top of the page.
