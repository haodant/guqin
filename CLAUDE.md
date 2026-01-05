# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for the New York Qin and Calligraphy Society (Su Ling Qin She) - an educational institution for Chinese guqin music and calligraphy instruction. Built with HTML5, CSS3, and vanilla JavaScript.

## Running Locally

No build step required. Open HTML files directly in a browser or use a local server:

```bash
python -m http.server 8000
# Or: npx http-server
```

## Architecture

**Pages:** 6 HTML pages (index, guqin, calligraphy, about, events, contact) with consistent navigation header/footer.

**Key Libraries (all vendored):**
- Bootstrap 3 - grid system and responsive utilities
- jQuery 1.11.0 - DOM manipulation
- Wow.js + Animate.css - scroll-triggered animations
- Font Awesome - icons

**Custom Code:**
- `css/main.css` - Site-specific styles, responsive breakpoints, color utilities
- `js/main.js` - Navbar scroll behavior, smooth anchor scrolling, Wow.js initialization

**Animation Pattern:** Uses `data-wow-delay` attributes on elements with class `wow` for staggered scroll animations. Animations disabled on mobile.

**Responsive Breakpoints:** 480px, 767px, 991px, 1199px

**Color Palette:** Primary brown (#a98175), teal accent (#70cbce), dark (#231f20)

## Deployment

Live site: https://newyorkguqin.com

Hosted via GitHub Pages. Pushing to `master` automatically deploys changes to the live site.

## Content Notes

- All pages are bilingual (English/Chinese)
- Typography uses Google Fonts: Montserrat (headings), Raleway (body)
