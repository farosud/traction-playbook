---
title: "SEO Deep Dive"
layout: default
parent: Home
nav_order: 23
---


# /seo-traction — Search Engine Optimization

Free traffic from search engines. Takes 3-6 months to see real results, but compounds forever. The ultimate long-term growth channel.

## Service Layer

```
SERVICE         USED FOR                                    FALLBACK
──────────────  ──────────────────────────────────────────  ──────────────────
Serper          SERP analysis, keyword competition,         Manual Google search
                featured snippet research, rank tracking
Exa.ai          Content gap analysis, find what ranks,      Serper results
                identify content opportunities
Firecrawl       Scrape competitor pages for structure,       Jina Reader (free)
                word count, heading analysis
```

## On Invocation

### 1. Gather Context

```
SEO INTAKE
==========
1. Site URL:           [or planned URL — new vs existing site]
2. Domain age:         [brand new / < 1 year / 1-3 years / 3+ years]
3. Domain authority:   [if known — use Moz, Ahrefs, or estimate]
4. Target audience:    [who should find you via search?]
5. Existing content:   [blog? docs? landing pages? how many pages?]
6. Competitor sites:   [2-3 who rank for terms you want]
7. Primary goal:       [signups / demos / purchases / authority]
8. Time to invest:     [hours/week for content creation]
9. Technical control:  [can you edit site code? CMS? static?]
```

### 2. Keyword Research

Generate keywords in 5 buckets:

#### A. Problem Keywords (people searching for the problem)
```
"how to [problem your product solves]"
"[problem] for [audience]"
"why [problem] keeps happening"
"[problem] solutions [year]"
```
Generate 20-30. These people don't know your product exists.

#### B. Solution Keywords (people searching for the solution type)
```
"[product category] tool/software/app"
"best [category] for [use case]"
"[category] comparison [year]"
"[category] free / open source"
```
Generate 15-20.

#### C. Comparison Keywords (people comparing options)
```
"[competitor] alternative"
"[competitor A] vs [competitor B]"
"[product category] comparison [year]"
"switching from [competitor]"
```
Generate 10-15.

#### D. Long-Tail Gold (low competition, high intent)
```
"[specific use case] [specific constraint] [solution]"
"[niche role] [specific problem] tool"
"[industry] [specific workflow] automation"
```
Generate 20-30.

#### E. Question Keywords (informational, builds authority)
```
"what is [concept related to product]"
"how does [category] work"
"[concept] vs [concept] difference"
"why [practice] matters for [audience]"
```
Generate 15-20.

### 3. Keyword Prioritization

Score each keyword on this matrix:

```
KEYWORD               VOL    COMP   INTENT        CONV   CAN RANK?  PRIORITY
────────────────────  ─────  ─────  ────────────  ─────  ─────────  ────────
[keyword]             high   low    transactional  9/10   YES        NOW
[keyword]             med    med    commercial     7/10   maybe      SOON
[keyword]             high   high   informational  4/10   unlikely   LATER
```

#### Priority Rules:
```
RANK NOW (Month 1-2):
  - Low competition + decent volume + high intent
  - Your brand name (must rank #1)
  - Specific feature/product names you coined
  - Very niche long-tail with clear buyer intent

RANK SOON (Month 2-4):
  - Medium competition + good volume
  - Comparison keywords (high intent, moderate competition)
  - Question keywords (build authority)

RANK LATER (Month 4+):
  - High competition head terms
  - Broad category keywords
  - Only attempt after building authority
```

### 4. Content Strategy

For each priority keyword cluster, create a content plan:

```
CONTENT PLAN: [keyword cluster name]
=====================================
TARGET KEYWORD:     [primary keyword]
SECONDARY KEYWORDS: [3-5 related terms to include]
CONTENT TYPE:       [blog post / landing page / comparison / guide / tool page]
SEARCH INTENT:      [what the searcher ACTUALLY wants — be specific]

OUTLINE:
  H1: [title with keyword — under 60 chars]
  H2: [section 1 — address the core question]
  H2: [section 2 — go deeper]
  H2: [section 3 — practical application]
  H2: [section 4 — common mistakes / FAQ]
  H2: [CTA section]

WORD COUNT TARGET:  [based on what currently ranks — match or exceed]
UNIQUE ANGLE:       [what makes YOUR content better than what ranks now?]
INTERNAL LINKS:     [what other pages to link to/from]
EXTERNAL LINKS:     [authoritative sources to reference]
CTA:                [what action should the reader take?]
```

### Content Types to Deploy:

```
TYPE                    WHEN TO USE                    WORD COUNT   SEO VALUE
──────────────────────  ───────────────────────────    ──────────   ─────────
Pillar pages            Broad topics, category terms   3000-5000    Very high
Blog posts              Specific topics, long-tail     1000-2000    High
Comparison pages        vs keywords, alternatives      1500-2500    Very high
Use-case pages          "[product] for [use case]"     800-1500     High
Programmatic pages      Template × data = scale        500-1000     Medium each
Tool/calculator pages   Free tools that rank + convert 300-500+     Very high
Glossary/wiki pages     Define terms in your space     500-1000     Medium
FAQ pages               Question keywords              1000-2000    Medium
```

### 5. Programmatic SEO

If applicable, design a programmatic SEO strategy:

```
PROGRAMMATIC SEO PLAN
=====================
TEMPLATE:        [page template structure]
DATA VARIABLE:   [what changes per page]
URL STRUCTURE:   site.com/[category]/[specific-term]

EXAMPLE PAGES:
  1. site.com/decisions/pricing-strategy
  2. site.com/decisions/when-to-pivot
  3. site.com/decisions/hire-vs-automate
  4. site.com/templates/saas-advisory-board
  5. site.com/tools/startup-idea-validator

TOTAL PAGES:     [estimated count]
UNIQUE VALUE:    [why these aren't thin/duplicate content]

EACH PAGE INCLUDES:
  - Unique intro paragraph (not just find-replace)
  - Structured data specific to the topic
  - Internal links to related pages
  - Clear CTA relevant to the page topic
  - User-generated content potential (comments, ratings)
```

### 6. Technical SEO Checklist

```
TECHNICAL SEO AUDIT
====================
CRITICAL (fix immediately):
[ ] SSL/HTTPS enabled
[ ] Mobile-responsive design
[ ] Page speed < 3s (Core Web Vitals passing)
[ ] XML sitemap exists and submitted to Google Search Console
[ ] robots.txt properly configured
[ ] No duplicate content (canonical tags)
[ ] No broken links (404s)
[ ] Site is indexable (no accidental noindex)

IMPORTANT (fix this week):
[ ] Meta titles on all pages (< 60 chars, keyword included)
[ ] Meta descriptions on all pages (< 160 chars, compelling)
[ ] Proper heading hierarchy (single H1, logical H2-H6)
[ ] Image alt text on all images
[ ] Internal linking structure (every page links to/from others)
[ ] URL structure is clean (/pricing not /page?id=123)
[ ] 301 redirects for any moved/deleted pages

NICE TO HAVE:
[ ] Schema markup (Organization, Product, FAQ, HowTo, Article)
[ ] Open Graph tags (for social sharing)
[ ] Breadcrumbs
[ ] Table of contents on long posts
[ ] Related posts/pages section
[ ] Lazy loading for images below the fold
```

### 7. Link Building Strategy

Realistic approaches for early-stage (no budget for buying links):

```
LINK BUILDING TACTICS (ordered by effort:impact)
=================================================

1. PRODUCT DIRECTORIES (easiest, lowest effort)
   Submit to every relevant directory:
   - Product Hunt
   - AlternativeTo
   - G2, Capterra (if B2B SaaS)
   - Industry-specific directories
   - Startup directories (BetaList, StartupStash, etc.)
   Effort: 2-4 hours one-time | Links: 10-20 DA 30-60 backlinks

2. HARO / CONNECTIVELY (free, recurring)
   Respond to journalist queries matching your expertise
   1-2 quality responses per week
   Effort: 2-3 hours/week | Links: 1-2 DA 50+ links/month

3. GUEST POSTS (medium effort, high value)
   Write for blogs your audience reads (tie to /targeting-blogs)
   Effort: 4-8 hours per post | Links: 1 DA 40-70 link per post

4. LINKABLE ASSETS (high effort, highest long-term value)
   Create something so good people link to it:
   - Original research/data
   - Free tools (tie to /eng-marketing)
   - Comprehensive guides
   - Templates/frameworks
   Effort: 20-40 hours | Links: 10-50 organic links over time

5. BROKEN LINK BUILDING (medium effort)
   Find broken links on relevant sites
   Offer your content as a replacement
   Use Firecrawl to scan competitor backlinks for broken URLs
   Effort: 3-5 hours/week | Links: 2-5 per month

6. RESOURCE PAGE LINKS
   Find "resources" / "tools we use" pages in your niche
   Reach out to be included
   Effort: 2-3 hours/week | Links: 1-3 per month
```

### 8. Quick Wins (rank in 30 days)

```
QUICK WIN KEYWORDS:
  1. Your brand name → must rank #1 (if you don't, fix ASAP)
  2. Very specific long-tail with < 100 monthly searches
  3. Unique terms you coined or own
  4. Local SEO terms (if you have a physical location)
  5. Comparison pages: "[your product] vs [competitor]"

QUICK WIN ACTIONS:
  1. Publish 4 blog posts targeting lowest-competition keywords
  2. Optimize existing pages (title tags, meta descriptions, H1s)
  3. Submit sitemap to Google Search Console
  4. Fix any technical issues flagged in GSC
  5. Get 5-10 easy directory backlinks
```

### 9. 90-Day SEO Plan

```
MONTH 1: Foundation
  - Technical SEO audit + fixes (1 week)
  - Keyword research complete (already done via this skill)
  - 4 cornerstone content pieces published
  - Directory submissions (10-20 links)
  - Google Search Console set up and monitoring

MONTH 2: Content Engine
  - 8 blog posts targeting long-tail keywords
  - Start HARO/Connectively responses (2/week)
  - 1 guest post published
  - Internal linking audit and improvement
  - First ranking assessments — what's moving?

MONTH 3: Scale + Optimize
  - Programmatic pages launched (if applicable)
  - 8 more blog posts (double down on what's ranking)
  - 2 more guest posts
  - Update/improve Month 1 content based on performance
  - Linkable asset created (free tool, research, guide)
  - First traffic + conversion analysis
```

### 10. Measurement

```
MONTHLY SEO DASHBOARD
=====================
Metric                    | This Month | Last Month | Trend
--------------------------|------------|------------|------
Organic traffic (sessions) |           |            |
Organic signups/conversions|           |            |
Keywords ranking top 10    |           |            |
Keywords ranking top 50    |           |            |
Pages indexed             |           |            |
Backlinks acquired        |           |            |
Avg position (GSC)        |           |            |
CTR from SERPs            |           |            |
Bounce rate (organic)     |           |            |
Time on site (organic)    |           |            |

TOP 5 PAGES BY ORGANIC TRAFFIC:
  1. /[page] — [X] visits — keyword: [term] — position: [#]
  2. ...

KEYWORD MOVEMENTS (biggest gains):
  1. [keyword] — position [X] → [Y] (+Z spots)
  2. ...

CONTENT PIPELINE:
  Published this month: [X] pieces
  In progress: [X] pieces
  Planned next month: [X] pieces
```

## Output Format

```
SEO STRATEGY FOR [PROJECT]
===========================

KEYWORD RESEARCH
  [Full keyword tables across 5 buckets with scores]

CONTENT PLAN
  [Prioritized content calendar with outlines]

PROGRAMMATIC SEO (if applicable)
  [Template + data plan + example pages]

TECHNICAL AUDIT
  [Checklist with current status]

LINK BUILDING PLAN
  [Tactics + targets + timeline]

90-DAY ROADMAP
  [Month-by-month action plan]

QUICK WINS (this week):
  1. [specific action]
  2. [specific action]
  3. [specific action]
```
