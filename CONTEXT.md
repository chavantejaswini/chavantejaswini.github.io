# Tejaswini Chavan — Portfolio CONTEXT.md
> Handoff for Claude Code. Read this before touching anything.

---

## What This Is
A single-file HTML portfolio targeting AI Engineering hiring managers. Dark-theme, animated, single-page. Quality benchmark: https://rajnikantportfolio.netlify.app

**Live URL:** https://chavantejaswini.github.io (GitHub Pages — auto-deploys from `main` branch)
**Repo:** https://github.com/chavantejaswini/chavantejaswini.github.io

---

## Owner Profile

**Name:** Tejaswini Chavan (goes by Teju)
**Role targeting:** AI Full-Stack Engineer / AI Engineer
**Location:** Boston, MA (open to remote)
**Email:** chavan.t@northeastern.edu
**Phone:** 720-757-3690
**LinkedIn:** https://linkedin.com/in/tejaswini-chavan/
**GitHub:** https://github.com/chavantejaswini
**Medium:** https://medium.com/@tejaswinitchavan16
**Status:** Graduating May 2026, F-1/OPT authorized, H-1B sponsorship required

---

## File Structure
```
index.html                        ← THE live file (GitHub Pages serves this)
tejaswini_portfolio_final.html    ← kept in sync with index.html
CONTEXT.md                        ← this file
```
**Always edit `index.html`. Run `cp index.html tejaswini_portfolio_final.html` before committing.**

---

## How to Deploy
GitHub Pages auto-deploys on every push to `main`. No manual step needed.
To push: `git add index.html tejaswini_portfolio_final.html && git commit -m "..." && git push`

---

## Tech Stack Used in Portfolio
- **Fonts:** Plus Jakarta Sans (headings) + DM Sans (body) + JetBrains Mono (code/tags)
- **Icons:** Devicons CDN — `https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/`
- **Badges:** shields.io static badges in GitHub section
- **CSS:** Pure CSS with CSS variables, no frameworks
- **JS:** Vanilla JS — IntersectionObserver reveals, counter animations, skill bars, 3D tilt, hamburger menu, nav highlight
- **No build step** — single HTML file, fully self-contained with base64 headshot

---

## CSS Variables (Design Tokens)
```css
--bg: #07071a        /* page background */
--bg2: #0d0d22       /* alternate section bg */
--card: #0e0e22      /* card background */
--v: #7c3aed         /* violet primary */
--vl: #a855f7        /* violet light */
--c: #06b6d4         /* cyan accent */
--t: #f0f0fa         /* primary text */
--tm: #8888bb        /* muted text */
--bd: #1e1e38        /* border color */
```

---

## Sections (in order)

1. **nav** — sticky, blur backdrop, logo `TC.ai`, section links + hamburger on mobile
2. **#hero** — split grid (1fr 460px): left (name, title, quote, stats, devicon stack tags) | right (profile card with floating tech badges)
3. **#about** — bio + metrics + bento tech stack cards (AI/ML, Backend, Cloud, Data, Salesforce)
4. **#skills** — 3-col skill groups with animated progress bars
5. **#exp** — experience cards (5 entries)
6. **#proj** — 7 project cards with pipeline flow diagrams
7. **#github-contrib** — GitHub section (stats, language bar, 6 repo cards, shields badges)
8. **#thought** — 4 thought leadership cards (2 Medium, 2 LinkedIn)
9. **#linkedin** — 4 LinkedIn post cards
10. **#phil** — 4 design philosophy cards
11. **#arch** — 4 clickable AI capability cards
12. **#tl-section** — alternating career timeline
13. **#certs** — certification cards
14. **#education** — education cards
15. **#resume** — resume download CTA
16. **#contact** — final CTA
17. **footer**

---

## Visual / UI Features Added

### 3D Effects
- **Card tilt** — all `.pc`, `.gh-card`, `.certcard`, `.ec`, `.archcard`, `.phc`, `.tlcard`, `.lpcard`, `.sc` tilt toward cursor on mousemove using `perspective(700px) rotateY/X` with directional shadow
- **Floating tech badges** — 5 badges (Python, React, AWS, TypeScript, Docker) float around the hero profile card using `@keyframes ftfloat`

### Icons
- **Favicon** — ⚡ lightning bolt SVG emoji
- **Hero stack tags** — devicon images (Python, TypeScript, React, AWS, Terraform, Docker, PostgreSQL, MongoDB)
- **About tech cards** — 3 large devicons (36px) per card + individual tech pills each with micro devicon (13px)
- **Floating badges** — devicon images in animated hero badges

### Tech Stack Cards (bento style)
Each `.sc` card has:
- Colored top accent bar via `::before` (unique gradient per category)
- `--sc-accent` CSS var for gradient: purple (AI/ML), cyan-blue (Backend), orange-yellow (Cloud), green (Data), Salesforce-blue (Ecosystem)
- 3 large header icons + category title
- Individual `.sc-pill` tags for each technology with hover effect

### Section Labels (`.slb`)
- `font-size: clamp(1rem, 1.3vw, 1.15rem)`, `font-weight: 800`
- Purple accent line via `::before` (28px × 2px)
- `letter-spacing: .22em`, `text-transform: uppercase`

### Section Padding
- `section { padding: 160px 5%; }`

---

## GitHub Section (`#github-contrib`)

**Stats:** 30+ repos, 6 languages, 15mo streak, active since 2024

**Language bar:** Python 55%, JavaScript 20%, TypeScript 11%, Java 8%, HCL 4%, Other 2%

**Repo cards shown** (all distinct from Key Projects section):
1. AI Rate My Professor — TypeScript, Next.js, Pinecone
2. Fundflow Finance Manager — JavaScript, React
3. AI SaaS Flashcard App — JavaScript, Generative AI, Stripe
4. CVS Pharmacy UX Redesign — UX Research, Figma
5. Library Management System — Java, OOP
6. Northeastern Fitness Hub — Java, campus app

**Shields.io badges:** GitHub profile, 30+ repos, Python Expert, TypeScript Advanced, AWS/Terraform, Active Since

---

## Thought Leadership

**Medium articles** (real):
- "Shopping Cart Abandonment: Challenges & Solutions for CVS Online Drugstore" — https://medium.com/@tejaswinitchavan16/shopping-cart-abandonment-challenges-and-solutions-for-cvs-online-drugstore-ad31b72dbf57

**LinkedIn posts** (placeholder URLs — link to profile root until real post URLs available):
- "Building Self-Evolving Agent Systems: Lessons from V1 to V3"
- "AWS Infrastructure Consolidation with Terraform: A Real Startup Story"
- "Why Your RAG System Needs Per-User Signal Weights"
- 4 LinkedIn post cards in `#linkedin` section

---

## Profile Card (hero right column)
- Photo: 190×190px base64 JPEG, `object-position: 50% 10%`
- Name: 1.3rem, weight 800
- Role: 0.95rem cyan
- Available badge: 0.8rem green
- Skill tags (ptag): 0.76rem
- Info rows (pi): 0.9rem — includes email, location, education, roles, LinkedIn, GitHub
- Wrapped in `.float-wrap` for floating badge positioning

---

## Experience Entries

1. **Graduate Research Assistant** — Northeastern University × NGI, Inc | Jan 2026 – Apr 2026
2. **AI/ML Engineer Intern (Co-op)** — NGI, Inc (Stealth Startup) | Sept 2025 – Dec 2025
3. **AI Software Engineering Fellow** — Headstarter AI | Jul 2024 – Aug 2024
4. **Software Engineer** — Avalara Technologies | Jul 2021 – Dec 2023
5. **Software Engineering Intern** — Avalara Technologies | Dec 2020 – Jun 2021

---

## Projects (Key Projects section)

1. Financial Advisor Copilot — Python, FastAPI, React/TypeScript, Salesforce SOQL
2. ML Agent Integration Layer — FastAPI, multi-agent, pgvector, Supabase
3. SmartScreen ATS — OpenAI embeddings, cosine similarity → `/Candidate-Recommendation-Engine`
4. AutoQA Multi-Agent System — LangChain, Agents-S → `/Agent-S`
5. CloudNative IaC — Terraform, Packer, AWS → `github.com/CSYE-6225Cloud2025Tejaswini`
6. Pantry Tracker AI — GCP Vertex AI, Next.js, LLaMA
7. AI Customer Support Chatbot — RAG, LangChain, Pinecone → `/AI-Powered-Chatbot`

---

## Certifications
- AWS Solutions Architect Associate ✓
- Salesforce AI Specialist ✓
- Headstarter AI Fellowship ✓
- Memory Threading — Published Article (Humanitarians AI · Northeastern) ✓
- Salesforce Platform Developer (LWC · Apex · SOQL · SOSL) ✓
- AWS Activate Founders (awarded 2025) ✓

---

## Education
- **MS Information Systems** — Northeastern University, Sep 2024 – May 2026
  - Supervised by Prof. Nik Bear Brown, INFO 7945 Master's Project
  - Coursework: Gen AI, Multi-Agent Systems, DBMS, Microservices, UIUX
- **B.E. Computer Science Engineering** — Shivaji University, Jun 2016 – May 2020

---

## Known Issues / TODO

### 🔴 Still Open
- **Resume download button** — `href="#"` is a placeholder. Replace with real hosted PDF URL.
- **Thought Leadership LinkedIn URLs** — most link to profile root. Update with real post URLs when published.
- **OG meta tags** — add `og:title`, `og:image`, `og:description` for LinkedIn/Slack unfurls.

### 🟡 Nice to Have
- Light mode toggle
- Real project screenshots or visual previews for project cards
- More Medium articles published → update Thought Leadership section

### ✅ Resolved
- Skill bar animation (double rAF fix) ✓
- Font size clamp on `.slb`, `.etag`, `.apill` ✓
- Hero 1100px breakpoint ✓
- Hamburger mobile menu ✓
- Visa details removed ✓
- Headstarter AI removed from education ✓
- Section spacing (160px padding) ✓
- Section labels large + accent bar ✓
- GitHub section added ✓
- Medium article linked ✓
- AWS cert present ✓
- Stripe in Flashcard SaaS ✓
- Devicons in hero, about cards, floating badges ✓
- 3D card tilt on all card types ✓
- GitHub Pages deployed ✓

---

## Key Metrics (hiring manager magnets)
- 95% precision on production knowledge graph at 200+ queries/second
- 86% thread connectivity across 535 moments / 1,024 relationships
- 78% keyword coverage on hybrid NER pipeline
- 500ms end-to-end latency on multi-agent NLP pipeline
- 6 hours/week saved per financial advisor
- 35% faster data processing @ Avalara
- 70% reduction in tax processing time @ Avalara
- 99.9% data accuracy on Kafka pipeline

---

## Notes for Claude Code
- All CSS: single `<style>` block in `<head>`
- All JS: bottom before `</body>` — two `<script>` blocks (main logic + fallback setTimeout)
- `.rv` = reveal class (`opacity:0; transform:translateY(22px)`) → gets `.vis` from IntersectionObserver
- `.rv1/.rv2/.rv3` = staggered delay variants (0.1s / 0.2s / 0.3s)
- `data-t="N"` + `data-suffix="X"` on stat numbers = counter animation target
- `data-w="N"` on `.skfill` = skill bar target width %
- `.ftag` = floating hero badge with `--fd` CSS var for animation delay
- `.sc-pill` = individual tech pill in about bento cards
- `--sc-accent` = CSS var on each `.sc` card for top gradient bar color
