---
title: "9. Email Marketing"
layout: default
parent: Home
nav_order: 10
---


# Email Marketing — Traction Channel 9

## Service Layer
- Resend: developer-first email sending (transactional + marketing)
- Loops.so: SaaS email marketing, event-driven sequences
- ZeroBounce/NeverBounce: email verification before sending
- Hunter.io: find email addresses
- Exa.ai: research audience pain points for email content

## On Invocation

### 1. Gather Context
```
PROJECT:           [name]
ONE-LINER:         [what it does]
CURRENT LIST SIZE: [0 / small / medium / large]
EMAIL TOOL:        [none / Resend / Loops / ConvertKit / Mailchimp / other]
GOAL:              [build list / nurture leads / convert trial users / retain]
AUDIENCE:          [who are they]
```

### 2. Lead Magnet Design

The email list starts with a reason to join. Generate 3-5 lead magnet ideas:

```
FORMAT per idea:
  NAME:        [catchy title]
  TYPE:        [PDF guide / email course / template / tool / checklist / quiz]
  HOOK:        [why someone would give their email for this]
  EFFORT:      [time to create]
  CONVERSION:  [expected opt-in rate: low/med/high]
  FUNNEL:      [lead magnet → what next?]

GOOD LEAD MAGNETS:
  - Solve a SPECIFIC problem (not "our newsletter")
  - Deliver value in under 5 minutes
  - Naturally lead to the product

BAD LEAD MAGNETS:
  - "Subscribe to our newsletter" (no value proposition)
  - 50-page ebook (nobody reads these)
  - Generic checklists with no unique insight
```

### 3. Welcome Sequence

Design a 5-7 email welcome sequence for new subscribers:

```
EMAIL 1 (Immediate):
  SUBJECT: [deliver the lead magnet + set expectations]
  GOAL:    Deliver value, establish tone, tell them what to expect
  CONTENT: Here's what you signed up for + who you are + what's coming
  CTA:     Reply and tell me [question] (starts a conversation)

EMAIL 2 (Day 2):
  SUBJECT: [address their #1 pain point]
  GOAL:    Demonstrate expertise, build trust
  CONTENT: Teach something valuable, no selling
  CTA:     Try this one thing today

EMAIL 3 (Day 4):
  SUBJECT: [a story/case study]
  GOAL:    Social proof, show transformation
  CONTENT: How someone like them solved the problem
  CTA:     See how [product] helped (soft mention)

EMAIL 4 (Day 7):
  SUBJECT: [contrarian insight about their industry]
  GOAL:    Position yourself as a thought leader
  CONTENT: Challenge conventional wisdom
  CTA:     Here's the tool I use for this (product intro)

EMAIL 5 (Day 10):
  SUBJECT: [the "why" behind the product]
  GOAL:    Emotional connection, founder story
  CONTENT: Why you built this, what you believe
  CTA:     Try it free / Join the community

EMAIL 6 (Day 14):
  SUBJECT: [specific feature/use case demo]
  GOAL:    Product education
  CONTENT: Show the product solving THEIR specific problem
  CTA:     Start your free trial / Sign up

EMAIL 7 (Day 21):
  SUBJECT: [final value + offer]
  GOAL:    Convert
  CONTENT: Summary of value delivered + special offer/incentive
  CTA:     Join now + limited time element (if authentic)
```

### 4. Newsletter Strategy

If running a recurring newsletter:

```
NEWSLETTER FRAMEWORK:
  FREQUENCY:  [weekly is optimal for most. less = forgotten, more = annoying]
  DAY/TIME:   [Tuesday-Thursday morning. Test and pick one.]
  FORMAT:     Pick one and be consistent:

  a) CURATOR — "3 things I found this week about [topic]"
     Low effort, high value if your curation is good

  b) ESSAY — one deep thought per week
     Higher effort, builds stronger connection

  c) PRODUCT LOG — "here's what we built/learned this week"
     Building in public. Works for early-stage.

  d) HYBRID — one essay + curated links + product update
     Most common. Covers all bases.

CHARACTER-DRIVEN EMAILS (advanced):
  Instead of "From: [Company] Team"
  Send from the AI advisors themselves:

  "From: Your CFO Advisor
   Subject: I looked at your pricing again...

   I've been thinking about the pricing question you
   asked the council last week. Here's a follow-up..."

  This is WILDLY effective for products with personas.
  Each advisor becomes a recurring email character.
```

### 5. Segmentation Strategy

```
BASIC SEGMENTS:
  - Stage: prospect / trial / active / churned
  - Source: how they found you (content / referral / ad / organic)
  - Engagement: active opener / occasional / cold
  - Persona: which persona type they match

BEHAVIORAL TRIGGERS:
  - Signed up but didn't activate → onboarding nudge
  - Used product 3 times → "you're getting the hang of it" celebration
  - Haven't logged in for 7 days → re-engagement sequence
  - Hit a milestone → congratulations + next steps
  - Invited a friend → thank you + referral program
  - Approaching plan limit → upgrade prompt with value framing

Each segment gets DIFFERENT emails. One-size-fits-all = spam.
```

### 6. Subject Line Framework

```
PATTERNS THAT GET OPENS:
  - Personal/conversational: "Quick thought about your [X]"
  - Curiosity gap: "The [thing] most [audience] get wrong"
  - Specificity: "3 [things] that [result] (tested on 200 users)"
  - Story: "How [person] [achieved result]"
  - Question: "Are you still [pain point]?"
  - Contrarian: "Stop [common advice]. Do this instead."

PATTERNS THAT GET IGNORED:
  - "[Company] Newsletter #47"
  - "Exciting news from [Company]!"
  - "Don't miss out!"
  - "You won't believe..."
  - ALL CAPS ANYTHING

A/B TEST EVERYTHING:
  Always send with 2 subject lines. 20% of list gets A,
  20% gets B, winning line goes to remaining 60%.
```

### 7. Re-engagement Sequences

```
FOR COLD SUBSCRIBERS (haven't opened in 30+ days):

EMAIL 1: "Still interested in [topic]?"
  Short, personal, genuine question. Make it easy to reply.

EMAIL 2 (if no open): "I'll stop emailing unless..."
  Give them control. "Click here to stay, or I'll remove
  you in 7 days." People who click back are re-engaged.

EMAIL 3 (if no open): Remove from list.
  Dead emails hurt deliverability. Better a clean list of
  500 than a dirty list of 5,000.
```

### 8. Email Deliverability Checklist

```
BEFORE SENDING:
  □ Verify all emails with ZeroBounce/NeverBounce
  □ SPF, DKIM, DMARC records set up
  □ Custom sending domain (not @gmail.com)
  □ Warm up new sending domain (start with 50/day, scale up)
  □ Clean list monthly (remove hard bounces, unengaged)
  □ Include plain text version
  □ Include physical address (CAN-SPAM)
  □ One-click unsubscribe in header
  □ Test with mail-tester.com before first send
```

### 9. Automation Flows

Beyond welcome sequence, design these automations:

```
FLOW 1: Lead Magnet → Trial
  Download lead magnet → 3 educational emails → trial offer

FLOW 2: Trial → Paid
  Start trial → onboarding tips (days 1,3,5) → value reminder (day 7)
  → conversion offer (day 12) → last chance (day 13)

FLOW 3: Churn Prevention
  Usage drops → "everything ok?" → feature highlight →
  personal offer → exit survey

FLOW 4: Referral Loop
  Happy user (high NPS or engagement) → "know someone who'd
  benefit?" → referral incentive → track and reward
```

### 10. Quick Win — Get Your First 100 Subscribers

```
TACTICS (ranked by speed):
  1. Add email capture to your landing page TODAY (obvious but often missing)
  2. Write one high-value thread on Twitter → CTA: "I write about this weekly,
     subscribe at [link]"
  3. Comment on 10 Reddit posts with genuine value → include lead magnet link
     in a follow-up (not the comment itself)
  4. Post lead magnet on Indie Hackers / Hacker News
  5. Email 20 people you know personally who fit the audience
  6. Cross-promote with a similar-sized newsletter (swap recommendations)
  7. Add "PS: I also write about [topic] at [newsletter link]" to your email signature
```

### 11. Measurement

```
KEY METRICS:
  - List growth rate (new subscribers per week)
  - Open rate (target: 30%+ for small lists, 20%+ at scale)
  - Click rate (target: 3-5%)
  - Reply rate (most underrated metric — replies = engagement)
  - Unsubscribe rate (target: under 0.5% per email)
  - Revenue per subscriber
  - Sequence completion rate (what % finish the welcome sequence)

MEMORY TRACKING:
  Record after each campaign:
  - Subject lines: which got highest opens
  - Content types: which got highest clicks
  - Send times: which day/time performed best
  - Segments: which audience segment converts best
  → Optimize future campaigns based on accumulated data
```

---

> **Deep Dive:** See the [Email Deep Dive]({% link playbooks/email-deep-dive.md %}) for the full playbook including lead magnet design, 7-email welcome sequences, newsletter strategy, segmentation, re-engagement sequences, and automation triggers.
