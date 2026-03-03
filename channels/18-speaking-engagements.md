---
title: "18. Speaking Engagements"
layout: default
parent: Home
nav_order: 19
---


# Speaking Engagements — Traction Channel 18

## Service Layer
Services this channel can leverage (check user's configured API keys):
- **Exa.ai**: discover podcasts and events accepting speakers, find people who spoke about similar topics, research what talks performed well
- **Firecrawl**: scrape podcast pages for submission forms, conference CFP pages, speaker lineup analysis
- **Hunter.io**: find email addresses for podcast hosts and event organizers
- **Apollo.io**: enrich speaker/organizer profiles, find decision-makers at events
- **Serper**: research "[topic] podcast", "[industry] conference call for speakers", speaking opportunity directories

If a service is available, USE IT to ground recommendations in real data rather than generic advice.


## On Invocation

When `/traction speaking` is called:

### Step 1: Gather Context
Ask for (if not already provided):
- Product/startup description
- Founder's area of expertise (what can you speak about credibly?)
- Target audience for the product
- Speaking experience level (never? a few times? experienced?)
- Preferred format: podcasts, stages, panels, webinars, all?
- Geographic constraints (local only? willing to travel? virtual only?)
- Time commitment (1 podcast/week? 1 event/month?)

### Step 2: Talk Topic Generation
Generate 5-7 talk titles that:
- Are interesting to the target audience (not a product pitch)
- Showcase expertise relevant to the product
- Have a contrarian or novel angle (stands out from typical talks)
- Work across formats (podcast interview, keynote, lightning talk, panel)

```
TALK TITLE FORMULA:
  [Contrarian take] + [Specific result] + [For whom]

  BAD:  "How to Use AI for Business"         (generic, boring)
  GOOD: "Why Having One AI Assistant Is Worse Than Having None" (provocative)
  GOOD: "The Decision That Almost Killed My Startup (And What 5 AI Advisors
         Would've Said)"  (story + product + lesson)
  GOOD: "Stop Asking ChatGPT for Business Advice: Why You Need a Council,
         Not a Chatbot" (contrarian + solution)

FORMATS:
  KEYNOTE (15-45 min): Tell a story. One big idea. Inspire action.
  LIGHTNING TALK (5 min): One sharp insight. One memorable takeaway.
  PANEL: Prepare 3 strong opinions you can state in 30 seconds each.
  PODCAST (30-60 min): Be conversational, have 5 great stories ready.
  WEBINAR (30-45 min): Teach something actionable. Include a demo.
  TWITTER SPACE (30-60 min): More casual, Q&A heavy. Be accessible.
```

### Step 3: Opportunity Discovery

**Podcasts (Highest ROI, Lowest Barrier):**
```
HOW TO FIND RELEVANT PODCASTS:
  1. Search "[your topic] podcast" on Apple Podcasts, Spotify
  2. Use ListenNotes.com (free) — search by topic, filter by size
  3. Exa search: "podcast about [topic] accepting guests"
  4. Check what podcasts your competitors/peers have been on
  5. Search Twitter: "[topic] podcast guest" or "looking for podcast guests"

TARGET PODCASTS BY SIZE:
  Micro (100-1K downloads/ep):   Easy to book. DM the host. 80%+ acceptance.
  Small (1K-10K downloads/ep):   Good ROI. Email pitch. 30-50% acceptance.
  Medium (10K-50K downloads/ep): High impact. Need warm intro or great pitch. 10-20%.
  Large (50K+ downloads/ep):     Dream list. Usually need existing authority. 5%.

THE STRATEGY:
  Start with 5-10 micro/small podcasts → build reps → use those episodes
  as proof → pitch medium → use medium as proof → pitch large.

  Most founders go straight for the big ones and get ignored.
  The ladder approach takes 2-3 months but actually works.
```

**Conferences & Events:**
```
HOW TO FIND SPEAKING OPPORTUNITIES:
  1. Search "call for speakers [industry] [year]"
  2. Check callforspeakers.com, sessionize.com, papercall.io
  3. Exa: "conference [topic] call for proposals"
  4. Follow event organizers on Twitter — they post CFPs
  5. Local meetup.com groups — organizers ALWAYS need speakers
  6. Join speaker Slack communities (TechSpeakers, etc.)

CFP TIMELINE:
  Most conferences plan 3-6 months ahead.
  CFP deadlines are usually 2-4 months before the event.
  Start searching NOW for events 3-6 months out.
```

**Other Opportunities:**
```
  - Webinars for partner companies
  - Twitter Spaces / LinkedIn Live (host your own)
  - YouTube collaborations / guest appearances
  - University guest lectures
  - Accelerator/incubator talks
  - Company lunch-and-learns (DM founders: "I'd love to give your
    team a 30-min talk on [topic]. Free, no pitch.")
```

### Step 4: Speaker Asset Creation

**Speaker One-Sheet:**
```
Generate a one-page document with:
  - Professional headshot (or clear photo)
  - Bio (50 words and 150 words versions)
  - 3-5 talk titles with 2-sentence descriptions
  - Past speaking experience (even if it's "Presented at [meetup]")
  - Social proof: follower counts, company name, notable achievements
  - Contact info
  - Links to any recorded talks (even if it's a Loom video)

  This is what you send when someone asks "tell me about yourself as a speaker."
```

**Talk Outlines:**
```
For each talk title, create:
  - 5-bullet summary
  - Key takeaway (one sentence the audience remembers)
  - Why this talk NOW (timeliness hook)
  - Ideal audience (helps organizers slot you correctly)
  - Duration flexibility (can do 5 min, 20 min, or 45 min versions)
```

### Step 5: Outreach Templates

**Podcast Pitch Email:**
```
Subject: [Specific episode reference] + guest idea

Hi [host name],

Loved your episode with [recent guest] about [specific topic] —
especially the part about [specific detail that shows you listened].

I'm [name], [one-line credibility]. I built [product] because
[origin story in one sentence].

I think your audience would find it interesting that [contrarian
take or surprising insight — NOT a product pitch].

Happy to share more if you're interested. Here's a [2-min video /
previous episode / article] that shows my style: [link]

[name]
```

**Conference CFP Submission:**
```
Talk title: [Title]
Abstract: [150-200 words, focus on what the AUDIENCE learns, not what you sell]
Takeaways: [3 bullet points — specific, actionable things they'll walk away with]
Audience level: [beginner / intermediate / advanced]
Bio: [100 words]
Previous talks: [links if available, or "First-time speaker eager to share [X]"]
```

**Cold DM to Event Organizer:**
```
"Hey [name], I've attended [event] the last [N] times and love it.
I've been building [product/concept] and think a talk on [topic]
would resonate with your audience because [specific reason tied to
their event's theme]. Would you be open to a 5-min lightning talk
or a full session? Happy to share an outline."
```

### Step 6: The Content Multiplication Effect

```
EVERY SPEAKING ENGAGEMENT GENERATES:

From a podcast episode:
  - 1 full episode (30-60 min of content)
  - 5-10 tweet-worthy quotes (pull them, tweet them)
  - 1 blog post (transcript → edit → publish)
  - 3-5 short video clips for social media
  - LinkedIn post summarizing key points
  - Newsletter content for 1-2 editions

From a conference talk:
  - 1 recorded talk (if they record)
  - Slides → SlideShare / PDF lead magnet
  - Blog post version of the talk
  - Twitter thread version
  - 5-10 social media clips
  - Photos for social proof
  - Connections with other speakers and attendees

ONE 45-MINUTE PODCAST = 2 WEEKS OF CONTENT
```

### Step 7: Progression Path

```
MONTH 1-2: Foundation
  - Create speaker one-sheet
  - Develop 3 talk topics with outlines
  - Book 4-6 micro/small podcasts
  - Speak at 1-2 local meetups
  - Record yourself giving a talk (even to your webcam) — this is your demo reel

MONTH 3-4: Building
  - Pitch 5-10 medium podcasts using micro podcast episodes as proof
  - Submit to 3-5 conference CFPs
  - Host 1-2 Twitter Spaces or webinars
  - Refine talks based on audience feedback

MONTH 5-6: Scaling
  - Medium podcasts start airing → pitch large ones
  - Conference talks happen → record → use as demo reel
  - Start getting inbound requests ("Can you speak at our event?")
  - Consider creating a speaking page on your website
```

### Step 8: Memory & Learning
After each engagement, record:
- Format (podcast, conference, meetup, webinar)
- Audience size (listeners, attendees)
- Topic that resonated most
- Questions asked (reveals what audience cares about)
- Traffic/signups generated (if trackable)
- Host/organizer contact for future opportunities
- What worked in delivery, what to improve
- Content pieces generated from this appearance


## Output Format

Deliver as:
1. `talk_topics.md` — 5-7 talk titles with outlines
2. `speaker_one_sheet.md` — ready-to-send speaker bio and topics
3. `opportunities.md` — discovered podcasts, events, and CFPs with scores
4. `outreach/` — pitch templates customized per opportunity
5. `content_plan.md` — how to repurpose each appearance
6. `tracking.md` — engagement log with metrics
