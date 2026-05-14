# CLAUDE.md — Chezka's Freelancer Profile

**Chezka (Franchezka N. Mendoza)** | ckmendoza.systems@gmail.com
**Niche:** Tech VA / AI Automation | **Education:** BS Psych, Adamson U (2022)
**Core Tools:** Zapier · Make.com · n8n · Claude · GoHighLevel

---

## Folders
- `MY PROJECTS/` — Sample project images: `GHL/` `MAKE.COM/` `N8N/` `ZAPIER/` ← read as portfolio proof
- `MY WORK EXPERIENCE/` — `resume/` (outdated) · `previous-work/`
- `portfolio-website/` — Static HTML/CSS/JS (`index.html` + `styles.css` + `favicon.svg`)
- `brand-assets/` — `headshot-gray-bg.jpg` (active, neutral gray bg) · `headshot.jpg` (original, warm bg) · brand visuals

> No folder called "SCREENSHOTS" — images live in the tool folders above.

---

## Portfolio Website
→ `Documents/portfolio-website/index.html` + `styles.css`
**Status: Fully built + polished.** All sections live and functional.

**Sections:** Nav · Hero · Tools Marquee · Pain · Services · Impact · Projects (desktop window) · About · Process · Results · CTA · Footer

**Section highlights:**
- **Nav:** Services · Projects · About · Process · Results (desktop + mobile hamburger; no Contact — Book a Call CTA covers it)
- **Hero:** "Stop Running Your Business on Manual." — animated chat widget, CTA to book a strategy call
- **Tools Marquee:** Auto-scrolling — Zapier · Make · n8n · GHL · Asana · Trello · Slack · Notion · Xero · Claude · OpenAI · Gemini · ElevenLabs · Airtable · GitHub · OpenRouter · Grok · Perplexity
- **Services:** eyebrow "WHAT I BUILD", heading "Automation, Done Right"; cards: GoHighLevel Systems · Zapier Automation · Make.com Workflows · n8n AI Agents
- **Impact stats:** 80% task reduction · <2 min lead follow-up · 10+ hrs/week saved · 5× more leads nurtured; headline "Less Manual Work. More Pipeline. Always On."; animated counters replay on every scroll in both directions (IntersectionObserver + cancelAnimationFrame, no once-only lock)
- **Projects:** eyebrow "MY WORK", heading "Systems Built to Deliver"; 20 systems across 6 categories — desktop-window UI with sidebar filter, list, preview pane, full modal per project (problem · steps · before/after · tools · gallery); modal gallery arrows + keyboard left/right arrows navigate images; gallery arrows fixed (symmetrical at left/right 10px, images have pointer-events: none)
- **About:** VA-turned-Automation Specialist, Philippines, 3+ years ops; uses `headshot-gray-bg.jpg`
- **Process** `id="process"`, eyebrow "MY PROCESS": 4-step — Discovery Call (free 30 min) → System Design → Build & Test → Launch & Handoff (30-day support); 4-col grid collapses 2-col @ 1024px, 1-col @ 768px
- **Contact/CTA:** All booking CTAs → `https://calendly.com/ckmendoza-systems/book-a-free-strategy-call`; email `ckmendoza.systems@gmail.com` stays as mailto
- **Footer:** 3-column — (1) brand logo + tagline + availability badge + location + LinkedIn/Upwork icons (subtle purple-to-blue gradient bg, purple icon color, `.f-social-link`); (2) Navigate (Services · Projects · About · Process · Results); (3) Specialties list; copyright bar with "Back to top ↑"
- **Meta/SEO:** title and og:title use `|` separator ("CK Mendoza | Automation Specialist"); og:description, og:type, twitter:card in `<head>`; `favicon.svg` (purple #8785FF, "CK" text); add `og:image` with absolute URL once deployed

**Interactive features (all in `index.html` `<script>`):**
- Dark mode toggle — sun/moon SVG; preference persists via `localStorage`; anti-FOUC inline script in `<head>`
- Mobile hamburger menu — slides in at ≤768px; closes on link click or outside tap
- Scroll-to-top button — fixed bottom-right, appears after 400px scroll
- Animated number counters — replays every IntersectionObserver entry; `cancelAnimationFrame` prevents overlap
- Project modal — gallery with arrows/dots/fullscreen + keyboard left/right arrow navigation; ≤900px clicking row opens modal directly; dark mode overrides on gallery arrows + fullscreen btn
- Chat widget — auto-cycling Q&A conversation in hero

**CSS architecture (`styles.css`):**
- CSS custom properties in `:root` — full token system (see Brand Assets below)
- Dark mode via `[data-theme="dark"]` on `<html>` — all tokens + components overridden
- Responsive breakpoints: 1024px · 900px · 768px · 480px
- Key classes: `.process-grid` / `.process-step` / `.ps-1–4` (Process section); `.f-social` / `.f-social-link` (footer social icons)

---

## Brand Assets

### Files
- `brand-assets/headshot-gray-bg.jpg` — **active** headshot, neutral gray bg (use this everywhere)
- `brand-assets/headshot.jpg` — original headshot, warm bg (do not use)
- `brand-assets/linkedin-banner.html` — dark LinkedIn banner (1584×396)
- `brand-assets/linkedin-banner-light.html` — light LinkedIn banner (1584×396)
- `portfolio-website/favicon.svg` — purple `#8785FF`, "CK" monogram text

### Typography
- **Font:** Plus Jakarta Sans — loaded from Google Fonts, weights 400/500/600/700/800
- **Fallback stack:** `'Plus Jakarta Sans', system-ui, sans-serif`
- **Headline (hero h1):** `clamp(40px, 6vw, 72px)`, weight 800, `letter-spacing: -2.5px`, `line-height: 1.08`
- **Section heading (`.sh2`):** `clamp(28px, 4vw, 46px)`, weight 800, `letter-spacing: -1.5px`, `line-height: 1.12`
- **Eyebrow:** `11px`, weight 700, `letter-spacing: 2.5px`, `text-transform: uppercase`, color: `--purple`
- **Body line-height:** 1.7; subtext `1.65`

### Color Tokens — Light Mode (`:root`)
```
--bg:           #ffffff
--bg-gray:      #f7f7f8
--text-primary: #111111
--text-second:  #555555
--text-muted:   #999999
--border:       rgba(0,0,0,0.07)

/* Purple */
--purple-pale:  #EBEBFF
--purple-light: #B5B4FF
--purple:       #8785FF   ← primary brand color
--purple-dark:  #6563D4

/* Orange */
--orange-pale:  #FFE7C2
--orange-light: #FFD699
--orange:       #FFA94D
--orange-dark:  #E07B00

/* Pink/Magenta */
--pink-pale:    #F7E4FF
--pink-light:   #E8AFFF
--pink:         #D771FF
--pink-dark:    #9B00CC

/* Blue */
--blue-pale:    #E0F2FF
--blue-light:   #7EC8FF
--blue:         #38B6FF
--blue-dark:    #1A9AE8
```

### Color Tokens — Dark Mode (`[data-theme="dark"]`)
```
--bg:           #0c0a1e
--bg-gray:      #161428
--text-primary: #f0eeff
--text-second:  rgba(240,238,255,0.62)
--text-muted:   rgba(240,238,255,0.38)
--border:       rgba(255,255,255,0.08)

--purple-pale:  rgba(135,133,255,0.15)
--orange-pale:  rgba(255,169,77,0.15)
--pink-pale:    rgba(215,113,255,0.15)
--blue-pale:    rgba(56,182,255,0.15)
--purple-light: #9d9bff
```

### Shadows & Radii
```
--shadow:    0 1px 2px rgba(0,0,0,0.04), 0 4px 12px rgba(0,0,0,0.06)
--shadow-lg: 0 2px 6px rgba(0,0,0,0.03), 0 16px 40px rgba(0,0,0,0.09)

--radius-sm: 6px
--radius-md: 10px
--radius-lg: 16px
--radius-xl: 24px
```

### Key Gradients
- **Hero / LinkedIn banner (light):** `linear-gradient(150deg, #ffffff 0%, #f4f1ff 30%, #edf7ff 62%, #fffaf2 100%)`
- **Hero (dark):** `linear-gradient(150deg, #0c0a1e 0%, #14103a 30%, #0e1630 62%, #15100d 100%)`
- **LinkedIn banner (dark):** `linear-gradient(135deg, #0a0718 0%, #150d35 40%, #1e1050 70%, #2a1870 100%)`
- **Primary CTA button:** `linear-gradient(135deg, #6563D4 0%, #8785FF 55%, #38B6FF 100%)`
- **Accent gradient (dark banner headline):** `linear-gradient(90deg, #8785FF 0%, #D771FF 100%)`

### Tool Brand Colors (badge backgrounds)
- **GHL:** `#0056B3` (blue)
- **Zapier:** `#FF6B2B` (orange)
- **Make.com:** `#6E00CC` (purple)
- **n8n:** `#EA4B71` (pink-red)

### Design Patterns
- Eyebrow labels always in purple (`--purple`), uppercase, tracked at 2.5px
- Cards use `border-top: 3px solid [accent color]` to color-code by tool/category
- Pill/badge shape: `border-radius: 100px`
- Orb blobs (blurred radial gradients) appear in hero and banner backgrounds as subtle depth
- Dark mode toggle: sun icon (light) / moon icon (dark), persisted via `localStorage`
- Availability indicator: `#22c55e` green dot + "Available Now" text

---

## Sample Projects (20 total)
- **GHL (6):** Appointment Booking · HVAC Landing Page · AI Bot "Anna" · 6-Workflow System · Courses · Payments & Funnels
- **Zapier (5):** Content Repurposing · CRM Lead Engagement · Lead Enrichment · Lead Intake · Booking & Reminder
- **Make.com (5):** Financial Reports · AI Doc Workflow · Social Media System · Candidate Screening · PDF Extraction
- **n8n (5):** FB Messenger Chatbot · Job Scraper · AI Newsletter · Autonomous Email Agent · Resume Screening

---

## Work Experience
Full finalized descriptions → `MY PROJECTS/upwork-descriptions.md` (reuse for all platforms)
1. Real Estate VA/TC — Amanda Nadia Group (Jun 2025–Apr 2026)
2. Real Estate Executive Assistant — 5-Agent Team (May 2024–Apr 2025)
3. Virtual Assistant — Nexa Mortgage nationwide (Aug 2021–May 2024)
4. HR Administrative Associate — 1,000+ Employee Org (Jan 2023–Jul 2023)

---

## Upwork Profile
- **Title:** AI Automation Expert - Zapier, Make.com, n8n, GoHighLevel ✓
- **15 Skills ✓:** Zapier · Make.com · n8n · Claude · HighLevel · Automation · AI Chatbot · Chatbot Development · Automated Workflow · CRM Automation · Email Automation · Business Process Automation · Sales Funnel · AI Agent Development · Marketing Automation
- **Links:** LinkedIn → `linkedin.com/in/ck-mendoza` · Upwork → `upwork.com/freelancers/~017c106844b4241997`
- **Pending:** Overview/bio · Portfolio · Hourly rate

---

## Rules
- Outputs = client-facing, professional, conversion-focused
- Use results-focused language with real numbers (contacts, hours, scale)
- Always connect work experience to tech/automation angle
- Read images in `MY PROJECTS/` as portfolio proof points when needed
- No em dashes in client-facing website content; use commas, colons, or periods instead
- Only update this CLAUDE.md when Chezka explicitly asks
