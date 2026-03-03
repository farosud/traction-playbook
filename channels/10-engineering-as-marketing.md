---
title: "10. Engineering as Marketing"
layout: default
parent: Home
nav_order: 11
---


# Engineering as Marketing — Traction Channel 10

## Service Layer
- Exa.ai: research what free tools exist in the space, find gaps
- Serper: check what people search for (tool-related keywords)
- Firecrawl: analyze competitor free tools
- Replicate/FAL.ai: if the tool involves AI/image generation
- Resend: capture emails from tool users

## On Invocation

### 1. Gather Context
```
PROJECT:           [name]
ONE-LINER:         [what it does]
TARGET AUDIENCE:   [who would use a free tool from you]
TECH STACK:        [what can you build with? Next.js, Python, etc.]
BUILD TIME BUDGET: [a weekend / a week / a month]
PRODUCT OVERLAP:   [how does the free tool relate to the paid product?]
```

### 2. Free Tool Ideation

Generate 5-7 free tool ideas. Score each:

```
FORMAT per idea:
  TOOL NAME:      [catchy, descriptive name]
  WHAT IT DOES:   [one sentence]
  WHY PEOPLE USE IT: [the problem it solves standalone]
  VIRAL MECHANIC: [why would someone share this?]
  LEAD CAPTURE:   [how does it capture emails / lead to paid product?]
  BUILD EFFORT:   [weekend / 1 week / 2 weeks / month]
  SHAREABILITY:   [1-10: would people screenshot/share the output?]
  PRODUCT FUNNEL: [how naturally does this lead to the paid product?]

  SCORE = (SHAREABILITY × PRODUCT_FUNNEL) / BUILD_EFFORT

IDEAL FREE TOOL CHARACTERISTICS:
  ✓ Solves a real problem (useful even if they never buy your product)
  ✓ Output is shareable (generates something people want to show others)
  ✓ Requires email for full results (natural lead capture)
  ✓ Demonstrates your product's core value (taste of the paid experience)
  ✓ Can be built in a weekend (don't over-invest before validation)
  ✓ Has a natural "want more?" moment (upsell feels like a service, not a pitch)
```

### 3. Tool Architecture

For the top-scoring tool, spec out the MVP:

```
FEATURES (MVP — absolute minimum):
  - [feature 1: the core value]
  - [feature 2: the thing that makes it shareable]
  - [feature 3: the lead capture moment]

NOT IN MVP (resist the urge):
  - [anything that doesn't serve the 3 goals above]

TECH APPROACH:
  - Frontend: [recommendation based on founder's stack]
  - Backend: [if needed — many tools are frontend-only]
  - AI: [if needed — specify which model and why]
  - Hosting: [Vercel/Netlify for free, or project-specific]

TIMELINE:
  Day 1: [build core functionality]
  Day 2: [add shareability + lead capture]
  Day 3: [polish, test, deploy]
```

### 4. The Conversion Funnel

```
FUNNEL DESIGN:
  STEP 1: User discovers free tool (via social share, search, or referral)
  STEP 2: User gets value (the tool works, they see results)
  STEP 3: "Want deeper/more/ongoing?" moment
          - NOT a hard gate. They already got value.
          - This is an invitation, not a restriction.
  STEP 4: Email capture or product signup
  STEP 5: Welcome sequence nurtures to paid conversion

GATING STRATEGIES (from least to most aggressive):
  a) NO GATE: tool is fully free, just "powered by [product]" branding
     → lowest conversion, highest usage/sharing

  b) SOFT GATE: full results require email
     → "Enter email to see your complete analysis"
     → good balance of usage and capture

  c) LIMIT GATE: free for X uses, then signup
     → "3 free analyses, then create an account"
     → works well for addictive tools

  d) FEATURE GATE: basic version free, premium features need account
     → freemium model for the tool itself
     → works when there's a clear basic vs advanced split
```

### 5. Shareability Design

The tool should produce OUTPUT that people want to share:

```
SHAREABLE OUTPUT PATTERNS:
  - Scores/grades: "Your startup idea scored 7.2/10" → screenshot + share
  - Comparisons: "You vs industry average" → ego-driven sharing
  - Visualizations: charts, maps, diagrams → visual social media content
  - Personalized insights: "Based on YOUR data, here's..." → feels special
  - Surprising/counterintuitive results: "Wait, really?" → conversation starter
  - Badges/certificates: "Verified: your idea is [X]" → social proof

MAKE SHARING EASY:
  - "Share your results" button with pre-written tweet/post
  - Open Graph meta tags so the link preview looks good
  - Unique URL per result (vibelife.sh/tool/results/abc123)
  - Include product branding in shared output (subtle watermark)
```

### 6. Launch Strategy for the Free Tool

```
PHASE 1: SOFT LAUNCH (Day 1-3)
  - Share with 10-20 people in your network
  - Get feedback, fix bugs
  - Collect 3-5 testimonials / screenshots of results

PHASE 2: COMMUNITY LAUNCH (Day 4-7)
  - Post on relevant subreddits (lead with the FREE TOOL, not your product)
  - Share on Twitter with results screenshot
  - Post on Indie Hackers, Hacker News (Show HN)
  - Submit to relevant Discord/Telegram communities

PHASE 3: AMPLIFICATION (Day 8-14)
  - Reach out to newsletter writers covering the space
  - Ask early users to share their results
  - Write a "how I built this free tool in a weekend" thread
  - The "building the tool" story IS content (meta-marketing)

PHASE 4: SEO (Ongoing)
  - Optimize tool page for "[problem] free tool" keywords
  - Create content around the tool's use cases
  - Build backlinks by getting listed on tool directories
```

### 7. Classic Examples to Learn From

```
TOOL → WHAT IT DOES → HOW IT LEADS TO PAID

HubSpot Website Grader → Scores your website → "Fix these issues with HubSpot"
Moz Domain Authority → Checks your DA → "Improve your DA with Moz Pro"
Mailchimp Templates → Free email templates → "Send them with Mailchimp"
Stripe Atlas → Free incorporation guide → "Incorporate with Stripe Atlas"
CoSchedule Headline Analyzer → Scores your headline → "Plan content with CoSchedule"
WordCounter → Word/character count → "Write better with [tool]"
Hemingway Editor → Readability check → "Write better" (standalone success story)
Carbon.now.sh → Code screenshots → "Powered by Carbon" (brand awareness)

PATTERN: Free tool solves ADJACENT problem → paid product solves CORE problem.
The free tool is the top of the funnel. The paid product is the solution.
```

### 8. Measurement

```
METRICS TO TRACK:
  - Tool usage (unique users per day/week)
  - Completion rate (% who finish the tool flow)
  - Share rate (% who share their results)
  - Email capture rate (% who give email)
  - Tool-to-signup rate (% who become product users)
  - Tool-to-paid rate (% who eventually pay)
  - Referral traffic (are shared links bringing new users?)
  - Search traffic (is the tool page ranking?)

MEMORY TRACKING:
  Record:
  - Which tool concept got most traction
  - Where the traffic came from
  - What conversion funnel step has the biggest drop-off
  → Iterate: improve drop-off points, double down on working channels
```

### 9. Quick Win — Build Something This Weekend

```
If your product involves AI/analysis:
  → Build a "[topic] analyzer" or "[topic] scorer"
  → Input: user describes their [business/idea/problem]
  → Output: scored analysis with 3-5 dimensions
  → Share: results page with pre-written share text

If your product involves data:
  → Build a "[topic] calculator" or "[topic] benchmark"
  → Input: user enters their numbers
  → Output: comparison to industry averages
  → Share: "I'm in the top X%" type result

If your product involves community:
  → Build a "[topic] quiz" or "[topic] assessment"
  → Input: user answers 5-10 questions
  → Output: personality/type result (like a BuzzFeed quiz but useful)
  → Share: "I'm a [type]! What are you?"

CONSTRAINT: It must be buildable in 8 hours or less.
If it takes longer, you're over-engineering it.
```
