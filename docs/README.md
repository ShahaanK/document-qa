# Verandah AI — Casual Market Atlanta landing page

A single-file landing page aimed at attendees of **Fall Casual Market Atlanta**
(Sept 15–18, 2026, AmericasMart Building 1), presented by the International
Casual Furnishings Association (ICFA) — including the ICFA Awards Gala on
Wednesday, Sept 16 at the Hyatt Regency Atlanta.

## Publishing on GitHub Pages

Repo → **Settings → Pages → Build and deployment**:

- **Source:** Deploy from a branch
- **Branch:** `claude/icfa-conference-website-f9ovc8` (or `main` after merge) → **`/docs`**

The page goes live at `https://<owner>.github.io/document-qa/`. `.nojekyll` is
present so Jekyll doesn't touch the raw HTML.

To preview locally: `python3 -m http.server -d docs 8000`

## Before you share the link

Three placeholders are deliberate — swap them:

| What | Where | Current value |
| --- | --- | --- |
| Company name | Throughout (`<title>`, header, footer) | `Verandah AI` |
| Contact email | `#contact` section | `hello@verandah.ai` |
| Phone number | `#contact` section | `Add your number` |

Renaming the company is a find/replace on `Verandah AI` (plus the
`verandah-theme` localStorage key and the `hello@verandah.ai` mailto if you
change domains).

## What's deliberately *not* on the page

No customer logos, testimonials, case-study numbers, or traction claims — there
are none yet, and fabricated social proof is the fastest way to lose a room full
of people who all know each other. The page sells the pipeline and the pilot
offer instead.

## Notes on the content

- Every industry figure in the "Why this year" table is sourced in the footer
  (tariff rates, import-volume swing, market format).
- The live strip counts down to Friday close (`2026-09-18T17:00:00-04:00`) and
  swaps its message once the gala evening passes and again after market closes.
  Update those two timestamps in the inline script to reuse the page for the
  next market.
- The "four pilots" capacity claim and the 14-day timeline are commitments —
  make sure you actually want to make them before sharing.
