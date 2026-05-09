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
- CSS custom properties in `:root` — full token system (colors, shadows, radii, font)
- Dark mode via `[data-theme="dark"]` on `<html>` — all tokens + components overridden
- Responsive breakpoints: 1024px · 900px · 768px · 480px
- Brand palette: purple `#8785FF` · orange `#FFA94D` · blue `#38B6FF` · pink `#D771FF`
- Font: Plus Jakarta Sans (Google Fonts)
- Key classes: `.process-grid` / `.process-step` / `.ps-1–4` (Process section); `.f-social` / `.f-social-link` (footer social icons)

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
