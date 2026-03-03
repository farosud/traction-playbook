---
title: "16. Trade Shows"
layout: default
parent: Home
nav_order: 17
---


# Trade Shows — Traction Channel 16

## Service Layer
Services this channel can leverage (check user's configured API keys):
- **Exa.ai**: discover upcoming events by industry, find speaker lists, research past event content and attendee profiles
- **Firecrawl**: scrape event websites for agenda, speakers, sponsors, attendee info
- **Apollo.io**: find and enrich contacts of speakers, organizers, and likely attendees
- **Hunter.io**: find email addresses for pre-event outreach to speakers and organizers
- **Serper**: research event reviews, find "best [industry] conferences" lists, discover niche meetups

If a service is available, USE IT to ground recommendations in real data rather than generic advice.


## On Invocation

When `/traction tradeshows` is called:

### Step 1: Gather Context
Ask for (if not already provided):
- Product/startup description
- Target audience (who are your ideal users?)
- Location/region (willing to travel? budget for travel?)
- Timeline (next 3 months? 6 months? 12 months?)
- Budget range (free meetups only? $500? $2000?)
- Goal: leads, partnerships, press, hiring, or learning?

### Step 2: Event Discovery
Search for events across multiple categories:

```
EVENT TYPES TO SEARCH:
  MAJOR CONFERENCES:
    Industry-specific (SaaStr, MicroConf, Web Summit, etc.)
    Tech general (CES, SXSW, TechCrunch Disrupt)
    AI/ML specific (NeurIPS, AI Summit, etc.)

  MID-TIER EVENTS:
    Regional tech conferences
    Industry vertical events
    Startup competitions / pitch events
    Demo days (accelerator graduations)

  LOCAL / FREE:
    Meetup.com groups in their city
    Co-working space events
    University entrepreneurship events
    Startup Weekend / hackathons
    Chamber of Commerce events

  VIRTUAL:
    Online summits and webinars
    Twitter Spaces and LinkedIn Live events
    Discord/community AMAs
    Podcast live recordings
```

### Step 3: Event Scoring
Score each discovered event:
```
EVENT           AUDIENCE FIT  COST     NETWORKING   PRESS OPP  TOTAL
                (0-3)         (0-3)    QUALITY(0-2) (0-2)      (0-10)
────────────    ────────────  ───────  ───────────  ─────────  ─────
[filled per project]

SCORING GUIDE:
  Audience Fit: 3=exact target users, 2=adjacent, 1=some overlap, 0=wrong crowd
  Cost: 3=free, 2=under $200, 1=under $1000, 0=over $1000
  Networking: 2=small/intimate (under 200), 1=medium, 0=huge (hard to connect)
  Press Opp: 2=journalists attend, 1=some coverage, 0=no press
```

### Step 4: Pre-Event Strategy
For each top event:

**2 weeks before:**
- Research speaker list → identify 5-10 people to meet
- DM speakers/attendees on Twitter/LinkedIn with genuine questions about their talks
- If possible, write a blog post or thread about one of the event's themes → share, tag organizers
- Prepare: 30-second pitch, business cards or QR code, laptop with demo ready

**1 week before:**
- Post "Who's going to [event]?" on Twitter/LinkedIn
- Schedule 3-5 coffee/dinner meetings with people you want to meet
- Join the event's Slack/Discord if they have one
- Prepare 3 questions to ask during Q&A sessions

**Night before:**
- Review the agenda, star the sessions most relevant to your audience
- Charge devices, download offline demo
- Set up a landing page or special offer for event contacts

### Step 5: At-Event Playbook

```
THE GUERRILLA APPROACH (no booth, no sponsorship):

DON'T:
  - Pitch everyone you meet in the first 30 seconds
  - Hand out business cards like flyers
  - Sit in sessions all day (that's what recordings are for)
  - Eat alone

DO:
  - Attend the hallway track (conversations between sessions)
  - Ask speakers a great question during Q&A → introduces you to the room
  - Host a spontaneous lunch/dinner → "I'm heading to [restaurant],
    anyone want to join?" posted in event Slack/Twitter
  - Offer to demo your product 1:1 to anyone interested (laptop ready)
  - Take notes on conversations → follow up within 24 hours
  - Live-tweet interesting insights (tags the event, builds visibility)
  - Ask "what's your biggest challenge right now?" not "can I pitch you?"

THE BOOTH ALTERNATIVE:
  Instead of paying $2K-10K for a booth, host a dinner/happy hour
  near the venue. $200-500 for drinks, 15-20 people, higher quality
  conversations than any booth interaction.
```

### Step 6: Post-Event Follow-Up

```
WITHIN 24 HOURS:
  - Connect on LinkedIn with everyone you met (personalized note)
  - Send "great meeting you" emails to top 5-10 contacts
  - Post event recap thread on Twitter/LinkedIn
  - Add all contacts to CRM/lead list with event context

WITHIN 1 WEEK:
  - Deeper follow-up with hot leads (schedule calls)
  - Write blog post about key takeaways from the event
  - Share any content created at the event

WITHIN 1 MONTH:
  - Measure: how many leads → conversations → signups from this event?
  - Decide: was this event worth it? Attend again or skip next year?
  - Record learnings in memory for future event decisions
```

### Step 7: Memory & Learning
After each event, record:
- Event name, date, location, cost
- People met (name, role, contact, conversation summary)
- Quality of audience fit (1-10)
- Leads generated → conversion outcomes
- What worked, what didn't
- Whether to attend again


## Output Format

Deliver as:
1. `events.md` — discovered events scored and prioritized
2. `pre_event/[event_name].md` — preparation plan per event
3. `outreach/` — pre-event DMs and emails to speakers/attendees
4. `post_event_template.md` — follow-up sequence template
5. `tracking.md` — ROI tracking per event
