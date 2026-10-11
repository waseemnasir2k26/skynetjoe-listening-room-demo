# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [2026.10] - 2026-10-12

- skynetjoe-listening-room-demo is a public static spec-demo landing page for The Listening Room (mental health advocacy, Leicester UK); no build step, deployed on Vercel, intentionally noindex.
- Reviewed October 2026: tree re-checked (index.html, assets, docs, .critic scorecards, archive); the README's one external link (skynetjoe.com) returned HTTP 200. Latest content commits are from 2026-09-10 (V2 promoted to root).
- Known gaps: the README says MIT but no LICENSE file existed, so a standard MIT LICENSE was added in this release; the README does not state the deployed demo URL; no CI.
- Release housekeeping only: Status line, changelog, LICENSE and Work with SkynetLabs section. No page or deploy-config changes.

## [2026.09] - 2026-09-16

- Maintenance review of skynetjoe-listening-room-demo — a spec demo landing page built by SkynetLabs for The Listening Room, an independent mental health advocacy service in Leicester, UK.
- Status: single-page static site (`index.html`, ~80 KB, with inline FAQ/JSON-LD content) plus `assets/`, no build step; deployed to Vercel. `vercel.json` sets `cleanUrls`, security headers (`nosniff`, `SAMEORIGIN`, `strict-origin-when-cross-origin`), a one-year immutable cache on `/assets/`, `X-Robots-Tag: noindex, nofollow`, and redirects `/v2`, `/v3` and `/archive/*` back to `/`.
- Supporting material is versioned alongside the page: `docs/` (client pitch and message, research, ship-gate report, evidence) and `.critic/` (three PASS scorecards from the 2026-09-07 critic run for v1/v2/v3); earlier variants are kept in `archive/`.
- Reviewed September 2026: docs refreshed, versioned as v2026.09. No page markup, asset or deploy-config changes in this release.
- Known gaps: README states MIT but there is no LICENSE file in the repo; no CHANGELOG.md before this release; the README does not state the deployed demo URL; the site is intentionally `noindex, nofollow` so it will not appear in search.
