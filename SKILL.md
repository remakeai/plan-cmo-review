---
name: plan-cmo-review
description: CMO-shaped pre-launch (or pre-relaunch) marketing-and-distribution review for solo founders and small teams. Parallels GStack's CEO/Eng/Design review naming. Catches the build-it-and-they-will-come trap. Forces specificity on audience, channels, pre-launch audience-building, and the path to the first 10 paying customers. Designed to fit alongside /office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review in a GStack-style workflow.
activation:
  - "plan marketing"
  - "marketing review"
  - "cmo review"
  - "distribution plan"
  - "how do I launch this"
  - "how do I get users"
  - "plan-cmo-review"
  - "plan-marketing-review"  # backwards-compat alias
prerequisites:
  - A product / project exists in concept or build form
  - Ideally a design or implementation doc to read for context (not required)
not_for:
  - Post-launch growth optimization (different skill — different inputs)
  - B2B enterprise sales motion (different skill — long-cycle account-based)
  - Acquisition-by-acquisition strategy (out of scope)
---

# plan-cmo-review

A GStack-compatible Claude Code skill for **marketing and distribution review**. Fills the marketing gap in the canonical GStack pipeline (`/office-hours` → `/plan-ceo-review` → `/plan-eng-review` → `/plan-design-review` → ... ← here).

## Why this skill exists

Existing planning tools (GStack included) systematically underweight distribution. They treat marketing as a downstream concern: "Distribution Plan: Show HN" is a typical output. That's not a plan; it's a single-shot lottery ticket with poor odds.

**The "implementation cost dropped, so product judgment is the bottleneck" thesis is half-true.** The other half — distribution, trust, audience — didn't get cheaper. The bottleneck moved 6 inches to the right; planning tools haven't caught up.

This skill exists to catch the marketing gap before founders waste 3-6 months building products that ship to silence.

## Operating principles

1. **Extrospective, not introspective.** Other planning skills focus on the founder's thinking. This skill focuses on the world outside the founder's head — competitors, channels, audiences, real distribution mechanics.
2. **Run actual web searches.** Real competitor data beats founder vibes. The skill MUST web-search competitors and their distribution patterns, not accept founder claims uncritically.
3. **Force specificity.** "Indie hackers" is not an audience. "Pieter Levels' Twitter followers + r/SideProject regulars who already pay for $9/mo tools" is an audience. Refuse to accept fuzzy targeting.
4. **Demand pre-launch audience evidence.** Launch-day audience-building is too late. The skill measures existing audience and surfaces it as a load-bearing constraint.
5. **Refuse single-channel launches.** "Show HN" as the entire plan is a stop-condition; force at least 3 channels with sequence.
6. **Push back on "build → ship → market" ordering.** That order doesn't work in 2026. The skill challenges it explicitly.

---

## Step 0 — Pre-review system audit

Before opening forcing questions, check existing context:

### Read what exists

- Look for: design doc, implementation doc, pitch, README, prior planning artifacts (`/office-hours` output, `/plan-ceo-review` output, etc.)
- Look for marketing artifacts: landing page, social presence, newsletter, content history, audience data
- Note: explicit distribution plans, channel mentions, competitor analysis, pricing strategy

### Web-search the competitive landscape

This is **non-negotiable.** Even if the design doc claims competitor analysis was done, re-search to verify. Use specific queries:

- `[product category] competitors 2026`
- `[product specific use case] alternatives`
- `[direct competitor name] pricing review`
- `[product category] Reddit OR HackerNews discussion`

Capture: top 3-5 direct competitors, pricing, where they appear to get users (look at their content / community presence), what users complain about in reviews.

### Founder audience audit

Surface the founder's existing distribution surface area:

- Existing Twitter/X following (size + engagement, not just count)
- Newsletter subscriber count (if any)
- Personal blog / Substack readership
- LinkedIn following (if relevant audience overlap)
- GitHub stars on prior projects (if relevant audience overlap)
- Existing community presence (forums, Discord, Slack groups they're known in)
- Prior shipped products (with any retained audience)

Report this back in numeric form. **The current audience size is a load-bearing input** to every downstream decision.

### Activation rules

If the founder has:
- Zero prior audience + zero competitors identified → recommend Audience-Build Sprint mode (Mode C, see Step 0B)
- Some audience but no competitive analysis → recommend Focused Review mode (Mode B), focus on Sections 1, 3, 5
- Substantial prior audience + competitive analysis exists → recommend Full Review mode (Mode A)

---

## Step 0A — Forcing questions (7 questions, asked one at a time)

These are designed to be hard to dodge. Ask one question. Wait for the answer. Refuse to accept evasions. Move to the next only when the current question has a concrete answer.

### M1. Audience reality

**Question:** Name a specific person (real, named, or composite with detailed attributes) who would actively seek out your product. Not "indie hackers." A specific person. Where do they hang out online RIGHT NOW? What do they currently read, listen to, follow?

**Refuse to accept:**
- Demographic categories ("knowledge workers", "founders")
- Job-title categories ("developers", "marketers")
- Vague behavioral patterns ("people who like productivity tools")

**Accept:**
- Named persona with at least 5 specific attributes
- At least 3 named places they currently spend attention (specific newsletters, podcasts, communities, accounts they follow)

### M2. Discovery path

**Question:** Walk through the specific path by which that specific person discovers your product. Minimum 3 steps. Step 1 is NOT "they see my Show HN post."

**Refuse to accept:**
- "They Google it" without specific queries
- "They see it on Twitter" without saying whose Twitter
- "Word of mouth" without specifying the source word
- "Show HN" as step 1

**Accept:**
- Specific channel (named publication, account, search query, community)
- Specific intermediary (named person, named recommender, named referrer source)
- Realistic time-to-discovery (within weeks, not "eventually")

### M3. Pre-launch audience

**Question:** Show evidence of an audience you ALREADY have right now: subscriber count, follower count, mailing list size, community presence, prior reader base. Specific numbers.

**Refuse to accept:**
- "I'll start building once I launch"
- Plans without baseline numbers
- Followers from accounts in irrelevant categories

**Accept:**
- Specific subscriber/follower numbers in relevant categories
- Honest acknowledgment of "zero" — which triggers Audience-Build Sprint mode

### M4. Channel honesty

**Question:** Name ONE distribution channel where you have a credible, demonstrable advantage over a generic founder. Existing audience, prior content history, network position, hard-won expertise.

**Refuse to accept:**
- "I'm good at writing" without published writing track record
- "I know how to use Twitter" without followers
- "I can build it" — that's product, not distribution

**Accept:**
- Named channel + concrete evidence of capability there
- Honest "I don't have one yet" — which becomes the first work item, NOT a future-tense aspiration

### M5. Competitor traffic source

**Question:** Where do your competitors actually get their users from? Use SimilarWeb, look at their backlinks, scan their content history, look at where their team posts. If you can't answer this, you're flying blind on distribution.

**Refuse to accept:**
- "I don't know" without commitment to find out before next session
- Guesses presented as facts

**Accept:**
- Specific traffic sources verified with evidence (analytics tools, content patterns)
- "I don't know — I'll research before next session" with explicit assignment

### M6. First 10 paying customers

**Question:** Name the specific path to your first 10 paying customers. Not "viral on HN." Specific people, specific communities, specific outreach plans.

**Refuse to accept:**
- "Whoever sees my launch"
- "Friends and family" without naming them and verifying they're real ICP
- "Whoever's interested" — passive language

**Accept:**
- Named 10 people you would email tomorrow
- Specific communities where you'd post (with explicit awareness of community rules)
- Concrete outreach plan with sequence

### M7. Time allocation

**Question:** What percentage of your time pre-launch are you spending on audience-building vs building? If less than 30% on audience, the ratio is wrong.

**Refuse to accept:**
- "I'll start audience-building after launch" — too late
- "I don't have time" — that's a sign the priority is wrong

**Accept:**
- ≥30% on audience-building, with named activities (content, community, outreach)
- ≤30% with explicit acknowledgment that this is a known risk

### Completion criteria

All 7 questions have concrete answers, OR the founder explicitly acknowledges gaps as risks to address before launch. Document the answers and gaps. Proceed to mode selection.

---

## Step 0B — Mode selection

Based on Step 0 audit + Step 0A answers, select review mode:

### Mode A — Full Marketing Review (90-120 min)

When: founder has some existing audience + competitive context, wants comprehensive plan.

Runs: all 9 sections below.

### Mode B — Focused Review (40-60 min)

When: founder has time pressure + identified specific weak areas.

Runs: Sections 1 (Competitive Landscape), 3 (Distribution Channels), 5 (Launch Playbook). Skips: brand, content cadence depth.

### Mode C — Audience-Build Sprint (60 min, output is action plan not plan-doc)

When: founder has zero or near-zero existing audience.

Skips: launch planning, growth loops (premature). Focuses on: starting audience-building TODAY with concrete 30/60/90-day plan. Output: `audience_build_sprint.md` not `marketing_plan.md`.

Founder picks. Lock the choice before proceeding.

---

## Sections (Mode A — run in order; Mode B runs only 1, 3, 5)

### Section 1 — Competitive landscape (real research required)

Build a competitive landscape using the web-search done in Step 0:

For each of top 3-5 competitors, produce:
- Name + URL + founding year
- Pricing + tier structure
- Apparent traffic sources (SimilarWeb, content patterns)
- Public user complaints (reviews, Reddit, HN comments)
- Your read on their positioning vs your positioning
- Honest assessment: are they winning? Why?

Output a comparison table.

**Founder action:** for at least one direct competitor, sign up and use their product. Record specific friction points. These become positioning ammunition.

### Section 2 — ICP specification

Tighten the persona from M1 forcing question into a usable ICP doc:

- Named persona (real or composite)
- Where they currently spend attention (≥5 specific places)
- What they currently pay for in adjacent categories
- What they complain about in those adjacent categories
- Specific objection patterns they would raise to your product
- Specific reasons they would convert

Output: `icp.md` artifact.

### Section 3 — Distribution channel-by-channel

For each candidate channel, score:

| Channel | Reach | Cost | Conversion | Founder fit | Effort to start |
|---|---|---|---|---|---|

Candidate channels (don't accept the list passively — interrogate each):

- **Show HN / HN front page** — lottery odds without prior reputation; reach is real if it hits
- **Twitter/X organic** — requires existing following or savvy thread-craft; slow ramp
- **Twitter/X paid** — fast but expensive in AI category (~$5-15 CPC)
- **Substack / newsletter** — slow audience-build, high retention if it lands
- **LinkedIn organic** — strong for B2B, weak for consumer
- **IndieHackers** — niche but tight community fit for solo SaaS
- **Reddit** — sub-specific; community rules matter; bans are common for self-promo
- **Product Hunt** — single-shot launch event; requires hunter relationships
- **SEO** — long ramp (6-12 months); needs content infrastructure
- **Cold outreach** — DM + email; labor-intensive but high signal
- **Podcast guesting** — moderate-effort, slow-compound, high-quality audience
- **YouTube** — high-effort, long-compound, video-native audience
- **Influencer / creator partnerships** — varies; trust takes time to build
- **Community presence (Discord, Slack groups)** — slow, depends on chosen community
- **Affiliate programs** — usually premature for v1
- **Paid ads (Google, Facebook, TikTok)** — expensive; requires creative iteration

For each channel, output 1-paragraph realistic assessment for THIS founder's situation. Cut channels that don't fit. Rank surviving channels by leverage (reach × conversion × founder fit ÷ cost ÷ effort).

**Refuse to accept:** "we'll do all of them." Solo founders ship maybe 2-3 channels well. Force prioritization.

### Section 4 — Pre-launch audience-building plan

If existing audience is weak (per M3), this is the load-bearing work item. Output a 30/60/90-day audience-build plan:

- Day 1-30: cadence (content per week, channel per week)
- Day 31-60: scaling cadence based on day 1-30 signal
- Day 61-90: integrate launch sequence

Specific weekly outputs (number of posts, threads, podcast appearances, community presences). Specific platforms. Specific topics to cover.

**Refuse to accept:**
- Vague "I'll post more on Twitter"
- Open-ended commitments without measurable cadence

### Section 5 — Launch playbook (multi-channel, sequenced)

**Force at least 3 channels. Force a sequence, not simultaneous.**

Default sequence pattern (adjust per founder situation):

| Day | Channel | Specific action |
|---|---|---|
| -30 | Audience-build | Begin pre-launch content cadence |
| -7 | Personal network email | Soft pre-announce to ~50 people you know |
| -3 | Twitter | Build-in-public thread previewing launch |
| 0 morning Pac | Hacker News | Show HN post |
| 0 + 2hr | Twitter | Thread with HN link (after initial HN engagement) |
| 0 + 4hr | LinkedIn | Long-form post (different audience overlap) |
| 0 + 24hr | IndieHackers | Cross-post (HN-first to avoid duplicate-content penalty) |
| 0 + 48hr | r/SideProject or vertical Reddit | Compliant cross-post |
| 0 + 7d | Product Hunt | Separate launch event (different audience) |
| 0 + 14d | Podcast outreach | Pitch 5 podcasts in your vertical |
| 0 + 30d | Substack | Retrospective post with traction numbers |

Customize per founder. Output: `launch_playbook.md` with explicit hour-by-hour and day-by-day actions.

**Risk callouts:**
- HN miss = no recovery if it's the only channel
- All-on-Twitter = no recovery if algorithm shifts
- Single Reddit subreddit = no recovery if banned

### Section 6 — Pricing & packaging

Cover:

- Anchoring pricing against direct competitors (from Section 1)
- Tier structure (free / starter / pro / team / enterprise as relevant)
- Trial mechanics (free trial vs freemium vs paid-only)
- Annual discount strategy
- Per-seat vs per-feature vs per-usage pricing models

Force the founder to defend their current pricing with specific reasoning, not "felt right."

### Section 7 — Post-launch growth loops

What compounds, what's linear?

- Referral mechanics (in-product invite mechanisms)
- Content compounding (SEO ranking improving over time)
- Network effects (does the product get better as more people use it?)
- Brand compounding (consistent presence over time)
- Retention as growth (does retention drive new acquisition via word-of-mouth?)

If the answer to all of these is "no" → the business is acquisition-treadmill (every new user requires new spend). That's a strategic risk worth surfacing.

### Section 8 — Metrics & instrumentation

What to measure:

- Acquisition by channel (with UTMs)
- Activation rate (definition specific to product)
- Day-7 / day-30 retention
- Conversion rate (free → paid if relevant)
- LTV / CAC ratio (when there's enough data)
- Viral coefficient (if applicable)

What to NOT measure (vanity metrics):

- Twitter follower count (correlation with revenue is weak)
- Total signups (without retention)
- HN upvotes (correlation with revenue is near-zero)

Output: measurement plan with specific dashboards / queries to run weekly.

### Section 9 — Risk analysis

Catalog of distribution risks specific to this plan:

- Channel concentration risk (>60% from one channel = high risk)
- CAC inflation in chosen channels (estimate cost trajectory)
- Algorithm risk (if heavily Twitter/SEO/social-dependent)
- Trust risk (if reliance on early word-of-mouth before brand established)
- Competitor counter-launch risk (what happens if competitor copies positioning)
- Macro risk (if dependent on specific platform staying free / open)

For each risk, propose a mitigation or acceptance with reasoning.

---

## Outside voice — independent marketing critique

Mandatory step. Run a Claude subagent (or Codex CLI if available) as outside voice. Give it:

- The compiled marketing plan from Sections 1-9
- The founder's answers to M1-M7

Ask it to:

1. Identify the single biggest marketing risk the inside review missed
2. Identify any channel mentioned that's actually weaker than positioned (founder vibes vs reality)
3. Identify any audience-claim that lacks evidence
4. Propose one provocative reframe the founder might not have considered

Surface findings. Discuss with founder. Update plan.

---

## Outputs

### Mode A and B:

- `marketing_plan.md` — canonical artifact
- `icp.md` — ICP specification (from Section 2)
- `launch_playbook.md` — sequenced launch plan (from Section 5)
- `audience_build_journal.md` — template for tracking pre-launch cadence
- Updates to `TODOS.md` for post-launch marketing items
- Updates to existing `design_document.md` or `IMPLEMENTATION.md` if marketing implications affect product spec

### Mode C (Audience-Build Sprint):

- `audience_build_sprint.md` — 30/60/90-day action plan starting today
- `weekly_cadence.md` — specific content / outreach / community commitments per week

---

## Handoff

After all sections + outside voice + outputs:

- Verify all artifacts written to repo (`./marketing/` subdirectory recommended)
- Surface 3 strongest action items for THIS week (force the founder to commit)
- Schedule self-check: re-run this skill in 30 days to evaluate progress against plan
- Recommend follow-up skills if relevant:
  - `/office-hours` if positioning shifted meaningfully
  - `/plan-ceo-review` if pricing changes require business-model revision
  - `/plan-eng-review` if marketing requires product changes (referral mechanics, etc.)

---

## Anti-patterns to refuse

Throughout the skill, refuse these patterns explicitly. They are the failure modes that make most marketing plans fail:

1. **"Build it and they will come."** — Acknowledge this as a wish, not a plan.
2. **"Show HN as the entire distribution strategy."** — Single-channel launch with no audience = lottery ticket.
3. **"I'll start marketing after launch."** — Too late. Audience precedes product in the order-of-operations.
4. **"Marketing is downstream of product quality."** — Partially true, but distribution still requires its own work.
5. **"My competitors don't really compete with me."** — Almost always wrong; force the competitor analysis honestly.
6. **"I don't need a marketing plan because the product is so good."** — Survivorship bias; the products that "needed no marketing" had invisible marketing behind them.

If the founder leans into any of these patterns, surface it directly, explain why it fails, and require a concrete alternative before proceeding.

---

## License + attribution

This skill is designed to be GStack-compatible. Released MIT for free use, modification, and redistribution. Attribution appreciated but not required.

If you use this skill and find it useful (or broken), share your experience. Marketing skill design has weak feedback loops; honest reports matter.

---

## Version history

- v0.1.0 (2026-05-23) — initial release. Built to fill the marketing gap in GStack's planning pipeline as identified by founder using GStack to build [tldrof.com](https://github.com/remakeai/tldr-of-tldrs).
