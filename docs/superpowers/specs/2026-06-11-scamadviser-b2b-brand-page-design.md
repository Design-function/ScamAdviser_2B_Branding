# ScamAdviser B2B Brand Guideline Page — Design Spec

**Date:** 2026-06-11
**Status:** Approved
**Source:** ScamAdviser_Brand Guideline_Visual_V1_20260209.pdf (82 pages)

## Overview

Single-page interactive HTML brand guideline for ScamAdviser's B2B identity. Protected by login gate. Content sourced from the 82-page PDF brand guideline. Images referenced from extracted `assets/` directory. Styled in the B2B visual language.

## Audience

Designers, internal team, and partners who need to understand how ScamAdviser B2B branding looks, feels, its tone of voice, and design system.

## Architecture

### Login Gate
- Dark overlay with centered card, ScamAdviser shield logo, password input
- Passwords: `1234`, `ScamAdviser2026`
- Fade-to-content transition on success

### Navigation
- **Sticky sidebar nav** (left, ~240px, dark background)
- Scroll-tracking active state highlights current section
- Collapses to hamburger overlay on screens < 1024px
- 12 section labels: Hero, Brand Personality, Tone of Voice, Logo, Co-Branding, Color Palette, Typography, Iconography & Graphics, Data Visualization, Photography, Brand Applications, Skills Download

### Hero
- Full-viewport dark section
- SVG red chevron shapes animate in from edges
- ScamAdviser shield logo centers and reveals
- Tagline types in: "Shaping the Global Anti-scam Industry in the AI Era"
- Version badge: "Brand Guidelines V.1 — Feb 2026"

## Sections

| # | Section | PDF Pages | Treatment |
|---|---------|-----------|-----------|
| 00 | Hero | Cover (p.1) | Animated geometric hero |
| 01 | Brand Personality | p.3-12 | Pillar cards, attributes grid |
| 02 | Tone of Voice | p.13-18 | Expandable content pillar cards, do/don't pairs |
| 03 | Logo | p.19-28 | SVG logo variants, clear space, misuse grid |
| 04 | Co-Branding | p.29-32 | Placement rules, spacing diagrams |
| 05 | Color Palette | p.33-38 | Interactive swatches, click-to-copy hex, 60-30-10 demo |
| 06 | Typography | p.39-44 | Live font specimens, type scale, hierarchy |
| 07 | Iconography & Graphics | p.45-52 | Icon grid, abstract graphics, chevron motif |
| 08 | Data Visualization | p.53-63 | 7 interactive SVG chart types |
| 09 | Photography | p.64-74 | Full gallery (~30 photos), 8 sub-categories, Do's/Don'ts |
| 10 | Brand Applications | p.75-82 | Mockup gallery from extracted images |
| 11 | Skills Download | Custom | Downloadable SKILL.md cards |

## Design Tokens

```css
:root {
  --sa-red: #CC1417;
  --sa-dark: #1A1A1A;
  --sa-white: #FFFFFF;
  --sa-light: #F5F5F5;
  --sa-grey: #E8E8E8;
  --sa-medium-grey: #666666;
  --font-primary: 'Inter', -apple-system, sans-serif;
  --font-secondary: 'Roboto', sans-serif;
  --font-regional: 'Noto Sans', sans-serif;
}
```

## Interactivity
- Click-to-copy hex values
- Smooth scroll nav with active section tracking
- Section entrance animations (fade-up on scroll)
- SVG chart hover states with tooltips
- Logo clear-space interactive overlay
- Expandable cards for Tone of Voice
- Photography lightbox
- Mobile hamburger nav

## File Structure
```
ScamAdviser_2B_Branding/
├── scamadviser-b2b-brand.html
├── assets/
│   ├── pdf-images/     (121 extracted images)
│   └── page-renders/   (82 page renders)
├── skills/
│   └── scamadviser-b2b-brand.md
└── docs/superpowers/specs/
    └── 2026-06-11-scamadviser-b2b-brand-page-design.md
```
