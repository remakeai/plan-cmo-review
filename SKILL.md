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

1. **Default founder assumption: technically strong, marketing-naive** (unless evidence proves otherwise). The typical user of this skill ships product reliably but has never sold one. Their marketing-related assertions — pricing, ICP, channels, launch platform, dogfood mix, "no anti-features in scope," calendar-driven launch dates — are SUSPECT BY DEFAULT and should be challenged before being optimized within. The only input accepted on faith (and even then with room for tweaks) is the **product description itself** (what the product does, how it works). Everything else gets premise-audited in Step 0.5.
2. **Extrospective, not introspective.** Other planning skills focus on the founder's thinking. This skill focuses on the world outside the founder's head — competitors, channels, audiences, real distribution mechanics.
3. **Run actual web searches.** Real competitor data beats founder vibes. The skill MUST web-search competitors and their distribution patterns, not accept founder claims uncritically.
4. **Force specificity.** "Indie hackers" is not an audience. "Pieter Levels' Twitter followers + r/SideProject regulars who already pay for $9/mo tools" is an audience. Refuse to accept fuzzy targeting.
5. **Demand pre-launch audience evidence.** Launch-day audience-building is too late. The skill measures existing audience and surfaces it as a load-bearing constraint.
6. **Refuse single-channel launches.** "Show HN" as the entire plan is a stop-condition; force at least 3 channels with sequence.
7. **Push back on "build → ship → market" ordering.** That order doesn't work in 2026. The skill challenges it explicitly.
8. **Premise-challenge before tactic-sharpen.** Tactical questions optimize WITHIN whatever framing the design doc accepted. If the framing is wrong, sharper tactics polish wrongness. Step 0.5 runs FIRST; tactical Step 0A questions inherit Step 0.5's findings.

### Evidence that overrides the default

The "marketing-naive by default" assumption flips ONLY when one or more of these are true:

- Founder has shipped ≥1 prior consumer/B2B product with verifiable paying traction at >$10K MRR
- Founder has a demonstrated marketing track record: published writing with measurable audience, prior brand-building work, named marketing roles at growth-stage companies
- Founder's existing audience surface area (per Step 0 audit) is genuinely large AND ICP-aligned (not just count — relevance)
- Founder has documented prior failed launches WITH retrospective analysis showing they learned the distribution lessons

If NONE of the above apply, default holds. Surface this explicitly in Step 0.5 findings: *"Working under marketing-naive default; premise-challenge is load-bearing."*

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

Audience SIZE is the primary mode-selection axis, but **ICP-ALIGNMENT modifies it**. Audience-count alone is not enough — a 10K-follower audience in the wrong category counts as zero for this product.

- **Mode C (Audience-Build Sprint)** — fires when the founder has effectively zero ICP-aligned audience for THIS product. Triggers: <500 followers in the relevant category, OR an existing audience in a different category from the product's ICP (e.g., 996 LinkedIn followers in semiconductors for a consumer newsletter product = Mode C), OR no content history demonstrating attention from the right audience.
- **Mode B (Focused Review)** — fires when the founder has SOME ICP-aligned audience AND time pressure or scope constraints make a full plan premature. Default to Mode A when in doubt; Mode B is a deliberate downgrade for compressed timelines, not the default for "some audience."
- **Mode A (Full Marketing Review)** — fires when (a) founder has ≥1K ICP-aligned attention surface AND competitive context exists, OR (b) the product is mid-build with a hard launch date and needs both audience-build AND a sequenced launch plan in one pass.

**Mode A vs C tie-breaker (load-bearing — this is the case the v0.2 b2b-saas runs disagreed on):** if the founder is mid-build with a hard launch date AND has either a small (<500) OR ICP-misaligned audience, prefer **Mode A with Section 4 elevated** (full plan PLUS embedded audience-build sprint) over Mode C alone. Reason: Mode C alone skips the launch playbook the founder still needs to ship; Mode A with elevated Section 4 produces both. Choose Mode C only when no launch is contemplated within the next 90 days.

---

## Step 0.5 — Premise audit (5 questions, run BEFORE Step 0A)

**This step is load-bearing under the marketing-naive default.** Step 0A's tactical questions sharpen execution within whatever framing the design doc accepted. If the framing is wrong, Step 0A polishes wrongness. Step 0.5 attacks the framing first.

The design doc's PRODUCT description is accepted on faith (with room for tweaks). Every MARKETING claim in the design doc — pricing, ICP, launch platform, dogfood mix, channels, in-scope features — is treated as suspect input requiring justification, not as locked truth.

### Premise extraction (do this first)

Read the design doc. Extract every marketing-relevant premise it accepts as given. Surface as a table:

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|

Typical marketing premises in a technical founder's design doc:

- **Launch platform** (often "Show HN")
- **Audience class** (often the founder's own peer group)
- **Pricing point AND pricing band** (often anchored on direct competitor pricing)
- **Dogfood mix** (often the founder's own subscriptions / use cases)
- **Launch gate** (often calendar-driven: "ship by day N")
- **In-scope features** (often includes power-user features that contradict positioning)
- **Channels** (often a single channel the founder knows: HN, Twitter, etc.)

The "Likely-wrong because" column is a HYPOTHESIS to test in M0a–M0e below, not an answer.

### M0a. Launch-platform audience-class fit

**Question:** Is the planned launch platform the right *audience class* for this product, or just the platform the founder is familiar with?

**Pattern this catches:** "Show HN as the launch" for consumer-habit products whose actual buyers aren't on HN. HN is excellent for some product categories (dev tools, developer-facing infra) and a CATEGORY ERROR for others (consumer subscriptions for non-technical buyers, regulated-industry SaaS). Same applies to Twitter for non-Twitter-native audiences, LinkedIn for consumer products, etc.

**Web-search to support:** look up similar products that did/didn't succeed via the planned platform. Specifically search "Show HN [product category]" results and check which got traction vs which got <5 upvotes (the "Hidden Signal" base rate).

**Refuse to accept:**
- "It worked for [X product]" without checking if X was the same product category and audience class
- "It's where founders hang out" — founders aren't always the buyer for the product being built
- "Other founders launched there" — survivor bias

**Accept:**
- Specific evidence the platform's audience overlaps with the product's actual ICP
- Honest acknowledgment that the platform was chosen because it's familiar to the founder, NOT because of audience fit — which then triggers an audience-fit re-analysis

### M0b. Canonical-success comparable

**Question:** Name the most successful product in this category at this motion class (consumer subscription / B2B SaaS / dev tool / marketplace / etc.). What did they do that the current plan does NOT?

**Pattern this catches:** plans that don't anchor against precedent. Most categories have 1-3 standout successes (Superhuman for premium-concierge consumer SaaS, Readwise for niche-indispensable subscription, Linear for design-led B2B, Stripe for developer-first infrastructure). Ignoring them produces from-first-principles plans that miss known playbooks.

**Web-search to support:** mandatory. Search for "[category] biggest success" / "[motion class] case study" / "[product type] won via." Specifically look for products that are KNOWN to have succeeded, NOT just direct competitors. Direct competitors are the alternatives; canonical successes are the precedents.

**Refuse to accept:**
- "There's no real comparable" — usually false; the founder hasn't searched yet
- Direct-competitor names only without canonical-success additions
- "Our motion is novel" — almost always wrong; named the wrong motion class

**Accept:**
- Named successful product with documented playbook + specific delta between their motion and current plan
- For each canonical success: pricing, primary acquisition channel, onboarding model, gate metric. Cited.

### M0c. Anti-feature surface

**Question:** Name 2+ features currently in scope that contradict the stated positioning, trust model, or business model.

**Pattern this catches:** Features that "sound good" but undermine the wedge. BYO-API-key for a trust-positioned product. Free tier for a premium-positioned product. Self-serve onboarding for a concierge-positioned product. MCP / programmatic integrations for a product whose paying ICP is non-technical. Power-user customization for a product positioning as zero-effort.

**How to find them:** read the in-scope feature list in the design doc. For each feature, ask: "Who does this serve, and is that person the paying ICP?" If the feature serves a segment that won't pay (technical DIY-by-instinct users for a consumer product, free-tier non-converters for a premium product), flag as anti-feature candidate.

**Refuse to accept:**
- "None of our features contradict positioning" — push back; look at the feature list line by line
- "Users want it" without showing that PAYING users want it (different segment)
- Defenses based on "it's optional" — optional features still split the product story

**Accept:**
- Named feature + specific contradiction explained
- Honest "I found N candidates; here's why each contradicts" only after an actual line-by-line check
- Acknowledgment that "kill, defer to v2, or restrict to enterprise tier" is the decision the founder owes themselves

### M0d. Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the planned acquisition tactic select for the wrong segment? Specifically: do free trials, cheap try-it offers, no-credit-card signups, or other low-commitment-low-risk acquisition mechanics attract people whose profile is OPPOSITE to the paying ICP?

**Pattern this catches:** Plans where the validation cohort is time-rich/money-poor (people willing to gamble time on uncertain product trials) but the paying ICP is time-poor/money-rich (people who buy on trust and don't trial-shop). Cheap trial mechanics are validation theater for the wrong segment.

**Diagnostic:** map the proposed acquisition tactic to the segment it ACTUALLY attracts:
- "Free trial, no CC required" → time-rich, low-commitment users
- "$1 reservation" → engaged but not paying customers
- "30-day money-back guarantee" → cautious buyers (any segment)
- "Concierge onboarding waitlist" → committed prospects, willing to wait, signal serious intent
- "Referral from someone they trust" → trust-led ICP, often time-poor/money-rich
- "Paid placement in trusted publication" → segment of that publication's audience

Then compare: is the attracted segment the same as the paying ICP? If not, the validation signal is misleading.

**Refuse to accept:**
- "Everyone tries products before buying" — not true for time-poor segments
- Defenses of the trial mechanic based on conversion-funnel orthodoxy ("industry standard is 7-day trial") without checking if industry-standard applies to this ICP
- "Free tier is just for top-of-funnel" — top-of-funnel still shapes brand perception and word-of-mouth pool

**Accept:**
- Honest assessment of which mechanic produces which selection bias
- Acknowledgment that high-trust acquisition (referral, comparable-recommendation, concierge) may be the right mechanic for time-poor segments — even if it scales slower

### M0e. Dogfood audience-class match (founder vs paying ICP)

**Question:** Is the audience the product was dogfooded on the same audience that will actually buy it? Or is the product being tuned to a proxy audience whose incentives differ from the paying ICP?

**Pattern this catches:** technical founders dogfood on themselves (technical audience) and tune the product for that audience, then plan to sell to non-technical buyers whose needs/behaviors are different. The product ships calibrated to the wrong audience. Specific failure modes:

- Dogfooded on developer newsletters; planning to sell to general professionals → dedup value is different, content style is different
- Dogfooded on free OSS users; planning to sell to enterprise → feature priorities are different
- Dogfooded on founder's own use case; planning to sell to a segment with adjacent-but-not-same needs

**Refuse to accept:**
- "The product works for anyone" — usually false; tuning has an audience signature
- "I'll re-tune after launch" — too late; first-cohort users entrench the audience identity
- "Both audiences need the same thing" — sometimes true, often not; force the comparison
- **"I'll defer the paying ICP and target the dogfood-aligned audience first"** — this is the most common wrong fix. The plan correctly identifies the mismatch, then PRESERVES the mismatch by deferring the right audience and keeping the wrong one. The correct fix is to PIVOT the target audience toward the paying ICP AND expand dogfood subjects to match. Both pivots are required. Doing only one (or worse, deferring the paying ICP entirely) keeps the mismatch and ships the product calibrated to the wrong audience.

**Accept:**
- Specific evidence dogfood audience = paying ICP (e.g., paying interviews with the actual ICP saying "this matches my needs exactly")
- Honest acknowledgment of mismatch + concrete plan with BOTH pivots: (a) pivot the TARGET audience in marketing materials, ICP doc, and launch sequencing to the paying ICP (not the dogfood-aligned proxy), AND (b) expand dogfood subjects to include paying-ICP-representative inputs BEFORE launch (1-2 weeks of buyer-aligned dogfood minimum). The fix is "pivot both," not "defer the paying ICP."

### Pricing-band sub-check (rolled into Section 6 if Step 0.5 doesn't already surface it)

Pricing has its own dedicated forcing question in Section 6 (Pricing & packaging). Step 0.5 surfaces pricing-band questions IF the design doc treats the price point as locked without ICP willingness-to-pay evidence. If surfaced here, also revisit in Section 6 with full depth.

### Completion criteria for Step 0.5

For each of M0a–M0e:
- Premise stated
- Web search performed (where applicable)
- Verdict: **premise survives / premise fails / premise inconclusive**
- If failed: cascading implications for the rest of the marketing plan documented

Document findings. Premises that failed challenge become EXPLICIT context for Step 0A. The tactical forcing questions in Step 0A know about Step 0.5 findings and adjust accordingly:
- If M0a flagged launch platform as wrong audience class, M2 (discovery path) refuses "Show HN as step 1" even more aggressively
- If M0d flagged freebie-disqualifier, M5/M6 push toward high-trust acquisition mechanics
- If M0e flagged dogfood mismatch, M1 (audience reality) requires the corrected ICP, not the dogfood ICP

If ≥2 of M0a–M0e fail, document a **PREMISE-LEVEL FINDINGS BLOCK** at the top of the eventual marketing_plan.md, BEFORE the tactical sections. This is the single highest-value thing the skill produces under the marketing-naive default.

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

Build a competitive landscape using the web-search done in Step 0. **TWO classes of comparable are required — direct competitors AND canonical-success comparables. Do not skip the second class.**

#### 1a. Direct competitors

For each of top 3-5 direct competitors, produce:
- Name + URL + founding year
- Pricing + tier structure
- Apparent traffic sources (SimilarWeb, content patterns)
- Public user complaints (reviews, Reddit, HN comments)
- Your read on their positioning vs your positioning
- Honest assessment: are they winning? Why?

Output a comparison table.

#### 1b. Canonical-success comparables (this is the part most plans skip)

For this product's motion class (consumer subscription / B2B SaaS / dev tool / marketplace / etc.), identify 2-4 **canonical successful products** — NOT direct competitors, but products that PROVE the playbook at this motion class. Examples by motion class:

- **Premium-concierge consumer subscription:** Superhuman ($30/mo, $825M acquisition Jul 2025) — manual concierge onboarding (Vohra personally did first 200), invite-only waitlist, two-sided referral
- **Niche-indispensable consumer subscription:** Readwise (~$10/mo, ~$14M ARR, >90% retention) — bootstrapped, product-led, partnerships, no paid acquisition
- **Design-led B2B:** Linear — bottom-up adoption, polish-as-marketing, founder presence
- **Developer-first infrastructure:** Stripe — docs as marketing, developer relations team
- **Two-sided marketplace:** Airbnb — manual supply-side acquisition before demand
- **Content-led SaaS:** ConvertKit, Ahrefs — content cadence as the primary channel

For each canonical success, produce:
- Name + price + founding year + current scale
- Primary acquisition channel (verified, not vibes)
- Onboarding model (self-serve / concierge / hybrid)
- Launch gate they used (PMF signal / calendar / waitlist threshold)
- Specific delta between their playbook and the current plan — what did they do that this plan does NOT?

Output a separate comparison table.

#### 1c. Pattern surface

After both tables exist, write a 1-paragraph pattern read:
- What do the canonical successes have in common that the current plan lacks?
- Where do direct competitors diverge from canonical-success patterns?
- Which pattern is the current plan implicitly following — and is that the right one?

**Founder action:** for at least one direct competitor AND one canonical-success comparable, study their public material (founder interviews, blog post histories, podcast appearances). Record specific patterns. These become both positioning ammunition AND playbook guidance.

**Refuse to skip 1b.** Most marketing plans fail because they anchor against direct competitors (who may be losing themselves) instead of against canonical successes (which prove what works at the motion class). The direct competitor is the alternative; the canonical success is the precedent.

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

#### Motion-class-specific channel and tonal rules

The generic channel table above is necessary but not sufficient. Specific motion classes have rules that override generic scoring:

**Consumer subscription:** see Step 0.5 M0a — many channels (especially HN) are wrong audience class for non-technical buyers. A high reach score in the table for HN does NOT translate to actual reach of the paying ICP when the ICP is non-technical.

**B2B SaaS (mid-market):** generic social channels are weak; specific vertical publications carry far higher conversion. For engineering-team products, name: Pragmatic Engineer, Lenny's Newsletter, LeadDev, Rands Leadership Slack, podcasts (Software Engineering Daily, Engineering Enablement). For other verticals (legal, finance, healthcare), name the equivalent vertical publications by sector. Add these to the channel table by name, not as a generic "B2B newsletters" entry.

**Dev tool / OSS + paid:** HN IS the right audience class — do NOT apply consumer-product HN skepticism. Three dev-tool surfaces are PRIMARY (not auxiliary):

1. **Docs / SEO compounding** — integration tutorials per framework rank for long-tail queries ("Next.js auth with X", "auth in [framework]"). Treat docs as marketing, not as separate documentation. Stripe is the canonical playbook.
2. **GitHub as marketing surface** — repo health (stars, watchers, contributors, issues hygiene, recognizable adopters in dependency graphs) is real social proof. Stars >5K materially affects evaluator conversion. Ecosystem-of-integrations (first-party SDK adapters, HashiCorp HUG-style contributor recognition, named visible adopters) is its own marketing motion. Score GitHub as a PRIMARY channel for dev tools, not a code host with side benefits.
3. **Founder's existing dev-audience surfaces** — technical blog, dev-Twitter, dev-podcast guesting, prior OSS reputation. Trust transfers within the developer community in ways it doesn't in consumer or B2B-non-dev. If the founder has any of these, rank them above generic launch channels.

**Dev-tool tonal rule (LOAD-BEARING for the launch playbook in Section 5):** on Show HN, r/programming, lobste.rs, and dev-Twitter, marketing-speak tone is INVERSELY correlated with traction. Specifically REFUSE to recommend in launch copy:

- Superlatives: "revolutionary", "best-in-class", "enterprise-grade", "world-class", "game-changing", "seamless", "robust"
- Benefit-led hero copy without technical specifics
- Marketer-vocabulary phrasing in launch posts

Specifically RECOMMEND:

- Lead with technical specifics (architecture decisions, named trade-offs)
- Honest comparisons that explicitly include "this is worse at X" — saying where you lose is what makes the wins credible to the developer audience
- Code-first framing: link to the GitHub repo BEFORE the landing page on HN / Reddit
- "Engineer wrote this for engineers" tonal register; cut anything that reads as "marketer wrote this for engineers"

This is the documented anti-pattern that has killed dev-tool launches. The founder's instinct is to write copy that "sells"; the dev audience reads selling as adversarial.

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

#### 5a. Question the launch gate BEFORE producing the playbook

Most technical-founder design docs commit to a calendar-driven launch gate ("ship on day 18 / launch by end of quarter"). Calendar gates fire whether or not the product is actually indispensable. For retention-driven products (consumer subscription, B2B SaaS with high renewal dependence), the launch gate should be **PMF-signal-driven**, not calendar-driven.

**Required question (do this before writing the sequence below):**

> What is the gate that fires the launch? Calendar (day N), or PMF signal (specific dependence metric)? If the product is retention-driven, why is calendar the right gate?

PMF-signal alternatives to surface:
- **Vohra "very disappointed" test:** ≥40% of trial users answer "very disappointed" to "how would you feel if you could no longer use this." Used by Superhuman to gate public launch.
- **Engagement threshold:** N% of dogfood users use the product N times/week for N weeks
- **Word-of-mouth signal:** unprompted referrals from first cohort
- **Concierge-onboard signal:** founder personally onboards first N users; widens rollout only after N report dependence

If the product is retention-driven AND the chosen gate is calendar, the skill should propose a **concierge-first cohort** alternative (manual founder onboarding of first 10-20 users before any public launch) and surface the Vohra/Readwise/Superhuman precedent. This pairs with Insight 7-class findings from Step 0.5.

If the founder defends the calendar gate, they must do it explicitly with reasoning that survives the Vohra/Superhuman precedent. Acceptable reasons exist (developer-tool launches benefit from time-bounded marketing moments; some marketplaces need a critical-mass-day) but most retention-driven consumer products should not be calendar-gated.

#### 5b. Default sequence pattern (adjust per founder situation)

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

#### 6a. Question the pricing BAND before the price point

Most technical-founder design docs anchor on competitor pricing: "competitors are $5-15, so we'll pick $9." This is BAND-FROM-COMPETITORS thinking, which is wrong if the competitor band itself is miscalibrated against the actual paying ICP's willingness-to-pay.

**Required question (do this BEFORE optimizing the price point):**

> Did the price band inherit from competitor anchoring, or from ICP willingness-to-pay evidence? If competitor-anchored, what does the ICP actually pay for similar tools in adjacent categories?

Common ICP-WTP evidence to gather:
- What does the ICP currently pay for similar attention/time/productivity products? (Superhuman $30/mo, Readwise $10/mo, Notion $10-15/seat, ChatGPT Plus $20/mo)
- What's the documented LTV-by-price-band evidence? (RevenueCat State of Subscription Apps: $5-9 is a documented LTV-penalty band; $10-15+ retains meaningfully better; annual billing dominates retention)
- For time-poor/money-rich ICPs (typical for premium consumer SaaS), does the chosen price match their adjacent-category spend, or undershoot it?

If the band is wrong, the price point optimization is the wrong work. Surface the band question first; then if the band is confirmed, optimize within it.

**Specific failure mode to flag:** matching the cheapest direct competitor's price (e.g., "Readless is $4.90, so we should be $5-6") is a common technical-founder reflex. It's almost always the wrong move when the paying ICP is time-poor — they DON'T price-shop at the bottom of the band; they trust-shop near the top. Cheapening the price signals "commodity" to exactly the segment that buys on trust.

#### 6b. Standard pricing & packaging coverage

After the band question is answered, cover:

- Tier structure (free / starter / pro / team / enterprise as relevant)
- Trial mechanics (free trial vs freemium vs paid-only) — **revisit M0d freebie-disqualifier findings here; if cheap-trial mechanic selects against the paying ICP, propose alternatives**
- Annual discount strategy (annual billing typically increases retention dramatically — name the evidence)
- Per-seat vs per-feature vs per-usage pricing models

Force the founder to defend their current pricing AND pricing model with specific reasoning, not "felt right" and not "matches competitors."

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
7. **"Match the cheapest competitor's price."** — Common technical-founder reflex; almost always wrong for time-poor/money-rich ICPs who trust-shop near the top of the band, not price-shop at the bottom. Cheapening signals "commodity" to the segment that buys on trust.
8. **"Calendar-driven launch is fine."** — For retention-driven products, the launch gate should be PMF-signal-driven (Vohra "very disappointed" or equivalent), not calendar-driven. Calendar gates fire whether or not the product is indispensable.
9. **"Cheap-trial mechanics validate willingness to pay."** — They validate willingness to TRY for free. For time-poor/money-rich ICPs, the validation cohort and the paying cohort are different humans. Cheap-trial validation is theater for the wrong segment.
10. **"All our in-scope features serve the paying ICP."** — Most plans have at least one anti-feature that contradicts positioning. Look line-by-line at the feature list before accepting this claim.
11. **"The product works for anyone — the dogfood audience doesn't matter."** — Tuning has an audience signature. Dogfooding on technical users tunes the product for technical users regardless of who you plan to sell to.
12. **"Direct competitors are the only comparables that matter."** — Direct competitors are alternatives. Canonical-success products at the same motion class are precedents. Both classes are required research.
13. **"Marketing-speak language in dev-tool launches."** — For dev-tool products specifically, superlatives ("revolutionary", "best-in-class", "enterprise-grade", "game-changing", "seamless", "robust") signal "marketer wrote this" to a developer audience and inversely correlate with launch traction. Lead with technical specifics, honest comparisons (including where you lose), and code-first links. See Section 3 motion-class-specific rules for the full dev-tool tonal pattern.
14. **"Pivot the dogfood to match the paying ICP" without also pivoting the target audience.** — When Step 0.5 M0e flags a dogfood/buyer mismatch, the correct fix is BOTH pivots: change the target audience in marketing materials AND expand dogfood subjects to match. Deferring the paying ICP "to v1.0.5" while keeping the dogfood-aligned audience preserves the mismatch — the product still ships calibrated to the wrong audience. See M0e for full prescription.

If the founder leans into any of these patterns, surface it directly, explain why it fails, and require a concrete alternative before proceeding.

**Default refusal posture (under marketing-naive default):** when in doubt between accepting a founder's marketing claim and challenging it, CHALLENGE. The asymmetry is: a wrongly-accepted premise produces a polished plan that ships to silence; a wrongly-challenged premise costs 10 minutes of founder time to re-defend. The cost asymmetry favors challenge.

---

## License + attribution

This skill is designed to be GStack-compatible. Released MIT for free use, modification, and redistribution. Attribution appreciated but not required.

If you use this skill and find it useful (or broken), share your experience. Marketing skill design has weak feedback loops; honest reports matter.

---

## Version history

- v0.1.0 (2026-05-23) — initial release. Built to fill the marketing gap in GStack's planning pipeline as identified by founder using GStack to build [tldrof.com](https://github.com/remakeai/tldr-of-tldrs).
- v0.2.0 (2026-06-01) — Premise audit added (Step 0.5 with M0a-M0e questions) in response to v0.1.0 failing its own regression test against the tldrof fixture (scored 2/7). Three core changes:
  1. Default founder assumption made explicit: technically strong, marketing-naive. PRODUCT description accepted on faith; all MARKETING premises (pricing, ICP, channels, launch platform, dogfood mix, in-scope features) suspect by default.
  2. Step 0.5 Premise Audit inserted BEFORE Step 0A tactical questions. Five new premise-challenge questions (launch-platform audience-class fit, canonical-success comparable, anti-feature surface, freebie-disqualifier, dogfood-vs-buyer audience match). Cascading findings flow into Step 0A questions.
  3. Section 1 now requires CANONICAL-SUCCESS comparables in addition to direct competitors. Section 5 questions launch GATE (calendar vs PMF-signal) before producing the sequence. Section 6 questions pricing BAND before optimizing price point. Anti-patterns list expanded from 6 to 12.
  Regression baseline: v0.2 scored 7/7 on tldrof, b2b-saas, dev-tool fixtures (3 fixtures × 1 run each = 3/3 STRONG PASS).
- v0.3.0 (2026-06-01) — Reliability-sweep findings (3 fixtures × 3 runs = 9 total runs) revealed three failure patterns that headline pass rates hid. All three fixed:
  1. **M0e dogfood-mismatch prescription strengthened.** v0.2 correctly identified dogfood/buyer mismatches but in one tldrof run prescribed the wrong fix (defer the paying ICP, keep the dogfood-aligned audience). M0e "Refuse to accept" now explicitly catches the deferral pattern; "Accept" requires BOTH pivots (target audience + dogfood subjects). Also added as anti-pattern #14.
  2. **Mode A vs Mode C activation criteria tightened.** v0.2's "some audience" was ambiguous — same b2b-saas input got Mode A in two runs and Mode C in one. Activation rules now disambiguate by ICP-alignment (not just count) and add a load-bearing tie-breaker: mid-build with hard launch date prefers Mode A with elevated Section 4 over Mode C alone, because Mode C alone skips the launch playbook the founder still needs.
  3. **Dev-tool motion-class rules added.** v0.2 trended consistently shallow on dev-tool insights 5 (GitHub ecosystem) and 6 (anti-marketing tonal register) across all 3 runs — a skill gap, not noise. Section 3 now has explicit motion-class-specific rules for consumer / B2B / dev-tool, with the dev-tool block elevating docs/SEO + GitHub-as-marketing-surface + founder-existing-dev-audience to PRIMARY channel status and adding a load-bearing tonal rule against marketing-speak in dev-tool launch copy. Also added as anti-pattern #13.
  Regression target for v0.3: 7/7 on all 3 fixtures, with insight 5 and 6 depth on dev-tool fixture improving to ≥1 deep (not consistently moderate as in v0.2). If a smoke-test run shows degradation on previously-passing insights, revert and re-design.
