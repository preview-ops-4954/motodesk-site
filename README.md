# gettorquebench.com homepage

Static marketing homepage for TorqueBench (https://gettorquebench.com). The product app
lives separately at https://torquebench.app/ (repo: motodesk-staging).

The legacy getmotodesk.com / app.getmotodesk.com pair was detached from the Render
services on 2026-09-17 and no longer serves the product. Contact inbox:
motoshop.research@mail.instinct.com. (Google Workspace mail on getmotodesk.com
still works; its MX/TXT records are separate and untouched.)

## Contents
- `index.html` - the whole page, self-contained (inline CSS, no build step, no JS)
- `favicon.svg` - site icon
- `og.png` - social share image (1200x630), generated from a screenshot of the hero
- `robots.txt`, `sitemap.xml` - crawl basics

## Deploy
Any static host works: upload these files and serve the directory as the site root.
Currently deployed as a Render static site from this repo with publish directory `/`.

Custom domains on the Render static site: `gettorquebench.com` (apex) and
`www.gettorquebench.com`.
DNS is at Porkbun: apex uses an ALIAS record to the Render target
(`motodesk-site.onrender.com`), `www` uses a CNAME. Do not touch the MX/TXT records
on getmotodesk.com - Google Workspace mail depends on them.

## Editing
Edit `index.html` directly; there is no framework. Keep the workbench identity:
paper #f4efdf, card #fffdf5, ink #111, accent #ef5b24, shadow #aaa28f;
headings Barlow Condensed, body IBM Plex Mono. If the hero changes, regenerate
`og.png` from a fresh 1200x630 screenshot of the top of the page.
