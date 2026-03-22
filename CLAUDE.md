# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Static HTML site hosted via GitHub Pages containing support pages and privacy policies for BrainVault iOS apps. No build tools, no frameworks, no dependencies — just plain HTML/CSS files served directly.

## Deployment

Push to `main` triggers GitHub Pages deployment automatically. The `.nojekyll` file disables Jekyll processing.

## Adding a New App

1. Create a directory named after the app (lowercase)
2. Add `index.html` (support page) and `privacy-policy.html`
3. Add a link card in the root `index.html`'s `.apps` div

## Design Conventions

All pages share the same visual language — match it when adding or editing pages:
- **Font stack**: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif`
- **Color palette**: background `#F9F6F2`, card white `#fff`, text `#2D2823`, accent `#8C7055`, secondary text `#6b6560`, border `#e8e2da`
- **Layout**: centered `.container` at `max-width: 720px`, `border-radius: 16px`, `box-shadow: 0 2px 12px rgba(0,0,0,0.06)`
- **CSS is inlined** in each HTML file (no shared stylesheet)
- Contact email: brainvault.mind@gmail.com

## Related Repositories

The iOS app source code lives in sibling directories:
- **CellMonitor (Datamonitor)**: `../Datamonitor`
- **iCart**: `../iCart`
