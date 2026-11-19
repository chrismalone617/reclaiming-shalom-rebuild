# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website rebuild for Reclaiming Shalom (reclaimingshalom.com) - a Narrative Focused Trauma Care practice. This rebuild replaces the original drawer/hamburger menu with a standard horizontal navigation.

## Development

No build process required. Open `index.html` directly in a browser to preview.

```bash
# Quick preview with Python server (optional)
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Architecture

**Single-page static site** with vanilla HTML/CSS/JS:
- `index.html` - Homepage (all sections in one file)
- `css/styles.css` - All styles with CSS custom properties
- `js/main.js` - Scroll effects, intersection observer animations, form validation utility

## Design System

CSS variables are defined in `:root` in `styles.css`:

| Variable | Value | Usage |
|----------|-------|-------|
| `--color-primary` | `#4a7023` | Primary green (brand color) |
| `--color-primary-dark` | `#3a5a1a` | Hover states |
| `--color-secondary` | `#f76a0c` | Orange accent (CTAs, links) |
| `--font-heading` | Barlow | H1-H6, logo |
| `--font-body` | Poppins | Body text, buttons |

Responsive breakpoints: 1024px (tablet), 768px (mobile)

## Current State

Homepage only. Placeholder content for:
- Images/illustrations in content sections
- Article images in blog cards
- Certification badge image
- Social media links in footer

Navigation links point to pages not yet created: `/about`, `/services`, `/blog`, `/resources`, `/contact`, `/consultation`
