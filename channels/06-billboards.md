---
title: "6. Offline Ads / Billboards"
layout: default
parent: Home
nav_order: 7
---

# Offline Ads / Billboards — Traction Channel 6

## The Guerrilla Play

In 2026, programmatic billboards changed everything. You can put your startup on a real physical billboard for $10-50 using platforms like Blip Billboards. The meta-play: the CONTENT about being on a billboard is worth 100x more than the billboard impressions themselves.

## Service Layer

- **Blip Billboards**: Programmatic billboard buying — select location, upload creative, set budget, go live
- **Agent-Browser**: Automate the billboard purchase workflow
- **Image generation tools**: Generate billboard creative (1920x1080 or board-specific dimensions)

## On Invocation

### 1. Gather Context

```
PROJECT:          [name of the startup/product]
URL:              [website URL to display on billboard]
TAGLINE:          [one-line value prop, max 7 words for billboard readability]
TARGET CITIES:    [where to place the billboard — pick cities with target audience]
BUDGET:           [default $10-20 for a test, up to $50 for wider coverage]
TONE:             [serious/playful/provocative/meta]
```

### City Selection Heuristics

```
AUDIENCE                  RECOMMENDED CITIES / AREAS
────────────────────────  ───────────────────────────────────────
Tech founders/builders    Austin TX, San Francisco CA, Miami FL,
                          Denver CO, Nashville TN
Creators/freelancers      Los Angeles CA, New York NY, Austin TX,
                          Portland OR, Atlanta GA
Enterprise/B2B            New York NY, Chicago IL, Dallas TX,
                          Washington DC, Boston MA
Crypto/Web3               Miami FL, Austin TX, New York NY
Students/young adults     College towns near target universities
Local business             User's own city/metro area
General/viral play        Times Square area (NYC), Vegas Strip,
                          LA billboards on Sunset Blvd
```

### 2. Billboard Creative Design

```
CRITICAL CONSTRAINTS:
  - 7 words or fewer for the main message (people see it for 6-8 seconds)
  - High contrast (dark text on light bg OR light text on dark bg)
  - ONE clear call-to-action (a short URL — easy to remember)
  - No small text — nothing under 30% of the billboard height
  - Brand colors if available, otherwise black + one accent color
  - File: .jpg or .png, max 2 MB, RGB color mode
  - NO QR codes (Blip bans them — distracted driving policy)
  - NO pure white backgrounds (use RGB 235,235,235 or darker)

COMMON BOARD DIMENSIONS (pixels):
  920 x 260    — standard large (14' x 48')
  1350 x 650   — medium (12' x 24')
  312 x 312    — square (10' x 10')
  1344 x 756   — HD landscape
  1920 x 1080  — full HD
```

### Creative Templates by Tone

**Meta / Self-Aware (highest viral potential):**
```
"This billboard cost us $10."
"[short-url]"

"We spent our entire marketing budget on this billboard."
"It was $10."
"[short-url]"

"You're reading a billboard bought by a solo founder."
"[short-url]"
```

**Provocative / Bold:**
```
"Your [competitor category] is lying to you."
"[product-url]"

"Stop [pain point]. Start [benefit]."
"[product-url]"
```

**Humor:**
```
"We could've bought 500 coffees with this ad budget."
"Instead, you're reading this."
"[product-url]"
```

### 3. Campaign Setup (Blip Billboards)

```
CAMPAIGN TYPES:
  Location-Based   → YOU pick specific boards on map (RECOMMENDED)
  Max Awareness    → Blip picks boards for best CPM
  Demographics     → Blip targets audience profiles

RECOMMENDED SETTINGS:
  - Daily Budget: $10-20/day for initial test
  - Max-per-Blip (MPB): $0.15-0.30 (your max bid per 7.5-8 sec display)
  - Duration: 3-7 days
  - Dayparting: Morning drive (6-10 AM) + Evening drive (4-7 PM)

BUDGET MATH:
  $10/day at ~$0.15/blip = ~66 blips/day
  $20/day at ~$0.15/blip = ~133 blips/day
  Over 5 days at $20/day = ~665 blips, thousands of impressions
```

### 4. Approval Process

```
TIMELINE:
  1. Blip reviews creative: ~90 minutes
  2. Billboard owner approves: 1-3 business days
  3. If rejected: revise and resubmit
  4. Once approved: campaign starts on your specified date

COMMON REJECTION REASONS:
  - White background, QR codes, missing brand identity, restricted content
```

### 5. Generate Social Content (The Real ROI)

The billboard is the excuse. The social content is the product.

**Twitter/X Thread template:**
```
Post 1: I just put [project] on a real billboard for $[amount]. Here's what it looks like 👇
Post 2: The economics: Cost $X, Duration Y days, Estimated impressions Z
Post 3: Why I did this: [1-2 sentences about the project]
Post 4: How you can do it too — step by step
Post 5: CTA for your product
```

**LinkedIn Post template:**
```
I just put my startup on a physical billboard. Total cost: $[amount].
Not $10,000. Not $1,000. $[amount].
The billboard ISN'T the marketing. This post is.
```

**The Meta-Creative Approach:**
```
BILLBOARD TEXT: "I'm going to post about this billboard on Twitter."
Then the Twitter thread references the billboard.
The billboard references the Twitter thread.
Infinite recursion of content. People LOVE this.
```

### 6. Measurement

```
BILLBOARD CAMPAIGN REPORT
─────────────────────────
Campaign:     [project name] on [billboard location]
Status:       [active/completed]
Blips:        [X] delivered of [Y] planned
Impressions:  ~[estimated]
Total Spend:  $[amount]
CPM:          $[calculated]
Duration:     [X] of [Y] days elapsed

SOCIAL CONTENT PERFORMANCE:
  Twitter thread:  [impressions/likes/retweets]
  LinkedIn post:   [views/reactions]
  Reddit post:     [upvotes/comments]

The real ROI = social content reach + signups from URL
```

### Fit Score

```
BILLBOARD CHANNEL FIT
  Signal that it fits:
    ✓ You have a short, memorable URL
    ✓ Your product has a visual or emotional hook
    ✓ You're comfortable with creative, scrappy marketing
    ✓ You want social content that stands out from "tips & tricks" threads
    ✓ Your audience overlaps with US billboard locations

  Signal that it doesn't fit:
    ✗ Enterprise B2B with long sales cycles
    ✗ Product requires explanation (billboard = 7 words max)
    ✗ No social presence to amplify the billboard content
    ✗ Target audience is outside the US (Blip is US-only)
```

---

> **Deep Dive:** See the [Billboard Playbook]({% link playbooks/billboard.md %}) for the full step-by-step automation guide including Blip browser automation, creative generation, and social content templates.
