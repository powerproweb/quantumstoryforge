# QuantumStoryForge.io — Navigation Reorganization & Premium CSS Upgrade

### -<<<|||>>>--<<<|||>>>--<<<|||>>>- BEGIN - DESCRIPTIONS -<<<|||>>>--<<<|||>>>--<<<|||>>>- ###

# Prompt for Descriptions: I need these descriptions of this project... 
	* 290 Character - Github Description:
	* long very complete description:
	* short & precise description:
	* About us page desc:
	* Homepage hero desc:
	* Polished promotional Desc:
	* github.README
	
	from the build.plan.features.benefits.md or something like this.
	
	After this create a GitHub.README.md also

# ChatGPT - BUILD_plan.md Description - Polished promotional description:


# ChatGPT - BUILD_plan.md Description - Homepage hero / intro version:


# ChatGPT - BUILD_plan.md Description - About Us Page:


# ChatGPT - BUILD_plan.md Description - Longest:


# ChatGPT - BUILD_plan.md Description - Long:


# ChatGPT - BUILD_plan.md Description - Short:


# ChatGPT - GitHub.README.md Description: 


# ChatGPT - GitHub.README.md Description2: 


# ChatGPT - 290 Character - Github Description: 


### -<<<|||>>>--<<<|||>>>--<<<|||>>>- END - DESCRIPTIONS -<<<|||>>>--<<<|||>>>--<<<|||>>>- ###

## Problem Statement

The site needs a reorganized navigation structure with renamed menu groupings and a new "Aetherforge AI Memory" link. The CSS should be cleaned up and elevated to premium quality while keeping the existing dark steampunk color theme (brass/amber accents on dark backgrounds).

## Current State

**Pages:** `index.html`, `contact.html`, `aetherforge_council_of_8.html`, `steampunk_stardate_calculator.html`, `peregrine_plasma_rifle.html`

**Stylesheets:** `site.css` (active, 1590 lines — all pages reference this), `custom.css` (legacy dead file — NOT linked by any page, contains unrelated styles from a previous project)

**Current nav (same across all 5 pages):**

- AetherForge Tools → Council of 8, Steampunk Stardate Generator
- WorldBuilding Extras → HMR-9 Peregrine Field Manual, QuantumDrive Forge Tree (external)
- Contact Us

## Proposed Changes

### 1. New Navigation Structure (all 5 HTML pages)

Update the nav in `index.html`, `contact.html`, `aetherforge_council_of_8.html`, `steampunk_stardate_calculator.html`, and `peregrine_plasma_rifle.html` to:

- **Aetherforge AI Tools** (dropdown)
  - Aetherforge AI Memory → `https://quantumstoryforge.io/recallos/`
  - Aetherforge Council of 8 → `aetherforge_council_of_8.html`
- **Worldbuilding Extras** (dropdown)
  - Steampunk Stardate Generator → `steampunk_stardate_calculator.html`
  - HMR-9 Peregrine Field Manual → `peregrine_plasma_rifle.html`
- **QD Forge Tree** → `https://qdls.io/` (top-level link, opens in new tab)
- **Contact Us** → `contact.html`

### 2. Premium CSS Enhancements in `site.css`

Keep the existing color palette (`--bg-main: #050608`, `--accent: #c28f3f`, `--accent-soft: #f3d5a1`, etc.) and upgrade:

- **Nav bar:** Add a subtle gold underline hover animation on nav links; smoother dropdown transitions with a slight backdrop blur; active-page indicator highlight.
- **Typography:** Import `Cormorant Garamond` from Google Fonts (already referenced as `--display-font` but never loaded); add a `font-display: swap` for performance.
- **Hero sections:** Add a subtle parallax-like shimmer/glow on the hero border frame using CSS keyframes; a faint animated gold gradient sweep on hero edges.
- **Cards (Council):** Subtle glassmorphism effect (backdrop-filter) on hover; refined glow ring.
- **Buttons:** Richer gradient transitions; subtle box-shadow pulse on hover.
- **Footer:** Slightly elevated with a faint top-edge gold glow line.
- **Scrollbar:** Custom-styled scrollbar matching the theme (`::-webkit-scrollbar`).
- **Selection:** Custom `::selection` highlight using brass/amber tones.
- **Overall polish:** Smoother transitions site-wide (300ms ease default), refined spacing consistency.

### 3. Delete `custom.css`

Remove `custom.css` entirely — it contains ~1600 lines of legacy CSS from a completely unrelated project and is not linked by any page.

### 4. Homepage Content Refresh (`index.html`)

Replace the current placeholder body text (generic hub description) with a more engaging layout:

- Add visual "feature cards" linking to each tool/page (Council of 8, Stardate Generator, Peregrine Manual) with short descriptions and subtle hover effects.
- This replaces the current wall-of-text with a visually navigable dashboard.

## Files to Modify

- `index.html` — nav + body content refresh
- `contact.html` — nav update
- `aetherforge_council_of_8.html` — nav update
- `steampunk_stardate_calculator.html` — nav update
- `peregrine_plasma_rifle.html` — nav update
- `site.css` — premium CSS enhancements, Google Font import, new card styles

## Files to Delete

- `custom.css`

---

## Change Log

### Completed — 2026-04-10

**1. Navigation restructured (all 5 HTML pages)**
- Renamed "AetherForge Tools" → **Aetherforge AI Tools**
- Added **Aetherforge AI Memory** dropdown link → `https://quantumstoryforge.io/recallos/`
- Kept **Aetherforge Council of 8** under AI Tools dropdown
- Renamed "WorldBuilding Extras" → **Worldbuilding Extras**
- Moved **Steampunk Stardate Generator** into Worldbuilding Extras dropdown
- Kept **HMR-9 Peregrine Field Manual** in Worldbuilding Extras dropdown
- Added **QD Forge Tree** as a new top-level nav link → `https://qdls.io/`
- Removed the old "QuantumDrive Forge Tree" from inside the dropdown
- Pages updated: `index.html`, `contact.html`, `aetherforge_council_of_8.html`, `steampunk_stardate_calculator.html`, `peregrine_plasma_rifle.html`

**2. Premium CSS enhancements (`assets/css/site.css`)**
- Imported **Cormorant Garamond** from Google Fonts (was declared in `--display-font` but never loaded)
- Added gold underline hover animation on nav links
- Added caret rotation (180°) on dropdown hover
- Dropdown menus now use **backdrop-filter blur** with glassmorphism effect
- Dropdown links slide-indent on hover with subtle background highlight
- Hero banner frames have an **animated gold shimmer border** (CSS `@keyframes heroShimmer`)
- Hero images have a subtle zoom on hover
- Council cards gain **glassmorphism + glow ring** on hover with card lift
- Buttons have richer hover with lift (`translateY(-1px)`) and double-layer glow shadow
- Footer has a **gold gradient glow line** across the top edge
- Added custom **brass-themed scrollbar** (`::-webkit-scrollbar` + Firefox `scrollbar-color`)
- Added brass/amber **`::selection`** text highlight

**3. Homepage content refresh (`index.html`)**
- Replaced generic wall-of-text with **5 interactive feature cards** in a responsive grid:
  - Aetherforge AI Memory → `quantumstoryforge.io/recallos/`
  - Aetherforge Council of 8 → `aetherforge_council_of_8.html`
  - Steampunk Stardate Generator → `steampunk_stardate_calculator.html`
  - HMR-9 Peregrine Field Manual → `peregrine_plasma_rifle.html`
  - QD Forge Tree → `qdls.io`
- Cards have hover lift, gold top-line reveal, and expanding arrow text

**4. Deleted `custom.css`**
- Removed ~1,600 lines of legacy CSS from an unrelated project (not linked by any page)

**5. Moved CSS to `assets/css/`**
- Relocated `site.css` → `assets/css/site.css`
- Updated `<link rel="stylesheet">` in all 5 HTML pages to reference `assets/css/site.css`

**6. Council of 8 — Individual Bio Pages (2026-04-10)**
- Created `gpt_council_8/` folder structure for council member pages
- Created 8 individual bio pages, each with:
  - Same header/nav/footer/CSS/JS as the main council page
  - Member headshot portrait
  - One-line tagline
  - **Signature Profile** — role description, specialties, traits, "known for"
  - **Full Backstory** — extended narrative origin story
  - "Back to Council of 8" breadcrumb navigation
- Pages created:
  - `gpt_council_8/caelan-rhys-mercer.html` — Hard SF Worldbuilding Engineer
  - `gpt_council_8/amara-lian-okafor.html` — Lore & History Cartographer
  - `gpt_council_8/rafael-inigo-duarte.html` — Political/Espionage Temporal Strategist
  - `gpt_council_8/sienna-myles-armitage.html` — Aether Systems Alchemist
  - `gpt_council_8/gideon-thane-blackwell.html` — Character Psychology Architect
  - `gpt_council_8/leyla-ferah-altun.html` — Conflict & War Theorist
  - `gpt_council_8/arata-kenjiro-sato.html` — Socio-Political Futurist
  - `gpt_council_8/seraphine-elowen-marcell.html` — Myth & Symbolism Curator
- Content merged from `council_8_backstories.md`:
  - Signature Profiles (lines 49–164)
  - Full Backstories (lines 200–305)
- Added **Section 14: Council Bio Pages** to `assets/css/site.css`:
  - `.council-bio-page` container layout
  - `.bio-header` flex layout with portrait + name/role/tagline
  - `.bio-portrait` styled with border glow and shadow
  - `.bio-section` content sections with gold divider borders
  - `.bio-traits` highlighted panel with brass accent background
  - `.bio-breadcrumb` back-navigation link
  - Responsive: stacks portrait/text vertically on mobile (≤720px)
- All 8 "Read Bio" links on `aetherforge_council_of_8.html` now resolve to working pages

## File Inventory

### Root Pages
- `index.html` — Homepage with feature cards
- `contact.html` — Contact form
- `steampunk_stardate_calculator.html` — Stardate tool
- `peregrine_plasma_rifle.html` — HMR-9 field manual

### Council of 8 (`gpt_council_8/`)
- `aetherforge_council_of_8.html` — Main council page with 8 headshot cards
- `caelan-rhys-mercer.html` — Dr. Caelan Rhys Mercer bio
- `amara-lian-okafor.html` — Amara Lian Okafor bio
- `rafael-inigo-duarte.html` — Rafael Íñigo Duarte bio
- `sienna-myles-armitage.html` — Dr. Sienna Myles Armitage bio
- `gideon-thane-blackwell.html` — Gideon Thane Blackwell bio
- `leyla-ferah-altun.html` — Leyla Ferah Altun bio
- `arata-kenjiro-sato.html` — Arata Kenjiro Sato bio
- `seraphine-elowen-marcell.html` — Seraphine Elowen Marcell bio
- `council_8_backstories.md` — Source content for all profiles and backstories

### Assets
- `assets/css/site.css` — Unified stylesheet (14 sections)

### Recallos (`recallos/`)
- `index.html` — Recallos AI Memory landing
- `benefits.html` — Benefits page
- `css/styles.css` — Recallos-specific styles
- `js/main.js` — Recallos scripts
- `errors/` — 400, 401, 403, 404, 500, 503 error pages
