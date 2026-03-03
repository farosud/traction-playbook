---
title: "Email Deep Dive"
layout: default
parent: Home
nav_order: 24
---


# /email-traction — Email Marketing

Direct line to people who opted in. Highest ROI of any digital channel (36:1 average). You OWN the list — not renting attention from platforms.

## Service Layer

```
SERVICE         USED FOR                                    FALLBACK
──────────────  ──────────────────────────────────────────  ──────────────────
Resend          Email sending (transactional + marketing)    Loops.so, Mailchimp
ZeroBounce      Email verification before sending            NeverBounce
Exa.ai          Research competitor email strategies,        Manual research
                find newsletter examples in your space
Hunter.io       Find email addresses for outreach            Apollo.io free tier
```

## On Invocation

### 1. Gather Context

```
EMAIL MARKETING INTAKE
=======================
1. Product:           [what do you sell?]
2. Current list size: [0 / < 100 / 100-1K / 1K-10K / 10K+]
3. Email tool:        [none yet / Resend / Loops / ConvertKit / Mailchimp / other]
4. Existing content:  [blog? newsletter? any email sequences running?]
5. Primary goal:      [build list / improve open rates / increase conversions / reduce churn]
6. Target audience:   [who should be on your list?]
7. Content frequency: [how often can you email? daily/weekly/biweekly/monthly]
8. Brand voice:       [professional / casual / technical / playful]
9. Website traffic:   [rough monthly visitors — determines list growth potential]
```

### 2. Lead Magnet Design

The lead magnet is WHY people give you their email. It must be:
- Immediately valuable (not "subscribe for updates")
- Specific to a pain point your audience has
- Quick to consume (not a 200-page ebook)
- Related to what you sell (attracts the RIGHT people)

#### Lead Magnet Ideas (generate 3-5 tailored to the project)

```
TYPE                EFFORT    CONVERSION   EXAMPLE
──────────────────  ────────  ──────────   ─────────────────────────────────
Checklist/Cheatsheet  Low     High         "The Solo Founder Decision Checklist"
Email course (5-day)  Medium  Very High    "5 Days to Better Pricing Decisions"
Template/Swipe file   Low     High         "10 Outreach Email Templates That Got Replies"
Free tool/calculator  High    Very High    "Startup Runway Calculator" (tie to /eng-marketing)
Quiz/assessment       Medium  Very High    "What Type of Founder Are You?" quiz
Exclusive data/report Medium  Medium       "State of Solo Founding 2026"
Video walkthrough     Medium  Medium       "15-min demo: How I use AI for strategy"
Community access      Low     Medium       "Join 500 founders making better decisions"
```

For each lead magnet suggestion:
```
LEAD MAGNET: [name]
TYPE: [checklist/course/template/tool/quiz/report]
TARGET PERSONA: [which persona does this attract?]
PROMISE: [what specific outcome do they get?]
FORMAT: [PDF / email series / web app / video]
CREATION TIME: [hours to build]
LANDING PAGE HOOK: [one-sentence pitch for the opt-in page]
FOLLOW-UP: [what happens after they get the magnet? → welcome sequence]
```

### 3. Opt-In Placement Strategy

Where to capture emails on your site:

```
PLACEMENT               CONVERSION RATE   NOTES
──────────────────────   ──────────────    ─────────────────────────────
Homepage hero section    2-5%              Above the fold, clear value prop
Exit-intent popup        3-7%              Trigger when cursor moves to close
Blog post bottom         1-3%              After they got value from content
Blog post inline         2-5%              Mid-article, contextual to the topic
Dedicated landing page   20-40%            For ads/social traffic pointing here
Sticky top bar           0.5-2%            Low friction, always visible
Resource/tools page      5-15%             Gated access to the tool
Welcome mat (full page)  5-10%             Aggressive but effective for launches
```

### 4. Welcome Sequence (5-7 emails)

The most important emails you'll ever write. They set the tone for the entire relationship.

```
WELCOME SEQUENCE FRAMEWORK
============================

EMAIL 1 — THE DELIVERY (Immediately after signup)
  Subject: [Deliver the lead magnet — "Here's your [thing]"]
  Content:
    - Deliver what you promised (link/attachment)
    - One sentence about who you are
    - Set expectations: "Over the next week, I'll send you [X]"
    - Quick win: one actionable tip they can use RIGHT NOW
  CTA: Use the lead magnet

EMAIL 2 — THE STORY (Day 1-2)
  Subject: [Something personal + intriguing]
  Content:
    - Your origin story / why you built this
    - The problem that drove you (they should see themselves in it)
    - Brief mention of how your product addresses it
    - NO hard sell
  CTA: Reply to this email with [question]

EMAIL 3 — THE VALUE (Day 3-4)
  Subject: [Biggest pain point + promise of solution]
  Content:
    - Teach something genuinely useful
    - Framework, strategy, or insight they can apply immediately
    - Show (don't tell) your expertise
    - Subtle product mention: "This is exactly what [product] helps with"
  CTA: Read more on blog / try the free tool

EMAIL 4 — THE PROOF (Day 5-6)
  Subject: [Social proof / case study / results]
  Content:
    - Customer story or your own results
    - Specific numbers and outcomes
    - "Before [product]" vs "After [product]"
    - If early stage: your own journey using the product
  CTA: See how [product] works → link to demo/tour

EMAIL 5 — THE OBJECTION KILLER (Day 7-8)
  Subject: [Address the #1 objection they have]
  Content:
    - Acknowledge their hesitation directly
    - Address the top 3 objections:
      "I already use [competitor]" → differentiation
      "I can't afford another tool" → ROI calculation
      "AI can't do this well" → proof/demo
    - Flip the objection into a reason TO try
  CTA: Start your free trial / Sign up

EMAIL 6 — THE SOFT CLOSE (Day 9-10)
  Subject: [Time-limited or exclusive offer]
  Content:
    - Summarize the value they've gotten from this sequence
    - Make a clear, direct ask
    - Optional: limited-time offer or bonus for acting now
    - Make it feel personal, not salesy
  CTA: [Primary conversion action]

EMAIL 7 — THE SEGMENTER (Day 12-14)
  Subject: "Quick question — which describes you best?"
  Content:
    - Ask them to self-select into a segment:
      "I'm building a startup solo"
      "I'm thinking about leaving my job"
      "I'm a creator looking to scale"
    - Use clicks to segment for future emails
    - Gives you data on who your list actually is
  CTA: Click to self-segment
```

### 5. Newsletter Strategy

```
NEWSLETTER FRAMEWORK
====================
NAME: [catchy newsletter name]
FREQUENCY: [weekly recommended for most startups]
SEND DAY: [Tuesday-Thursday, 7-10 AM reader's timezone]

NEWSLETTER STRUCTURE:
  1. HOOK (2-3 lines)
     Personal observation, trending topic, or provocative question

  2. MAIN CONTENT (300-500 words)
     One valuable insight, framework, or story
     Teach something or share a perspective

  3. PRODUCT TIE-IN (2-3 lines, optional, max 1x/month)
     Only when naturally relevant to the content

  4. CURATED LINKS (3-5 links)
     Best things you read/found this week
     Brief annotation for each (why it's worth their time)

  5. CTA (1 line)
     "Reply with your biggest [topic] challenge"
     "Forward this to a founder friend who needs to hear this"
     "Share on Twitter → [pre-written tweet link]"
```

### 6. Segmentation Strategy

```
SEGMENT BY:
  1. BEHAVIOR
     - Opened last 5 emails (engaged)
     - Hasn't opened in 30 days (at risk)
     - Clicked product link (high intent)
     - Downloaded lead magnet but didn't sign up (nurture)

  2. SELF-SELECTED (from segmenter email or quiz)
     - Persona 1 type
     - Persona 2 type
     - Persona 3 type

  3. SOURCE
     - Organic search subscribers
     - Social media subscribers
     - Referral subscribers
     - Event/webinar subscribers

  4. STAGE
     - Free trial users
     - Active paid users
     - Churned users
     - Never converted
```

### 7. Re-Engagement Sequences

```
RE-ENGAGEMENT: 30-DAY INACTIVE
================================
EMAIL 1 (Day 30 of inactivity):
  Subject: "Still there?"
  Content: Light, friendly check-in. Highlight what they've missed.

EMAIL 2 (Day 37):
  Subject: "Your best [topic] resource this month"
  Content: Send your single best piece of content from the month.

EMAIL 3 (Day 44):
  Subject: "Should I remove you from the list?"
  Content: Direct question. "No hard feelings — just want to respect
           your inbox. Click here to stay, or I'll remove you in 7 days."

If no click → remove from active list (keep in archive).
A clean list > a big list. Deliverability matters more than size.
```

### 8. Automation Triggers

```
BEHAVIOR-TRIGGERED EMAILS:
  Trigger: User visits pricing page 2+ times
  → Send: "Questions about pricing? Here's what's included..."

  Trigger: User starts free trial but doesn't complete setup
  → Send: "Need help getting started? Here's a 3-minute walkthrough..."

  Trigger: User's trial is expiring in 3 days
  → Send: "Your trial ends soon — here's what you'd lose..."

  Trigger: User cancels / churns
  → Send: "Sorry to see you go. What could we have done better?"
  → Wait 30 days → Send: "We've improved [thing they complained about]..."

  Trigger: User achieves a milestone (10th session, first month, etc.)
  → Send: "Congrats! You've [milestone]. Here's what to do next..."
```

### 9. Subject Line Formulas

```
HIGH-OPEN-RATE SUBJECT LINES:
  "[First name], quick question"              — personal, curiosity
  "I was wrong about [topic]"                 — contrarian, curiosity
  "The [topic] mistake costing you [result]"  — pain + specificity
  "[Number] [topic] lessons from [source]"    — listicle, authority
  "Stop [common practice]. Do this instead."  — contrarian, promise
  "Re: [topic]"                               — feels like a reply
  "This changed how I think about [topic]"    — personal, curiosity
  "[Topic] — the honest truth"                — transparency, trust

RULES:
  ✓ Under 50 characters (mobile preview)
  ✓ No ALL CAPS (spam filter + annoying)
  ✓ No clickbait you can't deliver on
  ✓ A/B test subject lines on every send
  ✗ Never use "Newsletter #47" as a subject
  ✗ Avoid spam trigger words (free, urgent, act now, limited)
```

### 10. Measurement

```
EMAIL DASHBOARD
===============
Metric              | Target    | This Month | Last Month
--------------------|-----------|------------|----------
List size           |           |            |
Growth rate         | +10%/mo   |            |
Open rate           | > 35%     |            |
Click-through rate  | > 3%      |            |
Reply rate          | > 1%      |            |
Unsubscribe rate    | < 0.5%    |            |
Spam complaints     | < 0.01%   |            |
Conversion rate     |           |            |
Revenue from email  |           |            |

PER-SEQUENCE PERFORMANCE:
  Welcome sequence:   [X]% completion rate, [X]% convert to paid
  Newsletter:         [X] avg open rate, [X] avg CTR
  Re-engagement:      [X]% re-engaged, [X]% cleaned
```

## Output Format

```
EMAIL MARKETING STRATEGY FOR [PROJECT]
=======================================

LEAD MAGNET
  [3-5 options with recommendation + creation plan]

OPT-IN PLACEMENT
  [Where to capture emails + priority order]

WELCOME SEQUENCE
  [Full 5-7 email sequence with subjects + content frameworks]

NEWSLETTER PLAN
  [Format + frequency + content structure]

SEGMENTATION
  [Segments to create + how to use them]

AUTOMATION TRIGGERS
  [Behavior-based email triggers]

FIRST MOVE (this week):
  1. Choose lead magnet and create it
  2. Set up email tool (Resend/Loops/ConvertKit)
  3. Write emails 1-3 of welcome sequence
  4. Add opt-in to homepage
  5. Launch
```
