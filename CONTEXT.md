# Tejaswini Chavan — Portfolio CONTEXT.md
> Handoff for Claude Code. Read this before touching anything.

---

## What This Is
A single-file HTML portfolio (`tejaswini_portfolio_final.html`) built to match the quality and structure of https://rajnikantportfolio.netlify.app. It's a dark-theme, animated, single-page portfolio targeting AI Engineering hiring managers.

**Current live draft:** https://serene-concha-20feb5.netlify.app/ (old Netlify AI version — ignore this, it's wrong)
**Current file:** `tejaswini_portfolio_final.html` — this is the real one.

---

## Owner Profile

**Name:** Tejaswini Chavan (goes by Teju)
**Role targeting:** AI Full-Stack Engineer / AI Engineer
**Location:** Boston, MA (open to remote)
**Email:** chavan.t@northeastern.edu
**Phone:** 720-757-3690
**LinkedIn:** https://linkedin.com/in/tejaswini-chavan/
**GitHub:** https://github.com/chavantejaswini
**Status:** Graduating May 2026, F-1/OPT authorized, H-1B sponsorship required

---

## Tech Stack Used in Portfolio
- **Fonts:** Plus Jakarta Sans (headings/display) + DM Sans (body) + JetBrains Mono (code/tags)
- **CSS:** Pure CSS with CSS variables, no frameworks
- **JS:** Vanilla JS — IntersectionObserver for reveal animations, counter animations, skill bar fills, nav highlight
- **No build step** — single HTML file, fully self-contained with base64-embedded headshot photo

---

## CSS Variables (Design Tokens)
```css
--bg: #07071a        /* page background */
--bg2: #0d0d22       /* alternate section bg */
--card: #0e0e22      /* card background */
--v: #7c3aed         /* violet primary */
--vl: #a855f7        /* violet light */
--c: #06b6d4         /* cyan accent */
--cl: #22d3ee        /* cyan light */
--t: #f0f0fa         /* primary text */
--tm: #8888bb        /* muted text */
--bd: #1e1e38        /* border color */
```

---

## Sections (in order)

1. **nav** — sticky top nav with logo `TC.ai`, section links, `⚡ Hire Me` CTA
2. **#hero** — split layout: left (name, title, quote, buttons, stats, tech stack tags) | right (profile card with photo + contact info)
3. **#about** — 4-paragraph rich bio + 4-stat metrics row + 2-col stack grid + Salesforce ecosystem card
4. **#skills** — 3-col skill groups with animated progress bars
5. **#exp** — experience cards (5 entries, see below)
6. **#proj** — project cards with pipeline flow diagrams (7 projects)
7. **#thought** — 4 thought leadership article cards
8. **#linkedin** — 4 LinkedIn post cards
9. **#phil** — 4 design philosophy cards
10. **#arch** — 4 clickable AI capability cards
11. **#tl-section** — alternating timeline
12. **#certs** — certification cards
13. **#education** — education cards (separate from certs)
14. **#resume** — resume download CTA section
15. **#contact** — final CTA with email/LinkedIn/GitHub
16. **footer**

---

## Experience Entries (correct order & titles from resume)

1. **Graduate Research Assistant** — Northeastern University × NGI, Inc | Jan 2026 – Apr 2026
   - Directed-graph multi-agent architecture, 3 agents + shared state bus, 500ms latency
   - OpenClaw autonomous agent framework
   - SynthesisAgent → CrewAI researcher agent, cross-session memory
   - AWS infra: Terraform, App Runner, RDS, Lambda, S3, CloudFront

2. **AI/ML Engineer Intern (Co-op)** — NGI, Inc (Stealth Startup) | Sept 2025 – Dec 2025
   - Production knowledge graph: fuzzy matching + vector similarity + rule-based = 95% precision, 200+ queries/sec
   - Memory Threading: PostgreSQL BFS + HuggingFace Sentence-Transformers = 86% thread connectivity, 535 moments, 1,024 relationships
   - Hybrid NER: spaCy + BERT, 78% keyword coverage

3. **AI Software Engineering Fellow** — Headstarter AI | Jul 2024 – Aug 2024
   - LangChain + Pinecone + AWS Bedrock chatbot, 35% resolution accuracy, 99.9% uptime
   - RAG professor recommendation system, 90+ reviews

4. **Software Engineer** — Avalara Technologies | Jul 2021 – Dec 2023
   - 3 Salesforce LWC interfaces, 35% faster data retrieval
   - Oracle Eloqua + Salesforce CRM integration (lead scoring, nurturing, campaign attribution)
   - Node.js pipelines + ML anomaly detection + Redis caching, 200ms API improvement
   - Java/Spring Boot + Postgres, 35% faster processing; tax workflow automation, 70% reduction
   - CI/CD: Packer + GitHub + Amazon CodeDeploy, 30% fewer deployment failures

5. **Software Engineering Intern** — Avalara Technologies | Dec 2020 – Jun 2021
   - Java/Spring Boot + Postgres, 35% faster data processing
   - Python + Apache Kafka pipeline, 99.9% data accuracy
   - A/B testing framework, 20% user engagement improvement
   - Sentry error logging, 60% faster issue resolution

---

## Projects (correct order)

1. **Financial Advisor Copilot** — Python, FastAPI, React/TypeScript, Streamlit, Docker, Salesforce (Mar 2026)
   - 3-agent pipeline (Access, Connection, Summary), live Salesforce SOQL integration
   - Human-in-the-loop accountability layer, AI briefings under 60 seconds
   - Saves financial advisors 6 hours/week
   - Pipeline: Salesforce CRM → 3-Agent Pipeline → Human-in-Loop → AI Briefing <60s

2. **ML Agent Integration Layer** — Production @ Node startup
   - FastAPI multi-agent system V1→V3, SharedContext state bus
   - Pipeline: Moments → NLP Pipeline → Priority Agent → Supabase

3. **SmartScreen ATS** — OpenAI embeddings + GPT-3.5, cosine similarity ranking
   - Pipeline: Resume → OpenAI Embed → Cosine Rank → Top Matches

4. **AutoQA Multi-Agent System** — LangChain, Agents-S framework
   - Pipeline: Test Case → Planner → Executor → Verifier

5. **CloudNative IaC** — Terraform + Packer, 20% faster deployment
   - Pipeline: Code Push → Terraform → Packer AMI → AWS Deploy

6. **Pantry Tracker AI** — GCP Vertex AI AutoML, 92% accuracy, Next.js + Firebase
   - Pipeline: Photo → Vertex AI → Item ID → LLaMA Recipe

7. **AI Customer Support Chatbot** — RAG + LangChain + Pinecone + AWS Bedrock
   - Pipeline: Query → Pinecone RAG → Claude/GPT-4 → Response

---

## Certifications
- AWS Solutions Architect Associate
- Salesforce AI Specialist
- Headstarter AI Fellowship
- Memory Threading — Published Article (Humanitarians AI · Northeastern)
- Salesforce Platform Developer (LWC · Apex · SOQL · SOSL)
- AWS Activate Founders (awarded 2025)

---

## Education
- **MS Information Systems** — Northeastern University, Sep 2024 – May 2026
  - Supervised by Prof. Nik Bear Brown, INFO 7945 Master's Project
  - Coursework: Gen AI, Multi-Agent Systems, DBMS, Microservices, UIUX
- **B.E. Computer Science Engineering** — Shivaji University, Jun 2016 – May 2020
- **Headstarter AI Fellowship** — 2024, Full-Stack AI Engineering

---

## Known Issues to Fix in Claude Code

### 🔴 HIGH PRIORITY
1. **Sections not rendering** — skills grid and experience cards were blank in Chrome (opacity:0 stuck). JS IntersectionObserver was partially broken after terminal removal. A fallback `setTimeout` was added but needs proper testing across browsers.

2. **Font size hierarchy** — Plus Jakarta Sans looks great but some nested card text (`.si3`, `.etag`, `.apill`) is still too small on large monitors. Needs a responsive type scale using `clamp()`.

3. **Hero layout on medium screens (960px–1200px)** — the profile card on the right gets squished before the breakpoint kicks in. Add an intermediate breakpoint around 1100px.

4. **Skill bars** — `data-w` attribute drives width but the CSS transition `width 1.1s ease` sometimes doesn't fire on first load if the section is already in viewport. Fix by checking `getBoundingClientRect` on DOMContentLoaded.

### 🟡 MEDIUM PRIORITY
5. **Thought Leadership / LinkedIn Posts** — these are placeholder content. Teja needs to either:
   - Write real LinkedIn post URLs and link them
   - Or replace with a "Coming Soon" state if not published yet

6. **Resume download button** — `href="#"` is a placeholder. Replace with an actual hosted PDF URL (Google Drive, Dropbox, or Netlify-hosted PDF alongside the HTML file).

7. **Project GitHub links** — most point to `https://github.com/chavantejaswini` (profile root). Should point to specific repos:
   - SmartScreen ATS: `/Candidate-Recommendation-Engine`
   - AutoQA: `/Agent-S`
   - CloudNative IaC: `github.com/CSYE-6225Cloud2025Tejaswini`
   - Chatbot: `/AI-Powered-Chatbot`
   - Financial Copilot: needs real repo URL

8. **Timeline section** — ID is `#tl-section` but nav links to `#tl`. Causes scroll mismatch. Either rename section ID or update nav href.

9. **Avalara intern dates** — currently says Dec 2020 – Jun 2021. Resume says Dec 2020 – Jun 2021 ✓ but double check.

### 🟢 NICE TO HAVE
10. **Add a real photo** — headshot is embedded as base64 (130×130px, cropped square from top). If you want a larger/better crop, re-run the Python resize script with `object-position` adjusted.

11. **Mobile nav** — nav links are hidden on mobile (`display:none`). Add a hamburger menu or mobile-friendly bottom nav.

12. **OG meta tags** — add `<meta property="og:title">`, `<meta property="og:image">`, etc. so LinkedIn/Slack unfurls look good when Teja shares her portfolio URL.

13. **Dark mode is only mode** — no light mode toggle. Could add one later.

---

## File Structure
```
tejaswini_portfolio_final.html   ← THE file (81KB, single-file, self-contained)
CONTEXT.md                        ← this file
```

---

## How to Deploy
1. Go to **app.netlify.com** → Add new site → Deploy manually
2. Drag `tejaswini_portfolio_final.html` into the drop zone
3. Done — live URL in 30 seconds
4. To add custom domain: Netlify → Domain settings → Add custom domain

**DO NOT** use Netlify's "Generate with AI / Claude" builder — it will regenerate a new generic portfolio and discard this file.

---

## Key Metrics to Highlight (hiring manager magnets)
- 95% precision on production knowledge graph at 200+ queries/second
- 86% thread connectivity across 535 moments / 1,024 relationships
- 78% keyword coverage on hybrid NER pipeline
- 500ms end-to-end latency on multi-agent NLP pipeline
- 6 hours/week saved per financial advisor (Financial Copilot)
- 35% faster data processing @ Avalara
- 70% reduction in tax processing time @ Avalara
- 99.9% data accuracy on Kafka pipeline
- 35% resolution accuracy improvement on RAG chatbot

---

## Notes for Claude Code
- All CSS is inside a single `<style>` block in `<head>`
- All JS is at the bottom before `</body>` — two `<script>` blocks (main + fallback)
- The headshot photo is embedded as a base64 data URI directly in the `<img src="">` — about 17KB
- `.rv` = reveal class (starts `opacity:0; transform:translateY(22px)`) — gets `.vis` added by IntersectionObserver
- `.rv1`, `.rv2`, `.rv3` = staggered delay variants (0.1s, 0.2s, 0.3s)
- `data-t="N"` on stat numbers = target value for counter animation
- `data-w="N"` on `.skfill` divs = target width % for skill bars
