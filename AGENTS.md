# AGENTS.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

QuantumStoryForge.io is the AetherForge Worldbuilding Hub — a steampunk science fiction worldbuilding and narrative infrastructure site. It hosts worldbuilding tools, story resources, interactive calculators, and AI-powered writer collaboration tools for a steampunk universe.

## Architecture

### Frontend (Static HTML + CSS + JS)

All pages are flat `.html` files at the project root with embedded or shared CSS. No build step, no bundler, no framework.

**Key pages:**
- `index.html` — AetherForge Worldbuilding Hub homepage with fixed header, responsive nav, and content sections
- `aetherforge_council_of_8.html` — Steampunk Science Fiction Writers Think Tank — 8 specialized AI personas, each a different genre author with unique skills
- `arc_team.html` — ARC team information
- `steampunk_stardate_calculator.html` — Interactive Steampunk Stardate Calculator (Chronometric Guild Edition) with tabbed UI, date conversion, and styled display
- `peregrine_plasma_rifle.html` — In-universe artifact page (Peregrine Plasma Rifle)
- `custom.css` — Shared custom styles

### Design System
- **Steampunk dark theme:** Dark base (`#050608`), brass/gold accents (`#c28f3f`, `#f3d5a1`), red accent (`#b84b3c`)
- **CSS custom properties** for all theme tokens
- **Fixed header** with brass-glow brand icon and CSS-only hamburger menu (checkbox toggle)
- **Panel/card system:** Glassmorphism panels with gradient backgrounds and soft borders
- **Typography:** System fonts for body, `Cormorant Garamond` / `Cinzel` for display headings, monospace for data displays
- **Interactive elements:** Tab components, styled form inputs, glowing buttons

## Tech Stack
- Static HTML + CSS (embedded and external) + vanilla JS
- No framework, no npm, no build tools
- Apache shared hosting (BlueHost/cPanel) with PHP 8.2 handler

## Hosting & Deployment
- `.htaccess` contains only the cPanel PHP handler
- Deploy by uploading files directly
- No build step required

## Conventions
- Steampunk brass/dark aesthetic across all pages
- CSS-only responsive hamburger menu (checkbox toggle pattern)
- Hero sections with gradient overlays and kicker/title/subtitle structure
- Tab components use `.tab-btn.active` / `.tab-content.active` pattern with JS toggle
- Pages are self-contained with embedded `<style>` blocks (some share `custom.css`)

## Important Notes
- The `.htaccess` is minimal (PHP handler only) — security headers and rewrites should be added before production use
- The Stardate Calculator has significant embedded JS for date conversion logic
- Pages share the same steampunk design system but embed their own CSS (no single shared stylesheet yet)
