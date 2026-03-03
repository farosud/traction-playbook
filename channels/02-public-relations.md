---
title: "2. Public Relations"
layout: default
parent: Home
nav_order: 3
---


# Public Relations — Traction Channel 2

## Service Layer
Services this channel leverages (check user's configured API keys):
- Exa.ai: semantic search for journalists covering the space, find recent articles by topic
- Hunter.io: find journalist email addresses from publication domains
- Apollo.io: enrich journalist profiles, find contact info
- Firecrawl: scrape journalist articles to understand their beat/angle
- Jina Reader: fallback for reading articles (free, no key needed)
- Serper: Google News search for recent coverage in the space

## On Invocation

### 1. Gather Context
- Product/startup name + one-liner
- What makes this NEWSWORTHY? (novel tech, contrarian take, impressive data, founder story)
- Stage (pre-launch, launch, post-traction)
- Any existing press coverage?
- Location of founder (for regional press angle)

### 2. Angle Generation
Generate 5-7 pitch ANGLES, not just one. Each angle targets a different journalist type:

FORMAT per angle:
  ANGLE NAME: [short hook]
  TARGET JOURNALIST TYPE: [beat reporter, tech columnist, industry analyst, newsletter writer]
  HEADLINE THEY'D WRITE: [what THEIR headline would be — not yours]
  WHY NOW: [timeliness hook — what makes this relevant TODAY]
  DATA/PROOF: [what evidence supports the story]
  EXCLUSIVITY VALUE: [what can you offer — early access, data, interview]

Angle categories:
- The Trend Rider: connect to something already trending in news
- The Contrarian: your product challenges conventional wisdom
- The Data Story: you have numbers nobody else does
- The Human Interest: founder's personal story + mission
- The Prediction: bold claim about the future of [industry]
- The How-To: educational angle that happens to feature your product
- The Local Hero: founder in [city] building [innovative thing]

### 3. Journalist Discovery
Using available services, find and score journalists:

#### Step 3a — Identify Target Publications
Using Serper (primary) or Exa.ai (if Serper unavailable):
- Search "[industry/topic] news" + "[industry] startups" + "[industry] technology"
- Capture the top 20-30 publications that appear consistently
- Separate into tiers (see below)
- FALLBACK if no API keys: manually list known publications for the vertical and prompt user to confirm

#### Step 3b — Find Specific Journalists
For each target publication:
1. Exa.ai (primary): semantic search "journalist [publication] [topic] [beat]" to find bylines
2. Firecrawl (secondary): scrape the publication's author pages or recent articles in the relevant section
3. Jina Reader (fallback, free): read article pages to extract author names and bios
4. Manual fallback: check the publication's "About" or "Team" page URL and prompt user to provide names

#### Step 3c — Get Contact Information
For each journalist identified:
1. Hunter.io (primary): search by publication domain to find email patterns and specific addresses
2. Apollo.io (secondary): enrich journalist by name + company to get email and social profiles
3. Twitter/X search via Serper (fallback): search "[journalist name] [publication] site:twitter.com"
4. Manual fallback: most journalists list contact info in their bio or on Twitter — provide the user with direct links to check

#### Step 3d — Understand Their Beat
For each high-priority journalist:
1. Exa.ai (primary): find their 5 most recent articles to identify recurring themes
2. Firecrawl (secondary): scrape their author archive page on the publication
3. Jina Reader (fallback, free): read 2-3 of their recent articles to extract topics and tone
4. Manual fallback: provide article URLs and ask the user to summarize the journalist's angle

For each journalist found:
  NAME:
  PUBLICATION:
  BEAT: [what they specifically cover]
  RECENT ARTICLE: [title + link of most relevant recent piece]
  RELEVANCE SCORE: [1-10 how closely their beat matches your story]
  TWITTER/X: [handle if found]
  EMAIL: [if found via Hunter/Apollo]
  PITCH ANGLE: [which of the 5-7 angles fits THEM best]
  DISCOVERY METHOD: [which service found them — for audit trail]

Tiered targeting:
  TIER 1 (dream): Top-tier tech press (TechCrunch, Verge, Wired, etc.)
  TIER 2 (realistic): Industry-specific outlets, mid-tier tech blogs
  TIER 3 (easiest): Newsletters, Substacks, podcasts, niche blogs
  TIER 4 (local): Regional tech reporters, local business journals

IMPORTANT: Start outreach from TIER 3/4 up. Build coverage snowball.

### 4. Pitch Crafting
For each high-priority journalist, generate a custom pitch email:

RULES:
- Subject line: under 6 words, no clickbait
- First sentence: reference THEIR recent work (proves you read it)
- Second sentence: the hook (why this matters for THEIR readers)
- Third sentence: what makes your thing different
- Fourth sentence: the ask (interview, demo, exclusive, data access)
- Total: 4-6 sentences MAX
- NO attachments
- NO press release format
- NO "I hope this finds you well"
- NO "I'd love to pick your brain"
- NO mass-email feel

#### Pitch Template Structure

SUBJECT: [under 6 words — newsworthy, specific]

[First name],

Your [recent article title] on [topic] [brief genuine reaction — "nailed the tension between X and Y" / "surfaced a trend I've been tracking too"].

[One sentence: the newsworthy thing — what happened, what you built, what data you have]. [One sentence: why their readers specifically would care].

[One sentence: what makes this different from the 50 other pitches they got today — contrarian angle, surprising data point, unique access].

Happy to [specific offer: share the data, give early access, do a 15-min call, provide an exclusive]. [Optional: time constraint — "launching Tuesday" / "embargo available"].

[Name]
[Title, Company]
[One-liner about the company]

#### Pitch Variations by Tier

TIER 3/4 pitch tone: casual, peer-to-peer, "thought you'd find this interesting"
TIER 2 pitch tone: professional, data-forward, clear news hook
TIER 1 pitch tone: concise, exclusive-offering, strong proof points

#### Follow-Up Template (Day 4)

SUBJECT: Re: [original subject] — [new data point or angle]

[First name],

Quick follow-up with a new angle — [genuinely new information, not just "checking in"].

[One sentence on why this is time-sensitive or newly relevant].

No worries either way.

[Name]

### 5. Press Kit Generator
Auto-generate press materials:

#### 5a — Core Messaging
- One-liner (10 words max — the "what is it" sentence)
- Boilerplate — 50 words (for article footers)
- Boilerplate — 150 words (for press releases)
- Boilerplate — 500 words (for feature stories and background)

#### 5b — Founder Materials
- Founder bio — professional angle (achievements, credentials, domain expertise)
- Founder bio — personal angle (origin story, mission, what drives them)
- Founder headshot specifications (list what's needed: high-res, white bg, casual, professional)

#### 5c — Key Stats and Milestones
- Revenue/growth numbers (if shareable)
- User/customer count or growth rate
- Funding raised (if applicable)
- Key partnerships or integrations
- Notable milestones with dates (timeline format)

#### 5d — Quotable One-Liners
Generate 5 quotable one-liners journalists can copy-paste as founder quotes:
1. The vision quote ("We believe [industry] will...")
2. The problem quote ("The current way of doing X is broken because...")
3. The traction quote ("[Specific number] proves that...")
4. The contrarian quote ("Everyone thinks [X], but actually...")
5. The mission quote ("We started this because...")

#### 5e — Suggested Headlines
Make the journalist's job easy — provide 5 headlines they could adapt:
1. News announcement style: "[Company] launches [product] to [solve X]"
2. Trend piece style: "The rise of [category]: how [company] is leading..."
3. Data story style: "[Surprising stat] reveals [insight], says [company]"
4. Profile style: "Meet the founder turning [personal experience] into [product]"
5. Contrarian style: "Why [company] is betting against [conventional wisdom]"

#### 5f — Media Assets Checklist
List what the startup should prepare (not generated, but specified):
- High-res logo (PNG, SVG, light bg, dark bg variants)
- Product screenshots (3-5 key screens/features)
- Founder headshot (professional quality, 300+ DPI)
- Product demo video or GIF (30-60 seconds)
- Architecture diagram or how-it-works visual (if technical product)

#### 5g — Reporter FAQ
5-8 questions a journalist would ask, with pre-written answers:
1. "What does [company] do in one sentence?"
2. "How is this different from [obvious competitor]?"
3. "Who is your target customer?"
4. "What traction do you have so far?"
5. "What's the business model?"
6. "Why now? Why didn't this exist before?"
7. "What's the biggest risk to this working?"
8. "What's the 5-year vision?"

### 6. Timing Strategy

#### Best Days and Times
- Best days to pitch: Tuesday-Thursday
- Best time: 6-9 AM in the journalist's local timezone
- Worst times: Monday morning (inbox flood), Friday afternoon (checked out)
- Exception: breaking/timely news — pitch immediately regardless of day

#### Newsjacking Calendar
Build a rolling 30-day calendar of events and trends to ride:
- Industry conferences and events
- Competitor announcements (react quickly)
- Regulatory changes
- Seasonal trends relevant to the product
- Earnings seasons (if B2B/enterprise)
- Cultural moments (if consumer-facing)

Using Serper or Exa.ai: search for upcoming events in the industry to populate this calendar.
FALLBACK: prompt the user for known upcoming events and deadlines.

#### Embargo Strategy
- OFFER embargoes to Tier 1 outlets for exclusive early access to news
- Standard embargo: give 3-5 days advance access before public announcement
- NEVER embargo more than one outlet at the same tier for the same story
- Embargo email format: clearly state date/time of lift, what's embargoed, consequences

#### Follow-Up Cadence
- Day 0: initial pitch
- Day 4: follow-up with NEW information (not "just checking in")
- Day 10: completely different angle or new news hook
- Day 14+: stop. They're not interested in this story. Move on.
- EXCEPTION: if they replied at all (even "not now"), they go on the warm list

### 7. The Press Snowball
After first coverage lands:

#### 7a — Amplify Existing Coverage
- Share the article across all social channels with genuine commentary (not just "we got covered!")
- Tag the journalist with a thank-you (public goodwill, they appreciate amplification)
- Send the article to other journalists: "as covered in [outlet]..." — social proof

#### 7b — Chain Reactions
Using Exa.ai or Serper:
- Search for who shared or referenced the original article
- Find journalists who cover similar topics to the one who wrote about you
- Pitch THEM with a fresh angle + citation of existing coverage
FALLBACK: manually search Twitter/X and Google News for references to the article.

#### 7c — The Snowball Principle
- Each piece of coverage makes the next pitch easier
- Maintain a "coverage page" or list that grows over time
- Reference prior coverage in every subsequent pitch (social proof)
- Track the chain: Article A led to Pitch B which led to Article C

#### 7d — Memory Tracking
Store in memory after each coverage win:
- Outlet name + article URL
- Journalist name (now a warm contact)
- Which angle worked
- Referral domain authority (for SEO value tracking)
- Traffic impact (if user provides analytics)

### 8. Regional Press Strategy

#### Why Local First
- Local tech/business reporters are 10x more responsive than national
- "Local founder" is inherently newsworthy in regional outlets
- Local coverage creates national-tier backlinks (same SEO value)
- Regional pieces get picked up by wire services and aggregators

#### Finding Local Journalists
For founder's city/region:
1. Serper (primary): search "[city] tech news" + "[city] startup news" + "[city] business journal"
2. Exa.ai (secondary): semantic search for technology reporters in [city/region]
3. Hunter.io: find emails at local publication domains
4. FALLBACK: every major metro has a Business Journal (bizjournals.com/[city]), a local tech blog, and local TV stations with tech/business reporters. List these for the user's city.

#### Local Pitch Angle
Template: "[City] founder builds [product] to solve [problem] — [traction proof point]"
- Emphasize local job creation, local office, local customers
- Reference other local startups or tech scene growth
- Offer to be a source for future local tech stories (relationship building)

#### Stepping Stone Strategy
1. Land local business journal coverage
2. Pitch regional tech blog citing local coverage
3. Pitch industry-specific outlet citing growing coverage
4. Pitch national outlet with full coverage portfolio

### 9. HARO / Connectively / Source Requests

#### What It Is
HARO (Help A Reporter Out) / Connectively sends daily emails with journalist queries seeking sources. Responding makes you the EXPERT, not the pitcher — completely different dynamic.

#### Monitoring Setup
- Sign up at connectively.us (formerly HARO) — free tier available
- Set alerts for your industry keywords
- Check 3x daily (morning, midday, evening sends)
- Respond within 2 hours of relevant query (speed wins)

Using Serper: periodically search "HARO" + "[your industry]" + "looking for sources" to find journalist queries posted publicly on Twitter.

#### Response Template
When a relevant HARO query appears:

SUBJECT: [Re: their query subject line] — [Your name], [credential]

[First name or "Hi"],

[Direct answer to their question in 2-3 sentences. Lead with the insight, not your bio.]

[One supporting data point or example from your experience.]

[One contrarian or surprising take that makes your quote stand out from the other 200 responses.]

For attribution: [Name], [Title] at [Company] ([one-liner about company]).

Happy to elaborate or provide additional data.

[Name]
[Contact info]

#### HARO Power Moves
- Respond to queries even slightly outside your lane (adjacent expertise counts)
- Include a quotable soundbite — journalists copy-paste, make it easy
- Attach a headshot (many won't use you without one)
- Be available for follow-up within hours (not days)
- Even if they don't use your quote, you're now in their contacts

### 10. Measurement

#### Track in Memory After Each PR Cycle
Pitches:
- Total pitches sent
- Response rate (any response, even "no thanks")
- Coverage conversion rate (pitches that became articles)
- Best-performing angle (which of the 5-7 angles landed)
- Best-performing tier (which tier converted best)

Coverage:
- Outlet name + URL
- Domain authority of the outlet (check via Serper or ask user)
- Estimated reach/readership
- Social shares of the article
- Backlink SEO value (dofollow vs nofollow)

Impact:
- Traffic spikes from each piece (ask user for analytics)
- Sign-up or conversion spikes correlated with coverage
- Inbound interest generated (investors, partners, customers who cited the article)

Relationships:
- Warm journalist list (responded positively, even if didn't cover this time)
- Hot journalist list (covered you — nurture for future stories)
- Journalist preferences noted (preferred pitch style, best contact method, topics they care about)

#### PR Scorecard (generate after each cycle)
  PITCHES SENT: [n]
  RESPONSE RATE: [%]
  COVERAGE LANDED: [n articles]
  TOTAL ESTIMATED REACH: [n readers]
  HIGHEST-TIER COVERAGE: [outlet name]
  BEST ANGLE: [which angle]
  BACKLINK DA AVERAGE: [domain authority]
  NEXT MOVE: [recommended next action based on results]
