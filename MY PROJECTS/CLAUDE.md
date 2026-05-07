# CLAUDE.md — Chezka's Freelancer Profile

**Chezka (Franchezka N. Mendoza)** | ckmendoza.systems@gmail.com
**Niche:** Tech VA / AI Automation | **Education:** BS Psych, Adamson U (2022)
**Core Tools:** Zapier · Make.com · n8n · Claude · GoHighLevel

---

## Folders
- `MY PROJECTS/` — Sample project images: `GHL/` `MAKE.COM/` `N8N/` `ZAPIER/` ← read as portfolio proof
- `MY WORK EXPERIENCE/` — `resume/` (outdated) · `previous-work/`
- `portfolio-website/` — Static HTML/CSS/JS (`index.html` + `styles.css`)
- `brand-assets/` — headshot.jpg and brand visuals

> No folder called "SCREENSHOTS" — images live in the tool folders above.

---

## Portfolio Website
→ `Documents/portfolio-website/index.html` + `styles.css`
**Status: Fully built + polished.** All sections live and functional.

**Sections:** Nav · Hero · Tools Marquee · Pain · Services · Impact · Projects (desktop window) · About · Results · CTA · Footer

**Section highlights:**
- **Hero:** "Stop Running Your Business on Manual." — animated chat widget, CTA to book a strategy call
- **Tools Marquee:** Auto-scrolling strip — Zapier · Make · n8n · GHL · Asana · Trello · Slack · Notion · Xero · Claude · OpenAI · Gemini · ElevenLabs · Airtable · GitHub · OpenRouter · Grok · Perplexity
- **Services:** GoHighLevel Systems · Zapier Automation · Make.com Workflows · n8n AI Agents
- **Impact stats:** 80% task reduction · <2 min lead follow-up · 10+ hrs/week saved · 5× more leads nurtured ← animated counters on scroll
- **Projects:** 20 systems across 6 categories — desktop-window UI with sidebar filter, list, preview pane, full modal per project (problem · steps · before/after · tools · gallery)
- **About:** VA-turned-Automation Specialist, Philippines, 3+ years ops
- **Contact/CTA:** All booking CTAs (Book a Call · Book a Free Call · Book a Free Strategy Call · Work With Me · Build Similar System) → `https://calendly.com/ckmendoza-systems` (opens in new tab); displayed email `ckmendoza.systems@gmail.com` stays as mailto
- **Footer:** 3-column — (1) brand logo + tagline "Automation Specialist building workflows that run 24/7" + green availability badge + location; (2) Navigate links (Services · Projects · About · Results); (3) Specialties plain list (Zapier · Make.com · n8n · GHL); copyright bar with "Back to top ↑" — no CTAs or email (handled by CTA section above); Results section has `id="results"` anchor

**Interactive features (all in `index.html` `<script>`):**
- Dark mode toggle — sun/moon SVG button upper-right nav; preference persists via `localStorage`; anti-FOUC inline script in `<head>`
- Mobile hamburger menu — slides in at ≤768px; closes on link click or outside tap
- Scroll-to-top button — fixed bottom-right, appears after 400px scroll, purple hover
- Animated number counters — `IntersectionObserver` triggers ease-out count-up (1.6s) + pop bounce when Impact section enters view; uses `data-count` / `data-prefix` / `data-suffix` on `.impact-num`
- Project modal — gallery with arrows/dots/fullscreen; on ≤900px clicking a project row opens modal directly (preview pane hidden); gallery arrows + fullscreen button have explicit dark mode overrides (dark bg, white text) so they're visible and clickable in dark mode
- Chat widget — auto-cycling Q&A conversation in hero

**CSS architecture (`styles.css`):**
- CSS custom properties in `:root` — full token system (colors, shadows, radii, font)
- Dark mode via `[data-theme="dark"]` on `<html>` — overrides all tokens + component colors; `.btn-white` forced to `color: #1a1840` in dark mode (prevents near-white text on white bg); `.gallery-arrow` and `.fullscreen-btn` get dark semi-transparent backgrounds in dark mode
- Responsive breakpoints: 1024px · 900px · 768px · 480px
- Brand palette: purple `#8785FF` · orange `#FFA94D` · blue `#38B6FF` · pink `#D771FF`
- Font: Plus Jakarta Sans (Google Fonts)

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
- **Work experience descriptions:** Finalized ✓
- **Pending:** Overview/bio · Portfolio · Hourly rate

---

## Rules
- Outputs = client-facing, professional, conversion-focused
- Use results-focused language with real numbers (contacts, hours, scale)
- Always connect work experience to tech/automation angle
- Read images in `MY PROJECTS/` as portfolio proof points when needed
- Only update this CLAUDE.md when Chezka explicitly asks
