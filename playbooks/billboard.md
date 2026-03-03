---
title: "Billboard Playbook"
layout: default
parent: Home
nav_order: 22
---


# /billboard — Guerrilla Billboard Advertising

Put your startup on a real physical billboard for as little as $10 and turn it into viral social media content.

The meta-play: the CONTENT about being on a billboard is worth 100x more than the billboard impressions themselves.

## Prerequisites

- `agent-browser` available via npx
- A Blip Billboards account (https://www.blipbillboards.com) — free to create
- A creative image file (.jpg or .png, recommended 1920x1080 or similar)
- The user must be logged into Blip OR provide credentials

## Workflow Overview

```
STEP 1: Gather Context      → what project, what message, what audience
STEP 2: Generate Creative    → design the billboard image + copy
STEP 3: Select Locations     → pick billboard locations on Blip
STEP 4: Launch Campaign      → upload creative, set budget, go live
STEP 5: Capture Evidence     → screenshot the live billboard listing
STEP 6: Generate Content     → create social media posts about it
```

## STEP 1: Gather Context

Extract from conversation or ask the user:

```
PROJECT:          [name of the startup/product]
URL:              [website URL to display on billboard]
TAGLINE:          [one-line value prop, max 7 words for billboard readability]
TARGET CITIES:    [where to place the billboard — pick cities with target audience]
BUDGET:           [default $10-20 for a test, up to $50 for wider coverage]
TONE:             [serious/playful/provocative/meta]
```

### City Selection Heuristics

If the user doesn't specify cities, recommend based on their target audience:

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

## STEP 2: Generate Creative

### Billboard Design Rules

```
CRITICAL CONSTRAINTS:
  - 7 words or fewer for the main message (people see it for 6-8 seconds)
  - High contrast (dark text on light bg OR light text on dark bg)
  - ONE clear call-to-action (a short URL — easy to remember)
  - No small text — nothing under 30% of the billboard height
  - Brand colors if available, otherwise black + one accent color
  - File format: .jpg or .png ONLY
  - File size: max 2 MB
  - Color mode: RGB (NOT CMYK)
  - Resolution: min 72 PPI, match specific board's pixel dimensions
  - NO QR codes (Blip bans them — distracted driving policy)
  - NO pure white backgrounds (use RGB 235,235,235 or darker)
  - NO grey/white/black bars or wasted space on edges
  - NO footnotes, disclaimers, or fine print
  - MUST include clear advertiser identity (logo, brand name, or URL)

COMMON BOARD DIMENSIONS (pixels):
  920 x 260    — standard large (14' x 48')
  1350 x 650   — medium (12' x 24')
  312 x 312    — square (10' x 10')
  264 x 480    — vertical (12' x 21')
  1344 x 756   — HD landscape
  1920 x 1080  — full HD (less common)
  Note: dimensions vary wildly per board. Check specific board specs on Blip.

WHAT WORKS ON BILLBOARDS:
  ✓ Bold statement + short memorable URL
  ✓ Provocative question + URL
  ✓ Humor/absurdity that makes people photograph it
  ✓ Self-referential / meta humor (highest viral potential)
  ✗ QR codes — BANNED on Blip, also don't work at highway speed
  ✗ Long copy — nobody reads paragraphs at 60mph
  ✗ Multiple CTAs — pick one thing
  ✗ Small logos — make it readable from 200ft away
```

### Creative Templates by Tone

**Meta / Self-Aware (RECOMMENDED — highest viral potential):**
```
"This billboard cost us $10."
"[short-url]"

"I asked my AI if I should buy a billboard."
"It said yes."
"[short-url]"

"We spent our entire marketing budget on this billboard."
"It was $10."
"[short-url]"

"You're reading a billboard bought by a solo founder."
"[short-url]"

"You're stuck in traffic. Might as well check out"
"[short-url]"
```

**Provocative / Bold:**
```
"Your [competitor category] is lying to you."
"[product-url]"

"Stop [pain point]. Start [benefit]."
"[product-url]"

"[Surprising statistic about the problem you solve]"
"[product-url]"
```

**Simple / Clean:**
```
"[Product name]"
"[One-line value prop]"
"[product-url]"
```

**Humor:**
```
"We could've bought 500 coffees with this ad budget."
"Instead, you're reading this."
"[product-url]"

"This billboard is smarter than your current [tool/process]."
"[product-url]"
```

### Generating the Image

If the user doesn't have a pre-made creative:

1. Ask if they want you to generate one (describe what an image gen tool should produce)
2. Or create a simple HTML billboard mockup that they can screenshot:

```html
<!-- Simple billboard creative generator -->
<div style="width:1920px;height:1080px;background:#000;color:#fff;
            display:flex;flex-direction:column;justify-content:center;
            align-items:center;font-family:system-ui;padding:80px;">
  <h1 style="font-size:120px;font-weight:900;text-align:center;
             margin:0;line-height:1.1;">[MAIN MESSAGE]</h1>
  <p style="font-size:64px;margin-top:40px;opacity:0.8;">[URL]</p>
</div>
```

You can create this as a local HTML file and screenshot it with agent-browser:
```bash
npx agent-browser open file:///tmp/billboard-creative.html
npx agent-browser set viewport 1920 1080
npx agent-browser screenshot /tmp/billboard-creative.png --full
```

## STEP 3: Select Locations on Blip

### Automating Blip Billboards

**IMPORTANT**: The user must have a Blip account. If they don't, walk them through creating one at https://www.blipbillboards.com first, or ask them to log in manually before you automate.

#### Login Flow (if needed)

```bash
npx agent-browser open https://marketplace.blipbillboards.com/login
npx agent-browser snapshot -i
# User fills in credentials or you use saved state
npx agent-browser wait --url "**/dashboard" --load networkidle
# Save auth state for reuse
npx agent-browser state save ~/.agents/skills/billboard/.blip-auth.json
```

#### Blip Campaign Types

Blip offers 3 campaign types. For guerrilla marketing, always use Location-Based:

```
TYPE               DESCRIPTION                      USE WHEN
──────────────     ──────────────────────────────   ──────────────────────────
Location-Based     YOU pick specific boards on map   Default. Best for targeting.
Max Awareness      Blip picks boards for best CPM    Widest reach, no control.
Demographics       Blip targets audience profiles    If you know demo, not location.
```

#### Search for Billboards

```bash
# Start a new campaign
npx agent-browser open https://marketplace.blipbillboards.com
npx agent-browser snapshot -i

# Click "+ Create Campaign" button
# Select "Location-Based" campaign type
# Use the interactive map to browse — red dots = available boards
# Click a dot to see: daily impressions, CPM, facing direction, screen dimensions
# Click "Add Sign" to include a billboard

npx agent-browser snapshot -i
# Search by city name or zip code in the map search
# Browse available billboards in target area
# Note the pixel dimensions shown (you'll need matching creative)
```

#### Select and Configure

```
SELECTION CRITERIA:
  - Sort by cheapest per blip (for guerrilla testing)
  - Prefer locations near:
    → Co-working spaces / tech hubs
    → Coffee shops in startup neighborhoods
    → Highway exits near business districts
    → College campuses (if targeting young audience)
  - Avoid: middle-of-nowhere highways with no foot traffic
  - Check the billboard photos — pick ones that are clean, well-lit, visible
  - Note the EXACT pixel dimensions for each selected board
```

#### Set Budget and Schedule

```
RECOMMENDED SETTINGS:
  - Daily Budget: $10-20/day for initial test
  - Max-per-Blip (MPB): $0.15-0.30 (your max bid per 7.5-8 sec display)
    Pro tip: bid slightly above round numbers ($0.27 not $0.25) to edge out competitors
  - Duration: 3-7 days
  - Dayparting: use the schedule grid to pick high-value time slots:
      Morning drive (6-10 AM) and Evening drive (4-7 PM) = most eyeballs
      Set higher MPB during these slots, lower or off during late night
  - A "blip" is one 7.5-8 second display of your ad
  - Blip runs auctions every 10 minutes — higher MPB = more wins

BUDGET MATH:
  $10/day at ~$0.15/blip = ~66 blips/day = ~66 x 8 seconds of screen time
  $20/day at ~$0.15/blip = ~133 blips/day
  Over 5 days at $20/day = ~665 blips, thousands of estimated impressions
```

### Upload Creative

```bash
# Navigate to creative upload section
npx agent-browser snapshot -i
# Find the upload button/area
# Upload the creative file
npx agent-browser upload @[ref] /path/to/billboard-creative.png
npx agent-browser wait --load networkidle
```

### Launch

```bash
# Review campaign summary
npx agent-browser snapshot -i
# Confirm budget, dates, locations, creative
# Click launch/submit
# Screenshot the confirmation
npx agent-browser screenshot /tmp/billboard-campaign-confirmation.png
```

### Approval Process (SET EXPECTATIONS WITH USER)

```
TIMELINE:
  1. Blip reviews creative: ~90 minutes
  2. Billboard owner approves: 1-3 business days
  3. If rejected: revise and resubmit (common reasons: white background,
     QR codes, missing brand identity, restricted content)
  4. Once approved: campaign starts on your specified date (or immediately)

BILLING:
  - Credit card required before activation
  - Day 1: authorization HOLD placed (not charged yet)
  - After 24h: only actual spend captured
  - Then: daily billing, progressively less frequent as trust builds
  - You can stop the campaign anytime from the dashboard
  - Prepaid credits available but NON-REFUNDABLE
```

## STEP 4: Capture Evidence

After the campaign is submitted/live:

```bash
# Screenshot the campaign dashboard
npx agent-browser screenshot /tmp/billboard-dashboard.png

# Screenshot the billboard location on the map
npx agent-browser screenshot /tmp/billboard-location.png

# If Blip shows a preview of your ad on the actual billboard:
npx agent-browser screenshot /tmp/billboard-preview.png
```

Also capture:
- The billboard's physical address
- The estimated impressions
- The total cost
- The dates it will run

## STEP 5: Generate Social Media Content

This is the REAL value. The billboard is content fuel.

### Thread / Post Templates

**Twitter/X Thread:**
```
Post 1:
I just put [project] on a real billboard for $[amount].

Here's what it looks like 👇
[attach billboard preview screenshot]

Post 2:
The economics:
- Cost: $[amount]
- Duration: [X] days
- Estimated impressions: [X]
- Cost per impression: $[calculated]

For context, a Facebook ad costs ~$7 per 1000 impressions.
This billboard costs ~$[X] per 1000.

Post 3:
Why I did this:
[1-2 sentences about the project and why billboard advertising
at this price point is an interesting growth hack]

Post 4:
How you can do it too:
1. Go to blipbillboards.com
2. Pick a billboard near your target audience
3. Upload your creative
4. Set budget to $10
5. You're on a billboard

The content ABOUT the billboard > the billboard itself.

Post 5:
If you're building something and want an AI [advisory council /
lead gen agent / whatever the product is]:

[project URL]

(Yes, the billboard was worth it just for this thread.)
```

**LinkedIn Post:**
```
I just put my startup on a physical billboard.

Total cost: $[amount].

Not $10,000. Not $1,000. $[amount].

Here's what I learned about guerrilla marketing in 2026:

1. Programmatic billboards changed the game
   [explain Blip pricing model]

2. The billboard ISN'T the marketing
   This post is. You're reading it right now.
   The billboard was the excuse to tell you about [project].

3. [Specific insight about their product/audience]

If you're a [target audience] who [pain point],
check out [project URL].

And yes — that's a real billboard in [city].
[attach screenshot]
```

**Reddit Post (r/startups, r/indiehackers, r/EntrepreneurRideAlong):**
```
Title: I put my startup on a real billboard for $[amount] — here's what happened

Body:
[Tell the story conversationally]
[Include the numbers]
[Share what you learned]
[Mention the product naturally, not as a hard sell]
[Ask the community a question to drive engagement]
```

### The Meta-Creative Approach

If the billboard creative itself references the social content:

```
BILLBOARD TEXT:
  "I'm going to post about this billboard on Twitter."
  "[twitter handle]"

Then the Twitter thread references the billboard.
The billboard references the Twitter thread.
Infinite recursion of content. People LOVE this.
```

## STEP 6: Track Results

After launch, check back periodically:

```bash
# Load saved auth
npx agent-browser state load ~/.agents/skills/billboard/.blip-auth.json
npx agent-browser open https://marketplace.blipbillboards.com
npx agent-browser snapshot -i
# Navigate to campaign dashboard
# Capture metrics: blips delivered, impressions, spend
npx agent-browser screenshot /tmp/billboard-results-[date].png
```

Report to user:
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
  Twitter thread:  [impressions/likes/retweets if available]
  LinkedIn post:   [views/reactions if available]
  Reddit post:     [upvotes/comments if available]

The real ROI = social content reach + signups from URL
```

## Quick Reference: Blip Billboard Specs

```
FORMAT:        Digital billboard (LED screen)
DISPLAY TIME:  7.5-8 seconds per "blip"
AUCTION CYCLE: Every 10 minutes
FILE TYPES:    .jpg, .png ONLY (no video)
FILE SIZE:     Max 2 MB
COLOR MODE:    RGB only (no CMYK)
RESOLUTION:    Min 72 PPI, varies by board
               Common: 920x260, 1350x650, 1344x756, 312x312
DAILY MIN:     ~$20/day practical minimum in most locations
PRICING:       ~$0.02-0.50 per blip depending on location and time
               Competitive bids: $0.10-0.30 typical range
COVERAGE:      2,000+ boards across the US
APPROVAL:      ~90 min Blip review + 1-3 days owner approval
BANNED:        QR codes, white backgrounds, alcohol, tobacco,
               nudity, profanity, hate speech, fine print
PAYMENT:       Credit card, pay-as-you-go (only charged for delivered blips)
ANALYTICS:     marketplace.blipbillboards.com/reports
               — blips, impressions, spend, per-board breakdown
               — proof of performance with timestamped play logs
```

## Error Handling

```
PROBLEM                         SOLUTION
──────────────────────────────  ───────────────────────────────────
Creative rejected by Blip       Check content policy — remove any
                                restricted content, ensure text is
                                readable, resubmit

No billboards in target city    Expand search radius, try nearby
                                metro area, or pick a different
                                city from the heuristics table

Budget too low for any boards   Some premium locations have higher
                                minimums — filter by cheapest first

Login/auth issues               Ask user to log in manually in a
                                headed browser session, then save state

Billboard specs don't match     Resize creative to match the specific
                                board's resolution requirements
```

## Notes

- Always ask the user to verify the creative before uploading
- The campaign needs Blip approval (1-2 business days) — set expectations
- Screenshot EVERYTHING for social content
- The billboard is the excuse. The social content is the product.
- A $10 billboard that generates a viral thread reaching 100K people is the best ROI in marketing
