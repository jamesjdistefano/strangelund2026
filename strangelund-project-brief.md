# Strangelund Portfolio Website — Project Brief

## What This Is

A portfolio website for James DiStefano (Jim), a systems designer repositioning away from traditional UX design toward "designing systems that make experiences possible."

**Brand:** Strangelund  
**Tagline:** A grove of unfamiliar trees

---

## The Goal

Create a portfolio that **excludes 95% of opportunities to find the 5% that fit.**

This is not a job-seeking portfolio. It's a filtering mechanism. The right visitor should immediately understand: this person doesn't design screens, they design the infrastructure underneath.

The wrong visitor (looking for a Principal UX Designer to make Figma flows) should self-select out.

---

## Strategic Positioning

Jim's work is about:
- Articulating vision and strategic position
- Designing systems (content models, probability engines, intelligence layers) that enable experience
- Building infrastructure that makes differentiated outcomes possible

He is not:
- A UI designer
- A screen-flow person
- Someone who catches up to competitors' feature sets

**The one-liner pattern across all work:**  
"I didn't [conventional framing]. I designed a system for [actual value]."

---

## Content Structure

### Pages

1. **Home**
   - Brief positioning statement
   - Navigation to case studies and article
   - The tagline: "A grove of unfamiliar trees"

2. **About**
   - Who Jim is
   - The shift from UX designer to systems designer
   - What he's looking for (the filter): green field problems, appetite for risk, aversion to parity
   - What he won't do: screens, incremental UI, catch-up roadmaps

3. **Case Studies** (8 total)
   - Southern Company Gas: "I didn't design five websites. I designed a system that produces websites."
   - Mailchimp: "I didn't build a content library. I designed a system for manufacturing marketing competence."
   - Drip: "I didn't design a dashboard. I designed a system that tells you where to intervene."
   - Grammarly: "I didn't design an email feature. I designed a system that turns email into a knowledge graph."
   - Rock and Roll Hall of Fame: "I didn't redesign a website. I designed a system for exercising authority at scale."
   - Stash Wealth: "I didn't add technology to a financial services firm. I designed a system that lets humans scale."
   - Boston.gov: "I didn't redesign a government website. I designed a system that makes bureaucracy invisible."
   - Super Deluxe: "I didn't fill a programming gap. I designed a system for incubating culture at scale."

4. **Article**
   - "Why I Stopped Calling Myself a UX Designer"
   - This is the philosophical spine — explains the shift, uses Rock Hall as the turning point

5. **Contact**
   - Email
   - LinkedIn (optional)
   - No contact form needed

---

## Content Files

Semantic HTML files for all case studies and the article are already written and available. These contain the full text content structured with proper heading hierarchy. Use these as the source of truth for copy.

---

## Technical Requirements

### Must Have
- **Accessible:** WCAG 2.1 AA compliance minimum
  - Proper heading hierarchy
  - Sufficient color contrast
  - Keyboard navigable
  - Screen reader friendly
  - Alt text ready (placeholders for now, visuals coming later)
  
- **SEO Optimized:**
  - Semantic HTML structure
  - Proper meta titles and descriptions per page
  - Open Graph tags for social sharing
  - Clean URL structure (/case-studies/rock-hall, not /case-studies?id=3)
  - Fast load times
  
- **Responsive:** Works on mobile, tablet, desktop

- **Performance:** Static site, minimal JavaScript, fast globally

### Technology Preferences
- Static site generator preferred (11ty, Astro, or similar)
- Deploy to Netlify, Vercel, or similar
- No framework overhead unless justified
- CSS that's maintainable (vanilla CSS custom properties, or utility classes if needed)

---

## Visual Direction

**Note:** Visual branding assets will be created separately and integrated later. For now, build with placeholder/minimal styling that can be themed.

**The aesthetic territory:**
- 1977 vector graphics (Tempest, Star Wars arcade)
- Organic but alien — natural but not quite recognizable
- Structured but not rigid
- Not tech-startup clean
- Not portfolio-template generic

**For initial build:**
- Use a minimal, readable base
- Establish CSS custom properties for colors, typography, spacing that can be swapped later
- Leave clear integration points for visual assets (logo, illustrations, textures)

---

## What Success Looks Like

1. A visitor lands on the site
2. Within 10 seconds they understand: this person thinks in systems, not screens
3. They either:
   - Self-select out (good — they wanted a UI designer)
   - Dig deeper into case studies (good — they're the 5%)
4. The case studies demonstrate the pattern: vision → system → infrastructure
5. The article gives philosophical context for skeptics or the curious
6. Contact is simple and direct

---

## What to Avoid

- Generic portfolio templates
- "I'm passionate about user-centered design" language
- Process theater (showing sticky notes and workshop photos)
- Listing tools and software as credentials
- Any implication that Jim is looking for a traditional UX role

---

## Open Questions for Later

- Domain: strangelund.com? Something else?
- Visual assets: will be created via separate skill/process
- Case study visuals: system diagrams, not UI screenshots — approach TBD
- Mad Branch integration: Jim's woodworking practice may eventually appear, but not in v1

---

## Files Included

The following semantic HTML files contain the full written content:

```
case-studies/
├── southern-company-gas.html
├── mailchimp.html
├── drip.html
├── grammarly.html
├── rock-hall.html
├── stash-wealth.html
├── boston-gov.html
├── super-deluxe.html
└── why-i-stopped-calling-myself-a-ux-designer.html
```

Use these as the canonical source for all copy. The structure (headings, sections) should inform the page layout.

---

## Contact

James DiStefano  
Atlanta, GA  
jamesjdistefano@gmail.com  
LinkedIn: linkedin.com/in/jamesdistefano
