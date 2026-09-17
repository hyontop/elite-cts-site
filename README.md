# Elite Construction Training Solutions

Website for Elite Construction Training Solutions — NPORS Accredited Training Provider.
Plant operator instruction and testing across 40 NPORS categories, NVQs levels 2–7,
CPCS, and NEBOSH-advised health & safety training. UK-wide, on site or at the training
facilities we use.

## What this is

A single self-contained `index.html`. No build step, no framework, no dependencies.
Fonts come from Google Fonts; the logo is embedded as a data URI. Open the file in a
browser and it works.

## Deploy

### Fastest — Vercel Drop (no Git, about a minute)

1. Go to **vercel.com/drop**
2. Drag `index.html` onto the page
3. Name the project, click **Deploy**

You get a live `*.vercel.app` URL immediately. Each drop creates a new project, so this
is best for getting something live today rather than for ongoing updates.

### Better — GitHub + Vercel (deploys itself on every push)

1. Push this repo to GitHub
2. vercel.com → **Add New → Project → Import** the repo
3. Framework preset **Other**. No build command, no output directory
4. **Deploy**

From then on, `git push` redeploys the site automatically.

### Custom domain

Vercel project → **Settings → Domains → Add** →
`eliteconstructiontrainingsolutions.co.uk`, then point the domain's DNS at Vercel as
instructed. Free on the Hobby plan.

## Editing

Everything is in `index.html`. The CSS custom properties at the top drive the design:

| Token | Purpose |
|---|---|
| `--ink` | Near-black — hero, proof section, footer |
| `--hiviz` | Brand yellow, sampled from the logo |
| `--hiviz-deep` | Darker yellow for small text (keeps contrast ≥4.5:1) |
| `--sand` | Warm off-white for alternating sections |
| `--s1`–`--s6` | Spacing scale (8 / 16 / 28 / 48 / 80 / 128px) |

## Still to add

Content only — the build is production-ready.

- [ ] **Company registration details.** A UK limited company must show its registered
      name, company number, place of registration and registered office address on its
      website. Not yet on the page because it has not been confirmed.
- [ ] Google reviews — ask every operator for one as you hand over their card
- [ ] A short video of a dig assessment or a test in progress
- [ ] Opening hours
- [ ] Lead instructor name and years of experience (the FAQ answer is currently accurate
      but generic)
- [ ] Which NEBOSH qualification the advisors hold
- [ ] Names for the two people in the testimonial photo — the caption reads "On site"

## Files

    index.html          the page
    img/                photography, accreditation marks, icons, share card
    favicon.ico         root-level icon
    robots.txt          allows all, points at the sitemap
    sitemap.xml         single URL, update lastmod when the page changes

`index.html` references `img/` by relative path. The single-file copy delivered
separately inlines every image as a data URI so it can be hosted by dropping one file.

## Verification

Checked at 320, 360, 390, 414, 600, 768, 834, 1024, 1280, 1440 and 1920px: no
horizontal overflow, no tap target under 44px, no contrast failure, no console errors,
no dead links or duplicate ids. All forty NPORS codes verified against the official
NPORS category list (Nov 2023). Hero headline contrast measured against the actual
backdrop of each slideshow frame: worst case 11.2:1 white, 6.4:1 hi-viz.
