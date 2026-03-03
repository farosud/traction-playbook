---
title: "15. Existing Platforms"
layout: default
parent: Home
nav_order: 16
---


# Existing Platforms — Traction Channel 15

## Service Layer
Services this channel can leverage (check user's configured API keys):
- **Exa.ai**: research what products succeeded on each platform, find launch timing patterns, discover platform-specific audiences
- **Firecrawl**: scrape platform listing pages, extract competitor positioning, analyze successful launches
- **Serper**: research platform algorithms, find launch playbooks, discover ranking factors per platform
- **Apify/SociaVault**: monitor platform activity, track competitor listings, measure engagement patterns

If a service is available, USE IT to ground recommendations in real data rather than generic advice.


## On Invocation

When `/traction platforms` is called:

### Step 1: Gather Context
Ask for (if not already provided):
- Product name, URL, one-liner
- Target audience description
- What platforms they've already tried
- Launch timeline (when they want to go live)
- Whether the product is technical or non-technical

### Step 2: Platform Mapping
Map ALL relevant platforms for their specific product and audience:

```
LAUNCH PLATFORMS (one-time events):
  Product Hunt     — tech products, biggest single-day traffic spike possible
  Hacker News      — technical audience, Show HN format, merit-based
  Indie Hackers    — bootstrapped/indie products, community-driven
  BetaList         — pre-launch signup collection
  Launching Next   — startup directory
  There's An AI    — AI-specific product directory
  Futurepedia      — AI tools directory

ONGOING PLATFORMS (sustained presence):
  Reddit           — niche communities, authentic participation required
  Twitter/X        — build in public, tech/startup audience
  LinkedIn         — B2B, professional audience
  YouTube          — demos, tutorials, thought leadership
  TikTok           — short-form product demos, younger audience

MARKETPLACE PLATFORMS (distribution):
  ChatGPT Plugin Store  — if AI-powered
  Slack App Directory   — if team/productivity tool
  Notion Templates      — if workflow/productivity
  GitHub               — if open source component
  VS Code Marketplace  — if developer tool
  Chrome Web Store     — if browser extension
  Zapier/Make          — if automation/integration
```

### Step 3: Platform-Specific Strategies

For EACH relevant platform, provide:

**Product Hunt Launch Playbook:**
- Pre-launch: build hunter relationships, collect supporters, prep assets
- Launch day: timing (12:01 AM PT), first hour strategy, comment engagement
- Assets needed: tagline, description, 5 images/GIFs, maker comment, first comment
- Post-launch: respond to every comment, share on social, follow up with upvoters
- Common mistakes: launching on wrong day, not having a community ready, bad assets

**Hacker News (Show HN) Strategy:**
- Title format that works: "Show HN: [Product] – [what it does in plain English]"
- Lead with technical depth, not marketing speak
- Comment strategy: respond thoughtfully to every question
- Best times: Tuesday-Thursday, 6-10 AM ET
- What gets flagged: anything that sounds like an ad

**Reddit Strategy:**
- NEVER post and run. Be a genuine community member FIRST (2+ weeks)
- Find 5-10 relevant subreddits, understand each culture
- Launch post format: tell the story, show the product, ask for feedback
- Comment karma matters — build it before posting
- r/startups, r/SaaS, r/indiehackers, r/sideproject + niche subs

**Indie Hackers Strategy:**
- Product listing + milestone posts
- Build in public updates (revenue, users, decisions)
- Engage in other people's threads FIRST
- The community rewards authenticity and transparency

**Build-in-Public (Twitter/X) Strategy:**
- Daily/weekly updates on metrics, decisions, learnings
- Share behind-the-scenes of product development
- Engage with other builders — reciprocity matters
- Thread format for deep dives on specific decisions
- Quote tweet and engage with relevant conversations

**AI Directory Listings:**
- There's An AI For That, Futurepedia, AI Tool Directory
- These are SEO plays — they rank well for "[category] AI tool"
- Submit to 10-15 directories, each takes 5 minutes
- Update listings quarterly as product evolves

### Step 4: Launch Calendar
Create a coordinated launch sequence:

```
WEEK -2: Pre-launch
  - Submit to BetaList, directories
  - Build Product Hunt supporter list (aim for 100+)
  - Start Reddit/IH community participation
  - Prep all assets and copy

WEEK -1: Warm-up
  - Tease launch on Twitter/X
  - DM supporters to confirm PH launch day
  - Post "building in public" updates
  - Join relevant Discord/Slack communities

DAY 0: Primary Launch (Product Hunt)
  - 12:01 AM PT: go live on PH
  - Morning: tweet, post in communities, email list
  - All day: respond to every PH comment
  - Evening: share results, thank supporters

DAY 1-3: Secondary Launches
  - Day 1: Show HN post
  - Day 2: Reddit posts (staggered across subreddits)
  - Day 3: Indie Hackers product listing + post

WEEK 1-4: Sustained Push
  - Weekly build-in-public updates
  - Continue community engagement
  - Follow up with PH/HN/Reddit commenters
  - Submit to remaining directories
```

### Step 5: Platform-Specific Content
Generate tailored copy for each platform because each has different culture and expectations:
- Product Hunt: benefit-focused, visual, social proof
- Hacker News: technical, honest, understated
- Reddit: conversational, vulnerable, community-oriented
- Indie Hackers: metrics-focused, journey-oriented
- Twitter: punchy, thread-worthy, shareable

### Step 6: Scoring & Prioritization
Score each platform:
```
PLATFORM        AUDIENCE FIT  EFFORT  TRAFFIC POTENTIAL  CONVERSION  PRIORITY
─────────────   ───────────   ──────  ─────────────────  ──────────  ────────
[filled per project]
```

### Step 7: Memory & Learning
After each platform launch, record:
- Traffic generated (unique visitors, signups)
- Engagement quality (comments, DMs, feedback richness)
- Conversion rate (visitor → signup → active user)
- What resonated vs what fell flat
- Community contacts made (for future launches)


## Output Format

Deliver as a structured action plan:
1. `platform_map.md` — all relevant platforms scored and prioritized
2. `launch_calendar.md` — coordinated timeline
3. `copy/` — platform-specific copy and assets list
4. `playbooks/` — detailed strategy per top 3 platforms
5. `tracking.md` — metrics to track per platform
