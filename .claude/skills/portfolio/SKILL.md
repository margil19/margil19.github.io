---
name: portfolio-margilgandhi
description: Use this skill when working on margilgandhi.com — the personal portfolio site. This includes adding/editing sections, updating content, fixing animations, deploying changes, or any task involving the portfolio HTML file. Triggers on mentions of "portfolio", "margilgandhi.com", "my site", "my website", or references to specific sections like hero, DNA helix, stats bar, testimonials, values, or about section.
---

# Portfolio Skill — margilgandhi.com

## Overview

Single-page HTML/CSS/JS portfolio deployed via **GitHub Pages** with a custom domain (margilgandhi.com) through **GoDaddy DNS**. The canonical source file is `index.html` in the GitHub repo `margilgandhi.github.io`.

---

## Site Structure (Top to Bottom)

1. **Navigation** — Sticky top bar. Links: Experience | Projects | Values | Skills | Education | About | Testimonials | Recommendations. No "Get in touch" button.

2. **Hero** — Large animated name display (MARGIL / GANDHI). Typewriter changing text: "I build products that..." with 5 rotating phrases (solve real problems, scale 0→1, empower users, create leverage, drive impact). Blinking cursor effect. No profile image. Everything centered — nothing should be left or right of the animation.

3. **Stats Bar** — 5 metrics with count-up animation on scroll:
   - $280K saved
   - $340K revenue
   - 2,500+ users
   - 8 Speaking Engagements
   - 6+ Years PM Experience

4. **Work / Experience** — Expandable cards for roles (Goldman Sachs PM, Sailsmith co-founder, CXtec).

5. **Projects** — AI tools and builds (Think Again, One Thing, Chorus/Lenny's Brain, Sailsmith, custom GPTs, AI agents, etc.).

6. **Values — DNA Helix** — 6 black cards with white text in a 3D rotating helix formation. Scroll-controlled rotation (200vh section height, 720° total rotation). No emojis. Values: Authenticity, Empathy First, Seek Truth Not Validation, Non-Zero-Sum Mindset, Learn by Doing, Relentless Curiosity.

7. **Skills** — Cards grouped by category. Must include AI-specific skills: RAG, MCP, AI Agents, Prompt Engineering, LLMs alongside PM and technical skills.

8. **Education** — Expandable. Syracuse University M.S.

9. **About** — Positioned before Testimonials. Personal tone, 3 short paragraphs. Focuses on who Margil is as a person, not a resume recap.

10. **Testimonials** — 18 testimonial cards in a Netflix-style horizontal scroll.

11. **Recommendations** — 2 full recommendation letters (Mary Collier, Jim Hazelton).

12. **Contact** — Bottom section.

---

## Design System

### Typography
- No generic fonts (no Inter, Roboto, Arial)
- The site uses a distinctive display font for headings and a clean body font
- Hero name is the largest element on the page

### Colors
- Predominantly white/light background
- Black cards for the Values DNA helix section
- Minimal accent colors — clean, editorial feel
- No purple gradients, no generic AI aesthetics

### Animations (3 key ones)
1. **Hero typewriter** — Changing text with blinking cursor, cycles through 5 phrases
2. **DNA helix rotation** — Scroll-controlled, 3D perspective, cards orbit in helix pattern
3. **Stats count-up** — Numbers animate from 0 to final value when scrolled into view

### Layout Principles
- Everything centered in the hero — no elements offset from the animation
- Generous whitespace between sections
- Cards-based UI for experience, projects, testimonials
- Responsive across desktop and mobile
- Netflix-style horizontal scroll for testimonials

---

## Rules When Editing

1. **Always preview before applying.** Show a standalone demo of any section change before modifying the final file. Margil reviews visually first.

2. **The base file is `portfolio-final__21_.html`** (renamed to `index.html` for deployment). Always work from this version.

3. **Do not remove or restructure existing animations** unless explicitly asked. The hero typewriter, DNA helix, and stats counter are intentional and tested.

4. **Section order matters.** About comes before Testimonials. Values (DNA helix) comes after Work/Projects. Don't rearrange without asking.

5. **Keep it a single HTML file.** No separate CSS or JS files. Everything inline. This is how it deploys on GitHub Pages.

6. **No emojis in the live site content.** The portfolio is clean and editorial.

7. **When adding new content** (projects, testimonials, skills), match the existing card structure and animation patterns — don't introduce new UI paradigms without discussion.

8. **Stats bar updates** — If metrics change, update both the display value and the `data-target` attribute used by the count-up script.

9. **New projects to add should include:** Project name, one-line description, tech stack used, and a quantified outcome where possible.

---

## Deployment

- **Hosting:** GitHub Pages (repo: `margilgandhi.github.io`)
- **Domain:** margilgandhi.com via GoDaddy DNS
- **Process:** Push `index.html` to the `main` branch → GitHub Pages auto-deploys in ~1-2 minutes
- **No build step.** Raw HTML served directly.

---

## Current AI Builds to Reference

When updating the Projects section, these are the builds to pull from:

- **Chorus (Lenny's Brain)** — RAG system, 270 episodes, Supabase + Voyage AI + Claude Sonnet + Next.js
- **Think Again** — AI reflection app, Lovable + Supabase + OpenAI
- **One Thing** — Micro-learning swipe app, GPT-4o + Pexels API
- **Sailsmith Phase 1** — React travel platform, 3 screens, 3000+ users
- **AI Follow-Up Agent** — Python + OpenAI APIs, automated recruiter follow-ups
- **Coffee Chat Scheduling Agent** — Flask + ngrok + webhooks
- **LinkedIn Knowledge Chatbot** — Flask + ChromaDB + Twilio + WhatsApp RAG
- **Custom GPTs** — Resume Review (1K+ chats), Cold Email (1K+ chats), Company Research (300+ chats)
- **Portfolio Site** — This site itself, HTML/CSS/JS, scroll animations, GitHub Pages
