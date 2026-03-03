---
title: "1. Viral Marketing"
layout: default
parent: Home
nav_order: 2
---


# Viral Marketing — Traction Channel 1

## Service Layer
Services this channel can leverage (check user's configured API keys):
- **Exa.ai**: research viral case studies, find similar product viral mechanics, surface "how X grew" breakdowns
- **Firecrawl**: scrape competitor referral programs, landing pages, and invite flows for structural inspiration
- **Apify/SocialVault**: track social sharing metrics, monitor brand mentions, measure earned media velocity
- **Serper**: research viral coefficient benchmarks by industry, find referral program teardowns, locate growth case studies

If a service is available, USE IT to ground recommendations in real data rather than generic advice.


## On Invocation

### 1. Gather Context
From conversation history or by asking directly:

- **Product name + what it does** (one sentence)
- **Current user count bracket**: 0 / 1-100 / 100-1K / 1K-10K / 10K+
- **Is there a natural sharing moment?** When does using the product create exposure to non-users? (e.g., sending a Calendly link, sharing a Canva design, cc'ing someone on a Notion doc)
- **What is the core value?** What makes someone say "you gotta try this" — the sentence they would text a friend
- **Who is the user?** Role, demographic, where they hang out online
- **Current growth channel** (if any): how are users finding the product today?
- **Business model**: free / freemium / paid / marketplace — this shapes what incentives are viable

Do NOT proceed with generic advice. Every recommendation below must reference the specific product, user, and context gathered here.


### 2. Viral Loop Design
Design 3-5 viral loops tailored to THIS product. Choose from the categories below based on what fits — not every category applies to every product.

**FORMAT per loop:**

```
LOOP NAME: [descriptive name]
TYPE: [word-of-mouth / incentivized referral / embedded / social proof / content / network effect]
TRIGGER: [specific user action or moment that causes sharing]
MECHANISM: [exactly how the sharing happens — the plumbing]
INCENTIVE: [what the sharer gets and WHY they care enough to share]
EXPOSURE: [what the recipient sees — the first impression]
CONVERSION: [why the recipient signs up — what is compelling about what they see]
VIRAL COEFFICIENT ESTIMATE: [K value estimate with reasoning]
CYCLE TIME: [hours/days from share event to new user activation]
EFFORT TO BUILD: [low / medium / high]
EXAMPLE: [concrete, specific example for THIS product with real copy/flow]
```

**Loop categories to consider (pick what fits):**

1. **Word-of-mouth loops** — Product is so good people tell others unprompted. Requires a "wow moment" that is hard to keep to yourself. Works best when the product solves a painful problem in a surprisingly elegant way.

2. **Incentivized referral loops** — Share for tangible rewards. Classic Dropbox model (give space, get space). Works when the reward aligns with product value and both sides benefit. Fails when the incentive feels transactional or attracts low-quality users.

3. **Embedded viral loops** — Using the product inherently creates exposure. Calendly links in emails, "Made with X" badges, shared documents, collaborative workflows. The most powerful type because sharing IS usage, not an extra step.

4. **Social proof loops** — Public usage creates FOMO or curiosity. Badges, public profiles, leaderboards, "X uses this" signals. Works in status-conscious communities (developers, designers, founders).

5. **Content loops** — Product generates artifacts people want to share. AI-generated images, custom reports, quiz results, wrapped/year-in-review summaries. The content must be interesting to the VIEWER, not just the creator.

6. **Network effect loops** — Product gets more valuable with more users. Messaging apps, marketplaces, collaborative tools. True network effects are rare — do not claim one exists unless it genuinely does.

**For each designed loop, also note:**
- What could kill this loop (biggest risk)
- What signal tells you this loop is working
- Minimum viable version you could ship in a week


### 3. Referral Program Design
Only recommend a formal referral program if:
- The product has some degree of product-market fit (users are retaining)
- There is a natural recommendation moment
- The unit economics support a referral incentive

If those conditions are met, design the program:

**Structure:**
- **Referrer reward**: What the existing user gets. Prefer product-value rewards (extra features, credits, extended trial) over cash. Cash attracts mercenaries; product rewards attract believers.
- **Referred reward**: What the new user gets. Should reduce friction to trying the product. Free trial extension, bonus credits, premium feature unlock.
- **Double-sided vs single-sided**: Double-sided (both get something) almost always outperforms single-sided. The referred user needs a reason to use the link instead of just signing up normally.

**Mechanics:**
- Unique referral links (short, memorable, optionally custom slugs)
- Referral codes as fallback (for word-of-mouth where links are awkward)
- Attribution window: how long after click does a signup count (7-30 days typical)
- Reward trigger: on signup, on activation, or on payment? (Later = higher quality but lower volume)
- Dashboard for referrers to track their invites and rewards

**Anti-gaming measures:**
- Require referred user to complete a meaningful action (not just create account)
- IP/device fingerprint deduplication
- Rate limits on referral rewards per period
- Manual review threshold (flag accounts with abnormally high referral rates)
- Clawback policy for fraudulent referrals

**Timing:**
- Do NOT launch a referral program on day 1. You need:
  - Enough users to seed it (at least 100-500 active users)
  - Proof that people recommend the product organically (even a few)
  - A product stable enough that referred users have a good first experience
- Soft launch to power users first, then open to all

**Referral program examples to study** (use Exa/Serper to pull current details if available):
- Dropbox: 500MB per referral, both sides. Drove 3900% growth.
- Robinhood: free stock for both. Waitlist created urgency.
- Morning Brew: tiered rewards (swag at 3, premium at 25). Gamified.
- Superhuman: invite-only created exclusivity. Referral = status.


### 4. Sharing Moment Audit
Identify the top 5 moments in the user journey where sharing is most natural. These are moments of peak emotion — delight, surprise, achievement, curiosity.

**Common high-sharing moments:**
1. **After getting a great result** — "Look what this thing just did for me"
2. **After hitting a milestone** — "I just reached X" (streaks, levels, completions)
3. **When comparing with others** — "How do you compare?" (personality quizzes, benchmarks, stats)
4. **When the product says something surprisingly insightful** — "This is so accurate" (AI analysis, recommendations, predictions)
5. **When they want validation from peers** — "What do you think of this?" (designs, writing, plans)
6. **When they save significant time or money** — "This saved me 3 hours"
7. **When onboarding is complete** — "Just set up X, pretty slick"
8. **When they discover a hidden feature** — "Did you know X can do this?"

**For each identified moment, specify:**

| Moment | Sharing Enhancement | Format | Target Platform | Effort |
|--------|-------------------|--------|----------------|--------|
| [specific moment] | [what to add — button, pre-written copy, generated image, link] | [screenshot / link / embed / quote card / video clip] | [Twitter, LinkedIn, iMessage, Slack, WhatsApp, email] | [low/med/high] |

**Sharing UX principles:**
- One tap/click to share. Every extra step loses 50%+ of potential sharers.
- Pre-populate share text but make it editable (nobody shares canned copy verbatim).
- Include a visual when possible — images get 2-3x more engagement than text links.
- Deep link to the relevant content, not the homepage. The recipient should see what excited the sharer.
- Mobile-first. Most sharing happens on phones.
- Do NOT require login to view shared content. Friction kills viral loops.


### 5. Viral Coefficient Calculator
Walk through the math for this specific product:

```
K = i * c

Where:
  i = average number of invites/shares per user
  c = conversion rate of those invites (% who become users)
  K = viral coefficient

If K > 1: exponential growth (each user brings more than one new user)
If K = 0.5-1: strong viral assist (viral supplements other channels)
If K < 0.5: viral is not a primary channel (focus elsewhere)
```

**Help estimate current state:**
- How many users share or invite others? (sharing rate)
- How many people does each sharer reach? (invites per sharer)
- What % of reached people sign up? (invite conversion rate)
- Effective K = sharing_rate * invites_per_sharer * invite_conversion_rate

**Identify the highest-leverage variable:**
- If sharing rate is low: focus on Sharing Moment Audit (Section 4) — make sharing effortless
- If invites per sharer is low: focus on incentives and prompts — give reasons to share more
- If conversion rate is low: focus on the landing/invite experience — what the recipient sees

**Cycle time matters as much as K:**
- K of 0.8 with 1-day cycle > K of 1.2 with 30-day cycle (in practical terms for months 1-6)
- Shorter cycles = faster compounding = faster learning
- Identify what controls cycle time and how to compress it

**Provide a simple projection:**
- With current estimated K and cycle time: users after 1/3/6 months
- With improved K (specify which lever): users after 1/3/6 months
- What K target is realistic in 90 days


### 6. Anti-Patterns
Warn about viral mechanics that BACKFIRE. Be specific about what to avoid and why.

**Forced sharing (gating features behind sharing):**
- Example: "Share to 3 friends to unlock this feature"
- Why it fails: Users resent being coerced. They share to empty accounts or spam groups. The "referred" users arrive annoyed, not curious. Net effect is negative brand sentiment.
- Exception: Waitlist skipping ("share to move up") works IF the product is genuinely supply-constrained.

**Spam loops (auto-posting to social feeds):**
- Example: Auto-tweeting "I just used X!" or mass-emailing contact lists
- Why it fails: Platforms will ban you. Users will revoke permissions. You become the product people warn others about. LinkedIn and Facebook have killed companies over this.
- The Branchout cautionary tale: grew to millions via Facebook spam, then Facebook cut access, company died.

**Incentive abuse (rewards attract gaming):**
- Example: $10 per referral with no activation requirement
- Why it fails: People create fake accounts, use VPNs, build referral farms. You pay for fake users while real metrics look inflated. PayPal spent $60M on referral bonuses — many were gamed.
- Fix: Reward on activation/payment, not signup. Cap rewards per user per period.

**Premature virality (going viral before product is ready):**
- Example: Getting on the front page of HN with a buggy MVP
- Why it fails: You get one shot at a first impression with each person. If they try a broken product, they will not come back. And they will tell others it is bad. Negative word-of-mouth is 2x more powerful than positive.
- Fix: Soft launch to a small, forgiving audience first. Fix retention before amplifying acquisition.

**Dark patterns that erode trust:**
- "Your friend X is using this" emails when they are not
- Uploading contact lists without clear consent
- Making it hard to tell what is an ad vs. organic share
- Fake urgency ("only 2 invites left!" when there is no limit)

**The vanity metrics trap:**
- Shares/invites sent is a vanity metric. Track shares that convert.
- A viral loop with high sharing but zero conversion is just noise.
- Optimize for users acquired through viral, not shares generated.


### 7. First Move
Recommend the single smallest experiment to test viral potential THIS WEEK.

**Criteria for the first move:**
- Can be built/launched in under a week (ideally 1-2 days)
- Tests a real hypothesis about viral behavior
- Produces measurable signal (even with small numbers)
- Does not require building a full referral system

**First move templates (pick the most relevant one):**

1. **The manual share test**: Add a share button at the highest-emotion moment. Track clicks. If >5% of users click it, there is viral intent worth building on.

2. **The "how did you hear about us" survey**: Ask new signups. If >10% say "friend/colleague told me," organic word-of-mouth is already happening and you should amplify it.

3. **The screenshot test**: Make one screen/result in the product look amazing when screenshotted. Add subtle branding. See if it spreads on social.

4. **The invite 3 friends test**: Personally ask 10 of your best users to each invite 3 friends. Track how many accept. This is your baseline K estimate.

5. **The content artifact test**: Generate a shareable output (report, card, image, score) and add a "share this" flow. Measure shares and clicks back.

6. **The NPS-to-referral bridge**: If you have NPS data, reach out to promoters (9-10) and ask them to refer one person. Conversion rate of this request = your referral program ceiling.

**Output format:**
```
FIRST MOVE: [name]
HYPOTHESIS: [what you are testing]
BUILD TIME: [hours/days]
STEPS: [1-2-3 implementation steps]
SUCCESS METRIC: [what number tells you it worked]
THRESHOLD: [what count/rate means "proceed to build more"]
NEXT IF IT WORKS: [what to build next]
NEXT IF IT FAILS: [what to try instead or which channel to explore]
```


### 8. Measurement
What to track, how to track it, and what good looks like.

**Primary metrics:**

| Metric | Definition | Good | Great | How to Track |
|--------|-----------|------|-------|-------------|
| Viral Coefficient (K) | Users * invites * conversion rate | 0.3-0.5 | >0.7 | Product analytics (invite events + signup attribution) |
| Cycle Time | Time from share event to new user activation | <7 days | <2 days | Timestamp diff between invite sent and invitee activation |
| Sharing Rate | % of active users who share at least once per month | 5-10% | >15% | Share button clicks / active users |
| Invite Conversion Rate | % of invite recipients who sign up | 10-20% | >30% | Signups with referral attribution / invites sent |
| Referral Quality | Retention of referred users vs. organic | At parity | Higher | Cohort analysis: referred vs. non-referred retention curves |

**Secondary metrics:**
- Shares per sharer (are a few power-referrers driving everything, or is it distributed?)
- Channel mix (which platform drives the most referred users? Double down there.)
- Time-to-first-share (how quickly after signup does a user share? Earlier = better product-market fit signal)
- Viral attribution rate (% of all new users that came through viral vs. other channels)
- Net promoter score by cohort (are referred users more or less likely to recommend?)

**Instrumentation checklist:**
- [ ] Unique referral/invite links with tracking parameters
- [ ] Event tracking on every share action (button click, link copy, social share)
- [ ] Attribution on signup (which invite link brought this user)
- [ ] Activation tracking for referred users (did they complete onboarding, not just sign up)
- [ ] Cohort tagging (mark users as "referred" vs. "organic" for retention comparison)

**Dashboards to build (in order of priority):**
1. Daily/weekly K factor trend (are viral loops improving?)
2. Funnel: shares sent -> link clicks -> signups -> activations
3. Top referrers leaderboard (who are your champions?)
4. Channel breakdown (Twitter vs. email vs. Slack vs. SMS)

**Review cadence:**
- Weekly: check K factor, sharing rate, conversion rate trends
- Monthly: deep dive on referral quality, cohort retention, channel mix
- Quarterly: decide whether viral is a primary channel or supplementary — reallocate effort accordingly


## Channel Fit Assessment

Before investing heavily in viral marketing, assess fit:

**Viral marketing works best when:**
- The product has a natural sharing moment (usage = exposure)
- The target audience is connected (communities, teams, friend groups)
- The product delivers visible value quickly (short time-to-wow)
- Word-of-mouth is already happening organically (even a little)
- The product is free or freemium (low friction for referred users)

**Viral marketing is a poor fit when:**
- The product solves a private/sensitive problem people do not discuss openly
- The target audience is fragmented (no dense networks)
- Value takes weeks/months to materialize (long time-to-wow)
- The product is high-price-point B2B with long sales cycles
- There is no natural artifact or moment to share

**If viral is not the right primary channel**, say so directly and suggest which of the other 18 traction channels to explore instead. Do not force viral mechanics onto a product where they do not fit.


## Cross-Channel Synergies

Viral marketing amplifies and is amplified by:
- **Content Marketing** (Channel 3): Shareable content feeds viral loops
- **SEO** (Channel 4): Viral landing pages accumulate backlinks
- **Community Building** (Channel 14): Communities accelerate word-of-mouth
- **Engineering as Marketing** (Channel 12): Free tools with built-in virality
- **Existing Platforms** (Channel 9): Platform integrations create embedded loops

Note which other channels are already active and design viral loops that compound with them.
