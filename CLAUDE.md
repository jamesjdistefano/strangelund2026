# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Strangelund is a portfolio website for James DiStefano, a systems designer. The site serves as a filtering mechanism—designed to exclude 95% of opportunities to find the 5% that fit. This is not a traditional UX portfolio; it positions Jim as someone who designs infrastructure and systems, not screens.

**Brand:** Strangelund
**Tagline:** A grove of unfamiliar trees

## Current State

This is a **greenfield project** using vanilla HTML, CSS, and JavaScript—no build system or static site generator.

### What Exists
- `strangelund-project-brief.md` — The canonical specification document. Read this first.
- 8 semantic HTML case study files with full written content
- 1 article HTML file (`why-i-stopped-calling-myself-a-ux-designer.html`)

### What Needs to Be Built
- Pages: Home (`index.html`), About, Case Studies (8), Article, Contact
- Clean URL structure using directory-based routing: `/case-studies/rock-hall/index.html` serves as `/case-studies/rock-hall/`
- Shared CSS with custom properties for theming
- Deploy configuration for Netlify/Vercel

## Technical Approach

**No build step.** Files are served as-is.

- **Accessibility:** WCAG 2.1 AA minimum
- **SEO:** Semantic HTML, meta tags, Open Graph per page
- **Performance:** Static files, minimal JavaScript
- **CSS:** Vanilla CSS with custom properties; must be themeable for later branding integration

## Local Development

Serve the site locally with any static server:

```bash
# Python
python3 -m http.server 8000

# Node (if npx available)
npx serve
```

Visual branding assets will be integrated later. Build with placeholder styling that exposes clear theming hooks.

## Content Files

The HTML files are the **source of truth** for all copy. Their heading structure should inform page layouts:

```
southern-company-gas.html
mailchimp.html
drip.html
grammarly.html
rock-hall.html
stash-wealth.html
boston-gov.html
super-deluxe.html
why-i-stopped-calling-myself-a-ux-designer.html
```

Each case study follows the pattern: "I didn't [conventional framing]. I designed a system for [actual value]."

## Voice and Tone

Avoid:
- Generic portfolio language ("passionate about user-centered design")
- Process theater (sticky notes, workshop photos)
- Listing tools as credentials
- Any implication of seeking a traditional UX role

The site should communicate: this person thinks in systems, not screens.
