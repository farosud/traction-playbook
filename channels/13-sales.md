---
title: "13. Sales"
layout: default
parent: Home
nav_order: 14
---


# Sales — Traction Channel 13

Direct selling. Talking to humans, understanding their needs, and converting them into customers. At early stage this is "doing things that don't scale." At growth stage it becomes a repeatable machine.

## Service Layer
- Exa.ai: find people publicly expressing the problem you solve
- Apollo.io: contact data, email addresses, company enrichment
- Hunter.io: email verification and domain search
- Clay: waterfall enrichment when primary sources fail
- ZeroBounce: email verification before sending
- Resend: sending outreach emails at scale
- Firecrawl: scrape prospect websites for personalization context
- Apify/Snscrape: social media signal monitoring

## On Invocation

### 1. Gather Context

```
PROJECT:          [name]
ONE-LINER:        [what it does]
PRICE POINT:      [free / $X/mo / $X one-time / custom pricing]
TARGET BUYER:     [who makes the purchase decision? job title, company type]
SALES CYCLE:      [impulse / days / weeks / months]
CURRENT PIPELINE: [how many leads do you have now?]
OUTREACH DONE:    [any previous outreach? what happened?]
BOTTLENECK:       [finding leads? getting replies? closing?]
```

### 2. Define Your Ideal Customer Profile (ICP)

Build a detailed ICP. Be ruthlessly specific.

```
IDEAL CUSTOMER PROFILE:

DEMOGRAPHICS:
  Company size:    [1 / 2-10 / 11-50 / 51-200 / 200+]
  Industry:        [specific verticals]
  Revenue:         [range]
  Location:        [if relevant]
  Tech stack:      [what tools they already use]

PSYCHOGRAPHICS:
  Pain level:      [mild annoyance / significant problem / hair on fire]
  Awareness:       [unaware / problem-aware / solution-aware / product-aware]
  Urgency:         [nice-to-have / should fix soon / must fix NOW]
  Budget authority: [individual / needs approval / committee decision]

TRIGGER EVENTS (when they become ready to buy):
  - [Event 1: e.g., "just launched and got no traction"]
  - [Event 2: e.g., "hired their first salesperson"]
  - [Event 3: e.g., "lost a deal to a competitor"]
  - [Event 4: e.g., "posted on social media about the problem"]

DISQUALIFIERS (don't waste time on these):
  - [e.g., "companies with an existing solution under contract"]
  - [e.g., "hobbyists who'll never pay"]
  - [e.g., "enterprise companies with 6-month procurement cycles"]
```

### 3. Lead Sourcing

Five methods to find leads, ordered by signal strength:

#### Method A: Signal-Based (HIGHEST QUALITY)
Find people who just expressed the pain you solve.

```
USING EXA.AI:
  Semantic search for pain signals:
  - "[problem statement] frustrated"
  - "looking for [solution category]"
  - "[competitor] alternative" (actively shopping)
  - "[pain signal phrase from persona research]"

SOCIAL MEDIA SIGNALS:
  Reddit: search subreddits for problem keywords (last 30 days)
  Twitter: search for pain phrases + complaints
  LinkedIn: search posts mentioning the problem

  SCORING:
    Posted in last 7 days:     +3 (hot)
    Posted in last 30 days:    +2 (warm)
    Posted 30-90 days ago:     +1 (cooling)
    Older than 90 days:        +0 (cold — skip)
```

#### Method B: Community Mining
```
COMMUNITIES TO MINE:
  - Reddit threads where people ask for solutions
  - Discord servers where people discuss the problem
  - Telegram groups in your niche
  - Facebook groups (yes, still relevant for some verticals)
  - Forum threads (Indie Hackers, HN, niche forums)

PROCESS:
  1. Join/monitor 5-10 relevant communities
  2. Search for pain signal keywords
  3. Extract usernames of people expressing the problem
  4. Cross-reference to find real names + contact info
  5. Score by recency + pain level + reachability
```

#### Method C: Competitor Customer Poaching
```
FIND COMPETITOR USERS:
  - Search "[competitor] review" → find reviewers
  - Search "[competitor] alternative" → find unhappy users
  - Check G2/Capterra reviews → find users who left ratings
  - Search Twitter for "[competitor] sucks" or "[competitor] problem"

  These people are ALREADY paying for your category.
  They just need a reason to switch.
```

#### Method D: Apollo/Hunter Database Search
```
USING APOLLO:
  Filter by:
    Job title: [target titles]
    Company size: [range]
    Industry: [verticals]
    Technologies used: [if relevant]
    Last funding round: [if relevant]

  Sort by: most recently funded, fastest growing, newest companies

USING HUNTER:
  Domain search for target companies
  Find the right person's email
  Verify before sending
```

#### Method E: Referral Chains
```
After every successful sale or positive conversation:
  "Thanks for trying [product]! Quick question — do you know
   1-2 other [persona description] who might find this useful?"

  After positive product feedback:
  "So glad it helped! Would you be comfortable introducing me to
   anyone else dealing with [the problem]?"

Track referral sources → some customers are "super-connectors."
Prioritize keeping THOSE customers incredibly happy.
```

### 4. Lead Scoring

Score every lead before outreach:

```
LEAD SCORING MATRIX:

SIGNAL STRENGTH (0-4):
  4 = actively seeking a solution (posted "looking for X")
  3 = expressed the pain publicly (complained about the problem)
  2 = fits the ICP perfectly (right title, company, industry)
  1 = adjacent fit (close but not exact match)
  0 = cold / no signal

TIMING (0-3):
  3 = trigger event in last 7 days
  2 = trigger event in last 30 days
  1 = general fit but no recent trigger
  0 = no timing signal

REACHABILITY (0-2):
  2 = email found + active on social (responds to DMs)
  1 = email OR social found
  0 = can't find contact info

NETWORK VALUE (0-1):
  1 = has audience/influence (could become a referral source)
  0 = individual user only

TOTAL: ___/10

TIERS:
  8-10 → HOT: reach out TODAY, personalized message
  5-7  → WARM: reach out this week, batch outreach
  3-4  → COOL: add to nurture list, reach out when capacity allows
  0-2  → COLD: skip or add to long-term drip
```

### 5. Outreach Sequences

#### For HOT leads (score 8-10): Hyper-Personalized

```
MESSAGE 1 (Day 0): The Signal Response

DON'T: "Hi, I noticed you posted about [problem]. Check out [product]."
DO:     Actually respond to their specific situation with value FIRST.

Template:
  "[Respond to their specific post/tweet/comment with genuine insight]

   I deal with this a lot — [1-2 sentences of actual helpful advice].

   I built [product] specifically for this. Happy to give you access
   and walk you through how it handles [their specific scenario].

   [Your name]"

CHANNEL: wherever they posted the signal (Reddit reply, Twitter reply,
         LinkedIn comment, then follow up via DM/email)
```

```
MESSAGE 2 (Day 3): The Follow-Up with Proof

"Hey [name], following up on [topic].

Thought you might find this useful: [link to case study, article,
or framework that helps with their specific problem].

If you want to try [product] for this, I set up [free trial /
demo link / special offer]. No pressure either way.

[Your name]"
```

```
MESSAGE 3 (Day 7): The Clean Break

"Last note on this — I know you're busy.

If [problem] is still on your radar, happy to help whenever.
If not, totally get it. Wishing you well with [their project].

[Your name]"
```

Three messages. That's it. If no response after 3, move on.
Desperation kills sales.

#### For WARM leads (score 5-7): Semi-Personalized Batch

```
MESSAGE 1 (Day 0):
Subject: Quick question about [their specific context]

"Hi [name],

I came across [something specific — their company, content, profile].

Question: [ask about a pain point you know they likely have].

Asking because I'm working on [product] which [one-sentence value prop],
and I'm trying to understand how [persona type] think about this.

Either way, would love your perspective.

[Your name]"

This works because you're ASKING, not pitching.
People respond to questions more than pitches.
```

```
MESSAGE 2 (Day 4):
"Following up — genuinely curious about your take on [question from msg 1].

Also, in case it's helpful: [link to useful resource, not your product].

[Your name]"
```

```
MESSAGE 3 (Day 10):
"Closing the loop on this. If timing isn't right, no worries.

If [problem] becomes a priority, here's where to find me: [link]

[Your name]"
```

### 6. Objection Handling

Pre-build responses to common objections:

```
OBJECTION FRAMEWORK:

"It's too expensive"
  → "What's it costing you to NOT solve [problem]? Let's do the math."
  → "Would a [smaller plan / trial / pay-as-you-go] make more sense to start?"
  → Ask: "What would you need to see to justify the investment?"

"I'm using [competitor]"
  → "How's that going? What do you wish it did differently?"
  → Never trash the competitor. Highlight your DIFFERENCE, not their weakness.
  → "A lot of our users came from [competitor] because [specific differentiator]."

"I need to think about it"
  → "Of course. What specific thing would help you decide?"
  → "Would it help if I [demo / case study / free trial / sent more info]?"
  → Set a specific follow-up: "Can I check back on [specific date]?"

"I don't have time right now"
  → "Totally understand. When would be better?"
  → "Would a 5-minute walkthrough this week work?"
  → This usually means "not convinced yet." Address the real objection.

"I need to check with [someone]"
  → "Makes sense. What would they need to know? I can put together a summary."
  → "Would it help if I joined a quick call with both of you?"
  → Ask: "What's their main concern likely to be?"

"Does it do [specific feature]?"
  → If yes: "Absolutely. Here's how: [show it]."
  → If no: "Not yet, but here's how people work around it: [alternative]."
  → If planned: "It's on our roadmap for [timeframe]. Would that work for you?"
```

### 7. The Conversation Framework

For actual sales calls/demos:

```
STRUCTURE (30 minutes):

OPEN (3 min):
  - Rapport: "How's your week going?"
  - Context: "You mentioned [their specific situation]. Tell me more."

DISCOVER (10 min):
  - "What's your current process for [thing your product helps with]?"
  - "What's the biggest pain point with that?"
  - "What have you tried to fix it?"
  - "What would ideal look like for you?"
  - "How much time/money does this problem cost you?"

  LISTEN MORE THAN YOU TALK. Ratio should be 70% them, 30% you.

PRESENT (10 min):
  - "Based on what you told me, here's how [product] handles that..."
  - Show THEIR use case, not a generic demo
  - Connect every feature to something THEY said in discovery
  - "You mentioned [pain]. This is how we solve exactly that."

CLOSE (5 min):
  - "Does this feel like it would solve [their stated problem]?"
  - If yes: "Great, here's how to get started: [specific next step]"
  - If hesitant: "What's holding you back?" (then handle the objection)
  - If no: "No problem. What WOULD help with [their problem]?" (learn from it)

FOLLOW UP (2 min):
  - "I'll send you a summary of what we discussed."
  - "I'll include [specific resource they asked about]."
  - Set next action: "I'll check in [day] to see how it's going."
```

### 8. Pipeline Management

```
PIPELINE STAGES:

STAGE          | DEFINITION                    | TARGET CONVERSION
─────────────  | ────────────────────────────  | ─────────────────
Identified     | Lead found, not contacted     | →
Contacted      | First message sent            | 20-30% reply
Replied        | Got a response                | 50% to call
Call Scheduled | Meeting booked                | 70% show up
Demo Given     | Had the conversation          | 30-50% to trial
Trial/Active   | Using the product             | 40-60% to paid
Paid           | Paying customer               | ✓ Done
Lost           | Said no or went silent        | Track reason

PIPELINE TRACKING (update weekly):
  Stage          | Count | This Week | Conversion Rate
  ─────────────  | ───── | ───────── | ───────────────
  Identified     | [N]   | [+/-]     | —
  Contacted      | [N]   | [+/-]     | [%] from above
  Replied        | [N]   | [+/-]     | [%]
  Call Scheduled | [N]   | [+/-]     | [%]
  Demo Given     | [N]   | [+/-]     | [%]
  Trial/Active   | [N]   | [+/-]     | [%]
  Paid           | [N]   | [+/-]     | [%]
  Lost           | [N]   | [+/-]     | → track reasons
```

### 9. Learning Loop

After every sales conversation, record:

```
CONVERSATION LOG:

DATE:        [date]
LEAD:        [name / company]
SCORE:       [their lead score]
CHANNEL:     [how you found them]
OUTCOME:     [converted / objection / lost / needs follow-up]
OBJECTION:   [what held them back, if anything]
INSIGHT:     [what you learned about the market/product]
QUOTE:       [anything they said worth remembering verbatim]
FOLLOW-UP:   [what you promised to do + when]

PATTERN TRACKING (review monthly):
  Top 3 objections this month:
    1. [objection] — heard [N] times — current response working? [yes/no]
    2. [objection] — heard [N] times
    3. [objection] — heard [N] times

  What converts best:
    Channel: [where do highest-converting leads come from?]
    Signal: [what trigger event predicts conversion best?]
    Message: [which outreach version gets the most replies?]
    Demo angle: [what part of the demo closes?]

  What to change next month:
    - [adjustment based on data]
```

### 10. Scaling: From Manual to Machine

```
STAGE 1: Founder Selling (0-20 customers)
  You do everything manually.
  Goal: learn what works, build the playbook.

STAGE 2: Documented Playbook (20-50 customers)
  Document every step that works.
  The agent starts automating lead finding + scoring.
  You still handle conversations and closing.

STAGE 3: Semi-Automated (50-200 customers)
  Agent finds leads, scores them, sends initial outreach.
  You handle replies, demos, and closing.
  Agent tracks patterns and suggests improvements.

STAGE 4: Mostly Automated (200+ customers)
  Agent runs the entire top-of-funnel.
  You handle only high-value conversations.
  Consider hiring a human salesperson using your playbook.
```

### 11. Channel Fit Assessment

Sales is likely strong for you if:
- Your price point is >$20/mo (worth the effort per customer)
- Your audience is reachable (you can find contact info)
- The buying decision is made by 1-2 people (not a committee)
- You enjoy or can tolerate conversations with strangers
- Your product can be demoed in under 15 minutes
- You're still figuring out product-market fit (sales = learning)

Sales is likely NOT your channel if:
- Price point is <$10/mo (unit economics don't work for 1:1 selling)
- Your audience is mass consumer (can't do 1:1 at scale)
- The sales cycle is 6+ months (early stage can't wait that long)
- You have zero tolerance for rejection

Timeline:
- Week 1: ICP defined, first 50 leads identified and scored
- Week 2: First outreach batch (10-15 HOT leads)
- Week 3-4: First conversations, first objections documented
- Month 2: Patterns emerging, playbook forming, 5-10 paying customers
- Month 3: Repeatable process, ready to semi-automate
