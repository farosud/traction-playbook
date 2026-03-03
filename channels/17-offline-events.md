---
title: "17. Offline Events"
layout: default
parent: Home
nav_order: 18
---


# Offline Events — Traction Channel 17

## Service Layer
Services this channel can leverage (check user's configured API keys):
- **Exa.ai**: research successful event formats in your industry, find venue options, discover what events competitors/peers host
- **Firecrawl**: scrape event platform pages (Eventbrite, Luma, Meetup) for format inspiration and pricing benchmarks
- **Resend**: send event invitations, reminders, and follow-up emails
- **Replicate/FAL.ai**: generate event promotional graphics and social media assets
- **Apollo.io**: find and invite ideal attendees by role/industry

If a service is available, USE IT to ground recommendations in real data rather than generic advice.


## On Invocation

When `/traction events` is called:

### Step 1: Gather Context
Ask for (if not already provided):
- Product/startup description
- Target audience (who should attend?)
- City/region for the event
- Budget ($0 = host at your apartment, $500 = rented space + food, $2000+ = proper event)
- Goal: user acquisition, community building, product feedback, partnerships, content?
- Timeline: when do you want to host this?
- Existing audience size (email list, social followers, community members)

### Step 2: Event Concept Generation
Generate 3-5 event concepts tailored to the product and audience:

```
EVENT FORMAT OPTIONS:

INTIMATE (5-15 people, $0-200):
  "Founder Dinner"
    → invite 8-12 founders, home or restaurant, one topic of discussion
    → vibelife.sh example: "AI Decision-Making Dinner — bring your hardest
      current business decision, we'll discuss as a group + run it through
      the AI council live"
    → LOW cost, HIGH relationship quality, great for first 20 users

  "Office Hours / Clinic"
    → 1-on-1 sessions back-to-back, 20 min each
    → vibelife.sh: "Free AI Advisory Session — bring a business question,
      get council advice live"
    → GREAT for product demos disguised as value-giving

  "Mastermind Circle"
    → recurring monthly group, 6-8 people, each presents a challenge
    → builds community, creates recurring touchpoint, generates loyalty

MEDIUM (20-50 people, $200-1000):
  "Workshop"
    → teach a skill or framework, use your product as the tool
    → vibelife.sh: "Strategic Decision-Making Workshop — learn frameworks
      Fortune 500 boards use, practice with AI advisors"
    → charge $25-50/seat to cover costs + signal value

  "Demo Night / Showcase"
    → live product demo + Q&A + networking
    → invite complementary products to co-present (shared audience)
    → vibelife.sh: "The AI Advisor Showdown — watch 5 AI advisors debate
      real startup decisions live"

  "Problem-Solving Jam"
    → attendees bring real problems, break into groups, solve together
    → your product is the tool used during the session
    → everyone leaves with actual actionable advice

LARGE (50-200 people, $1000-5000):
  "Mini-Conference"
    → 3-5 speakers + panels + networking
    → partner with other companies to share cost and audience
    → vibelife.sh: "The Solo Founder Summit — a day of strategy,
      decision-making, and building your advisory network"

  "Hackathon"
    → build something in a day using your platform
    → vibelife.sh: "AI Advisor Hackathon — build custom AI advisors
      for different industries, best one wins a prize"
    → generates content, community, and product improvements

RECURRING (any size):
  "Monthly Meetup"
    → consistent cadence builds habit and community
    → different theme each month
    → becomes the "thing" people associate with your brand
```

### Step 3: Logistics Planning
For the chosen event concept:

```
VENUE OPTIONS (by budget):
  $0:       Your home/apartment, co-working space community room,
            public library meeting room, park/outdoor space
  $50-200:  Restaurant private room (often free with food min),
            coffee shop event space, brewery/bar back room
  $200-500: Co-working event space rental, community center,
            small gallery or studio space
  $500+:    Dedicated event venue, hotel conference room,
            startup hub/incubator space

PLATFORM FOR TICKETING/RSVP:
  Luma        — beautiful, free, great for tech events
  Eventbrite  — largest platform, good discovery
  Partiful    — casual, social, good for dinners/parties
  Lu.ma       — (same as Luma, tech crowd loves it)

FOOD/DRINK (the #1 thing people remember):
  $0:         BYOB, potluck
  $5/person:  Pizza + drinks
  $15/person: Catered light bites + beer/wine
  $30/person: Full dinner at restaurant

  Rule: spend 60% of budget on food/drink.
  Bad venue + great food > great venue + no food.

TIMING:
  Weekday evening (6-9 PM) — for professional events
  Saturday afternoon — for workshops/hackathons
  Sunday morning — for brunches/masterminds

  AVOID: Monday, Friday evening, holiday weekends
```

### Step 4: Promotion Plan
How to fill seats:

```
4 WEEKS OUT:
  - Create event page (Luma/Eventbrite)
  - Post on Twitter/LinkedIn with event details
  - Email your list (if you have one)
  - DM 20-30 ideal attendees personally

3 WEEKS OUT:
  - Post in relevant communities (Discord, Slack, Reddit, Telegram)
  - Ask confirmed attendees to invite 1-2 friends
  - Cross-post on Facebook events (still drives local attendance)

2 WEEKS OUT:
  - Second email to list + social post
  - Partner with 1-2 complementary brands to co-promote
  - Post "X seats remaining" urgency content

1 WEEK OUT:
  - Final push DMs to target attendees who haven't RSVP'd
  - Reminder email to confirmed attendees
  - Post speaker/agenda details as content

DAY OF:
  - Morning reminder email with logistics
  - Live-tweet/post from the event
  - Take photos/video for post-event content

TARGETING STRATEGY:
  Don't invite "everyone." Curate the guest list.

  For a 20-person dinner, invite:
  - 5-7 people who are your ideal users
  - 3-4 people who are connectors (know lots of your target users)
  - 2-3 people who bring credibility (known names, but reachable)
  - The rest: interesting people who'll contribute to good conversation

  This mix creates energy, social proof, and organic referrals.
```

### Step 5: Event Execution Guide

```
BEFORE GUESTS ARRIVE:
  - Test all tech (projector, WiFi, demo, etc.)
  - Set up name tags or place cards (people love seeing their name)
  - Have a "host helper" — someone who can greet while you set up
  - Prepare your 2-minute intro/welcome speech
  - Queue up your demo/presentation

DURING THE EVENT:
  - Welcome everyone, set the tone (casual? structured? both?)
  - Introduce people to each other (the host's #1 job)
  - Run the main content (talk, demo, workshop, discussion)
  - Weave the product in naturally — don't make it a sales pitch
  - Take photos (ask permission) — this is content for later
  - Leave 30+ min for unstructured networking at the end

THE PRODUCT DEMO MOMENT:
  Don't pitch. SHOW.

  "Let's run [attendee's real problem] through the AI council
   right now and see what happens."

  Live demos with real problems > polished presentations.
  The audience's reaction to seeing their problem solved IS the pitch.

CLOSING:
  - Thank everyone
  - Tell them what's next (next event, product launch, community)
  - Collect feedback (simple: "what was your favorite part?")
  - Group photo (social content)
```

### Step 6: Post-Event Sequence

```
SAME DAY:
  - Post event photos on Twitter/LinkedIn with takeaways
  - Thank-you message in any group chat created for the event

NEXT DAY:
  - Personal follow-up email/DM to each attendee
  - "Thanks for coming. Here's [one thing of value from the event]."
  - Include product link naturally: "If you want to try what we
    demoed last night: [link]"

WITHIN 1 WEEK:
  - Blog post / thread recapping the event
  - Share attendee quotes/testimonials (with permission)
  - Invite attendees to your community/product if they haven't signed up

WITHIN 1 MONTH:
  - Announce next event date
  - Use this event's photos/content to promote the next one
  - Track: attendees → signups → active users → referrals
```

### Step 7: Content Extraction
Every event generates multiple pieces of content:

```
FROM ONE 2-HOUR EVENT YOU GET:
  - 3-5 photos for social media
  - 1 event recap blog post/thread
  - 1 "behind the scenes" story
  - 3-5 attendee quotes/testimonials
  - 1 "what we learned" post
  - Video clips if recorded (even phone recordings)
  - Content ideas from conversations
  - Product feedback and feature requests

  The event costs you $200. The content would cost $2000 to produce.
```

### Step 8: Memory & Learning
After each event, record:
- Event format, size, cost, venue
- Attendee list (name, contact, engagement level)
- What format worked (discussion? demo? workshop?)
- Conversion: attendees → signups → retained users
- Best moments (what generated the most energy/excitement)
- What to change next time
- Which promotion channels filled seats


## Output Format

Deliver as:
1. `event_concepts.md` — 3-5 event ideas scored by impact × effort
2. `logistics.md` — venue, catering, timeline, budget breakdown
3. `promotion_plan.md` — week-by-week promotion calendar
4. `run_of_show.md` — minute-by-minute event flow
5. `follow_up_sequence.md` — post-event emails and content plan
6. `tracking.md` — metrics and conversion tracking template
