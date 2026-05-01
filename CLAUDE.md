# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This repo hosts legal documents (privacy policies, terms of use) for Tanner Gordon's apps as a GitHub Pages site. The live site is at `https://tannergordon.github.io/legal/`.

## Structure

- `_config.yml` — Jekyll config (Minima theme, no build step needed)
- `index.md` — landing page linking to all app legal docs
- `<appname>/privacy.md` — privacy policy for each app
- `<appname>/terms.md` — terms of use for each app

## Adding docs for a new app

1. Create `<appname>/privacy.md` and `<appname>/terms.md` with Jekyll front matter:
   ```yaml
   ---
   layout: page
   title: "AppName – Privacy Policy"
   permalink: /<appname>/privacy
   ---
   ```
2. Add links to the new pages in `index.md`.
3. Update the URL constants in the corresponding app's source code.

## Deployment

GitHub Pages builds automatically on every push to `main`. No local build needed. To enable Pages on a fresh clone of the repo: **GitHub → Settings → Pages → Source: Deploy from branch → main / (root)**.
