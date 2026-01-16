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

## Image Generation — Vector Arcade Style

Use this prompt template with ChatGPT (GPT-4 + DALL-E) to generate images in the Strangelund visual style.

**Goal: Simple but recognizable.** Think 1983 arcade aesthetics—wireframe with visible structure, but not dense polygon meshes. The subject should read clearly but feel sparse and geometric. Aim for the complexity of a Battlezone tank or Star Wars TIE fighter: identifiable shapes with some internal wireframe lines, but not photorealistic detail.

```
Vector graphics illustration of [SUBJECT] in the style of 1983 arcade vector games like Battlezone and Star Wars. Simple wireframe rendering—visible geometric structure but not dense polygon meshes. Glowing phosphor [COLOR] lines on pure black background. [SUBJECT] as low-polygon wireframe: [SPECIFIC GEOMETRY DESCRIPTION]. Show the basic 3D structure with edge lines and a few internal divisions, but avoid dense grid patterns or excessive detail. The look of early 3D graphics—clearly geometric, clearly digital. Generous empty space around the subject. CRT phosphor bloom effect on the lines. Technical, stark, and strange.

Keep it simple: outline the form, show basic internal structure, stop there. No surface texture, no dense meshes, no realistic detail.

No realistic rendering, no photography, no filled shapes, no gradients, no pixel art, no raster graphics, no color except [COLOR], no backgrounds, no textures, no organic curves, no hand-drawn style, no cartoon style, no dense wireframe grids, no busy compositions.

Style references:
Atari Battlezone (1980) — simple 3D tanks and obstacles
Atari Star Wars (1983) — TIE fighters, Death Star trench
Vectrex console graphics — clean glowing wireframes
```

**Variables:**
- `[SUBJECT]`: What you're depicting (trees, buildings, mountains, etc.)
- `[COLOR]`: Line color (light blue, green, amber, magenta, etc.)
- `[SPECIFIC GEOMETRY DESCRIPTION]`: How the subject becomes wireframe (basic shapes, simple divisions)
- `[OFFSET]`: Position of main subject — `left`, `right`, or `center`

**Refinement prompt:** `[COMPOSITION]. Position the main subject on the [OFFSET] side of the frame. Fade to pure black on the opposite side and at the bottom edge—keep those areas empty for text. Keep the wireframe simple—basic structure, not dense mesh. Make it [WIDTH] wide at [RATIO] aspect ratio. Use [COLOR].`

**If the result is too detailed:** "Simplify the wireframe. Remove the dense grid pattern—keep only the major structural lines that define the shape. Think Battlezone, not modern 3D software."

**If the result is too simple:** "Add some internal wireframe structure to show 3D form—a few horizontal or vertical divisions. It should look like a low-polygon 3D model, not just an outline."

## Voice and Tone

Avoid:
- Generic portfolio language ("passionate about user-centered design")
- Process theater (sticky notes, workshop photos)
- Listing tools as credentials
- Any implication of seeking a traditional UX role

The site should communicate: this person thinks in systems, not screens.
