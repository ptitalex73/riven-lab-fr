# Riven Lab

A free, community-made Warframe Riven analyzer. It reads a Riven screenshot, extracts the weapon and stat lines, and estimates a build-fit grade. It can also compare matching public asking listings from Warframe Market and rivens.wf when those services are available.

**Public project, built primarily with AI assistance (OpenAI Codex).** The maintainer provides requirements, checks results, and reports corrections. This is not a hand-coded project.

## Features

- Screenshot OCR for English and French Riven cards
- Manual review and correction of recognized stats
- Heuristic Riven analysis with its assumptions shown in the app
- Optional lookup of public asking listings; prices are not completed sales or appraisals
- No automated trading, purchases, sales, or trader messages

## Run locally

Requires Node.js 22 or later and the Netlify CLI.

1. Install the Netlify CLI.
2. From this directory, run `netlify dev`.
3. Open the local address printed by the CLI.

The Market lookup is served by `netlify/functions/market.mjs`. It uses public listing data and includes request caching and throttling. No API key or account token is required by this project.

## Deployment

Deploy this directory as a Netlify site with the included `netlify.toml`. Keep `.netlify` state and any environment files out of version control.

## Notes

This is an independent community project and is not affiliated with Digital Extremes, Warframe, or Warframe Market. Grades are heuristic, not official Warframe ratings. Warframe Market prices are sellers' asking prices and can change at any time.

No license has been granted for reuse; all rights are reserved by the copyright holder unless a license is added later.
