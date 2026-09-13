# Elite Construction Training Solutions

The website for Elite Construction Training Solutions — NPORS Accredited Training
Provider, plant operator instruction and testing across 40 NPORS categories, NVQs,
CPCS and NEBOSH-advised health & safety training.

## What this is

A single self-contained `index.html`. No build step, no framework, no dependencies.
Fonts load from Google Fonts; the logo is embedded in the file as a data URI. You can
open `index.html` in a browser and it works.

## Deploying to Vercel

1. Push this repo to GitHub (see below)
2. Go to vercel.com and sign in
3. **Add New → Project → Import** this repository
4. Framework preset: **Other**. No build command, no output directory. Vercel serves
   `index.html` automatically
5. **Deploy**

After that, every push to `main` redeploys the site automatically.

### Custom domain

In the Vercel project: **Settings → Domains → Add**, enter
`eliteconstructiontrainingsolutions.co.uk`, then point the domain's DNS at Vercel as
instructed. Free on the Hobby plan.

## Editing the site

Everything lives in `index.html`. The CSS custom properties at the top control the
whole design:

| Token | Purpose |
|---|---|
| `--ink` | Near-black used for the hero, footer and headings |
| `--hiviz` | Brand yellow, taken from the logo |
| `--hiviz-deep` | Darker yellow for small text (keeps contrast ≥4.5:1) |
| `--sand` | Warm off-white for alternating sections |
| `--s1`–`--s6` | The spacing scale |

## Still to add

These are marked in the page and need real information before going live:

- [ ] Opening hours (contact section)
- [ ] Lead instructor — name, years of plant/site experience, instructing background
- [ ] Which NEBOSH qualification the health & safety advisors hold
- [ ] Photographs — see the three labelled slots in the page:
  - 360 excavator with an operator, on site or in the yard
  - Instructor with an operator at the controls
  - Operator holding a newly issued NPORS card

## Accuracy note

Every claim on this page comes from either the business's own live site or the NPORS
instructor category list. The 40 N-codes are cross-referenced against the official
NPORS published category list. Nothing is invented — please keep it that way when
editing.
