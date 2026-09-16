# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [2026.09] - 2026-09-16

- Maintenance review of skynetjoe-listening-room-demo — a spec demo landing page built by SkynetLabs for The Listening Room, an independent mental health advocacy service in Leicester, UK.
- Status: single-page static site (`index.html`, ~80 KB, with inline FAQ/JSON-LD content) plus `assets/`, no build step; deployed to Vercel. `vercel.json` sets `cleanUrls`, security headers (`nosniff`, `SAMEORIGIN`, `strict-origin-when-cross-origin`), a one-year immutable cache on `/assets/`, `X-Robots-Tag: noindex, nofollow`, and redirects `/v2`, `/v3` and `/archive/*` back to `/`.
- Supporting material is versioned alongside the page: `docs/` (client pitch and message, research, ship-gate report, evidence) and `.critic/` (three PASS scorecards from the 2026-09-07 critic run for v1/v2/v3); earlier variants are kept in `archive/`.
- Reviewed September 2026: docs refreshed, versioned as v2026.09. No page markup, asset or deploy-config changes in this release.
- Known gaps: README states MIT but there is no LICENSE file in the repo; no CHANGELOG.md before this release; the README does not state the deployed demo URL; the site is intentionally `noindex, nofollow` so it will not appear in search.
