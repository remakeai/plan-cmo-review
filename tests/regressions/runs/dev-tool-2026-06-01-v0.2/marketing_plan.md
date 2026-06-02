# AuthForge — Marketing Plan (Dev-Tool Fixture, v0.2 Regression Run)

**Date:** 2026-06-01
**Skill version:** plan-cmo-review v0.2
**Mode:** TBD — selected after Step 0B
**Founder default:** Technically strong; first-time at marketing/launching a paid product. Has a real dev-Twitter + blog audience that IS ICP-aligned (override candidate for the marketing-naive default).

---

## PREMISE-LEVEL FINDINGS BLOCK

Step 0.5 results: **3 of 5 premises FAIL, 1 SURVIVES, 1 INCONCLUSIVE.** Premise audit IS load-bearing — the design doc is technically reasonable but commercially generic. Highlights:

- **M0a (launch-platform fit): SURVIVES.** HN + r/programming are correctly the right *audience class* for an open-source backend-engineer SDK. This is the unusual case where "Show HN" is not a category error — HN's median commenter is the target ICP. *But* the depth of plan (single Show HN as the whole strategy) is still the lottery-ticket anti-pattern; the platform is right, the level of investment is wrong.
- **M0b (canonical-success comparable): FAILS.** Design doc has zero named precedents. AuthForge's motion class — OSS-core + hosted tier in dev infra — has 4+ canonical successes (HashiCorp, Supabase, Sentry, Posthog, Cal.com). Each used a specific playbook (community-led growth, docs-as-marketing, conferences/meetups, content compounding). "Show HN + r/programming + tutorials" is from-first-principles thinking that ignores 10 years of precedent. **Cascading impact:** Section 1b mandatory; Section 5 launch sequence must add audience-build months, not days.
- **M0c (anti-feature surface): FAILS.** "Simpler than Auth0, more flexible than Supabase Auth, open-source" is three positionings, not one. "Simpler" implies a curated narrow surface; "more flexible" implies an expansive configuration surface; "open-source" attracts self-hosters who will never convert to the $99/mo hosted tier. These pull in opposite directions on roadmap and on hosted-tier conversion math.
- **M0d (freebie-disqualifier): FAILS.** OSS MIT license is the maximum-free, maximum-self-select-against-paying-segment acquisition mechanic. Self-hosters are technical, time-rich, money-averse — the opposite of the buyer who pays $99/mo for managed infra. The validation cohort (GitHub stars) is structurally different from the paying cohort (teams who don't want to operate auth). Stars are vanity for the hosted-tier conversion goal. **Cascading impact:** the gate metric "100 stars + 5 hosted signups" is a wrong-grain metric — 100 stars is easy and proves nothing; 5 hosted signups in 60 days is the real signal and is much harder.
- **M0e (dogfood audience-class match): INCONCLUSIVE — likely FAIL.** Founder is ex-Stripe (technical, infra-comfortable). Hosted-tier buyer is a small/medium-team backend engineer who is paying $99/mo *to not deal with* what the founder is comfortable building from scratch. There is a real risk that the SDK ergonomics are optimized for "engineer who would prefer to self-host" and the hosted tier ends up under-served.

**Working under marketing-naive default.** Founder has shipped no prior commercial products, has a real and genuinely-relevant dev audience (3K Twitter + 20K-readers blog), and is making first-time-launching-a-paid-product errors. The audience asset overrides the default *partially*: we trust the founder's ability to reach dev attention. We do NOT trust their pricing, gate metric, or conversion assumptions.

---

## Step 0 — Pre-review system audit

### What exists in the design doc
- Distribution model: MIT OSS SDK + hosted tier ($99/mo + $0.001/MAU over 10K)
- Target audience: backend engineers integrating auth
- Distribution plan: "Show HN at launch + post on r/programming + write integration tutorials" (three-line plan)
- First 10 customers: "GitHub stargazers who upgrade" (passive)
- Validation gate: 100 GitHub stars + 5 hosted-tier signups by day 60
- Positioning: "Simpler than Auth0, more flexible than Supabase Auth, open-source"

### Founder audience audit (numeric)
- Twitter/X: ~3,000 followers, dev-tech focused (relevant ICP overlap — high)
- Personal blog: ~20,000 monthly readers (technical content — high ICP overlap)
- Newsletter: not specified
- GitHub stars on prior projects: not specified
- Prior shipped products: zero commercial; ex-Stripe engineer (credibility-adjacent, audience-adjacent)
- **Net audience asset:** moderate and ICP-aligned. Better than 90% of first-time founders. Better than v0.1 tldrof founder by an order of magnitude in relevance. **Mode A is justified.**

### Competitive landscape (cached from web search; expanded in Section 1)
Direct competitors found: Auth0 (Okta-owned, enterprise default, $0.07/MAU), Clerk (premium DX, indie-SaaS default, $0.02/MAU after 10K free), Supabase Auth ($0.00325/MAU after 50K free, bundled with DB), Stytch (10K MAU free, passwordless-led), WorkOS (B2B SSO leader, 1M MAU free on AuthKit).

**Implication:** AuthForge is entering a saturated, well-funded category. The $99/mo hosted tier sits oddly between Clerk's per-MAU pricing (cheaper for small) and Auth0's enterprise model (more capable). Pricing-band question is live (M0c, Section 6).

## Step 0.5 — Premise audit (M0a–M0e)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| 1 | "Show HN at launch" is sufficient distribution | Distribution Plan | Single-channel lottery; HN is right *class* but launch is point-in-time |
| 2 | $99/mo flat hosted tier is correctly priced | Distribution model | Competitor-anchoring; Clerk at $25 + per-MAU is the live benchmark |
| 3 | "GitHub stargazers upgrade to hosted" is a real conversion path | First 10 customers | Star→paid conversion is famously weak; stargazers are evaluators, not buyers |
| 4 | 100 stars + 5 hosted signups in 60 days is a meaningful gate | Validation gate | Stars are easy/vanity; 5 hosted signups in 60 days is the actual hard metric |
| 5 | OSS license + tutorials produces conversion to hosted | Implied throughout | OSS attracts self-hosters who self-select AGAINST paid; M0d failure |
| 6 | "Simpler than Auth0, more flexible than Supabase, open-source" is positioning | Differentiation | Three contradictory positionings; pick one |
| 7 | Audience is "backend engineers" | Target users | Too broad; "backend engineer at 5-25 person team without dedicated security person" is the actual ICP |

### M0a — Launch-platform audience-class fit

**Question:** Is HN + r/programming the right audience class for an OSS backend auth SDK?

**Answer:** **YES — premise SURVIVES.** This is the case where the founder's instinct is correct.

**Evidence:**
- HN is dominated by backend/infra engineers; per the search, Fly.io (dev infra), HashiCorp tools, and most modern OSS dev tools launched and gained durable adoption via HN.
- r/programming is large (~6M subs) and skews backend; tolerates technical SDK posts more than r/webdev does.
- Unlike consumer-habit products (where HN is a category error), an auth SDK is exactly what HN's median commenter evaluates professionally.

**But** — the *level* of plan is wrong. "Show HN as the launch" is a lottery ticket regardless of audience fit. Per the Groove case (105K HN visits → 97 signups → 14 paying), even a successful HN hit converts at ~0.013% to paying. For AuthForge:
- A median Show HN dev-tool launch gets <50 upvotes and dies.
- A top-decile launch (200+ upvotes) drives 5–20K homepage visits.
- Conversion to a $99/mo hosted product from HN traffic is realistically 0.05–0.2%.
- Best-case math: 20K visits × 0.1% = 20 hosted signups. Median-case: 0–2.

**Verdict:** Audience class is right. Tactic depth is wrong. Don't downgrade HN; *upgrade everything else.*

### M0b — Canonical-success comparable

**Question:** Name the most successful OSS-core + hosted-tier dev infra products and what they did that AuthForge's plan does NOT.

**Answer:** **PREMISE FAILS** — design doc names zero precedents. There are at least 6 known successes; ignoring them is from-first-principles thinking.

**Canonical successes for OSS-core + hosted dev infra:**

| Product | Founded | Playbook |
|---|---|---|
| **HashiCorp (Terraform, Vault)** | 2012 | Community-led growth via HUGs (HashiCorp User Groups), HashiConf annual conference, free OSS + enterprise features tiered. Conference + community + slow compound. NOT launch-day. |
| **Sentry** | 2008 | Long OSS journey before commercial; documented integrations for every language/framework; FSL license; sponsorships of dev podcasts/conferences. |
| **Supabase** | 2020 | Build-in-public on Twitter, weekly "Launch Week" events as recurring narrative, generous free tier, Postgres-first positioning. |
| **PostHog** | 2020 | Open core w/ extremely generous free tier (100x more session replays than Sentry); transparent pricing; product-led with content compounding. |
| **Cal.com** | 2021 | Open-source + hosted; community-led; the "Calendly alternative" wedge; meme-driven dev marketing; transparent funding/financials. |
| **Plausible** | 2018 | Bootstrapped, content marketing + values-based positioning (privacy), no free tier (key delta — they refused the freebie trap). |

**Specific deltas vs AuthForge plan:**
1. Every success above invested 6+ months in **content/community before commercial scale** — AuthForge has a Day 0 commercial gate.
2. Every success had a **clear single wedge** (Terraform = infra-as-code; Sentry = error tracking; Plausible = privacy analytics). AuthForge's "simpler AND more flexible AND open" is three wedges.
3. Most ran **recurring narrative moments** (Launch Week, HashiConf) — AuthForge plans a single Show HN.
4. Most had **docs-as-marketing infrastructure** that took weeks to author — AuthForge mentions "integration tutorials" as one line.
5. Plausible specifically **refused** the freebie pattern and ran trial-only; this would be worth considering for AuthForge given M0d.

**Verdict:** Premise FAILS. Section 1b must build this out; launch playbook (Section 5) must adopt at least 2 of the precedent moves.

### M0c — Anti-feature surface

**Question:** Name 2+ features in scope that contradict the positioning, trust model, or business model.

**Anti-features identified:**

1. **"Open-source (MIT)" + "$99/mo hosted tier"** — these are in tension. MIT license means anyone can self-host trivially. The hosted tier's value prop is "you don't want to run this yourself" — but backend engineers are *exactly* the people who can and will run it themselves. The license is anti-feature relative to the hosted tier business model.
2. **"More flexible than Supabase Auth"** — flexibility implies a large configuration surface, which contradicts "Simpler than Auth0." You can be simpler OR more flexible; you cannot be both without a strong opinion that resolves the tension.
3. **"$0.001/MAU above 10K"** — undercuts Clerk ($0.02/MAU) by 20x. Either this is unsustainable (you can't run managed auth profitably at $0.001/MAU once you factor in compliance, on-call, SOC2 audit, etc.) or it signals "commodity / lowest-price-wins" — exactly the wrong signal for a trust-led category like auth. Auth buyers do NOT trust-shop at the bottom of the price band.

**Verdict:** Premise FAILS. The product is trying to be all things; needs a sharper wedge. Recommended resolution surfaced in Section 6.

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does OSS-MIT + free GitHub repo as primary acquisition select for the wrong segment relative to the paying ICP?

**Answer:** **PREMISE FAILS — high confidence.**

**Mapping:**
- Acquisition mechanic: free MIT SDK on GitHub
- Segment attracted: backend engineers who want to evaluate auth code, modify it, self-host. Profile: technical, time-rich (willing to integrate from scratch), money-averse (will avoid $99/mo if they can ship the OSS).
- Paying ICP for $99/mo hosted: team without time/skill to operate auth infra reliably. Profile: time-poor, money-acceptable. Probably less senior or less infra-focused engineer at a small/medium team.

**These are opposite profiles.** The OSS audience self-selects AWAY from the paying audience. This is the structural reason Sentry/HashiCorp/Cal.com all have an *enterprise* tier (where buyers are not the OSS users at all — they're procurement) and a small hosted tier — they don't actually convert OSS users to paid much; they convert *new* users who found them via OSS reputation to paid.

**Specific evidence from search:**
- Free-to-paid in dev tools typically tops out at ~7% (and that's for tools where the free tier is *the same product* — Clerk free tier IS hosted Clerk just at low MAU).
- Stars→deal conversion is "2–6 months from first star to closed deal" (per saashero search result) — this is enterprise sales motion, not self-serve.
- Plausible's choice to *refuse* the freebie pattern is the most-cited counter-example; their thesis is that free tiers attract non-payers and create a noisy support load.

**Cascading impact:**
- M6 (first-10 customers) cannot rely on stargazers converting; must explicitly target small-team backend engineers via a different surface (newsletter, podcast, content).
- Validation gate (100 stars + 5 hosted signups) is wrong; stars are vanity, the 5 signups is the real metric and is probably realistic only with active outreach.
- Pricing strategy must be reconsidered (Section 6) — if conversion from OSS is rare, hosted price should be higher and trust-led, not undercut Clerk.

### M0e — Dogfood audience-class match

**Question:** Is the audience the product was/will-be dogfooded on the same audience that will pay for the hosted tier?

**Answer:** **INCONCLUSIVE, leaning FAIL.**

**Analysis:**
- Founder is ex-Stripe — used to building infra from primitives, comfortable operating production systems. This is the *self-hoster* profile.
- Paying hosted-tier ICP is the *opposite* — engineer who wants to not think about auth infra.
- Risk: SDK ergonomics will be tuned for "developer who wants to understand auth deeply" not "developer who wants auth to be one config block and forget about it." These imply different default exports, different error messages, different docs structure.

**To resolve:** founder needs to interview/dogfood with at least 5 small-team backend engineers (NOT ex-Stripe friends) BEFORE launch and tune defaults to that audience. Currently no evidence this has been done.

**Cascading impact:** M1 (audience reality) requires the corrected ICP — small/medium-team backend engineer at company without dedicated security team — not "backend engineers" broadly and not "engineers like the founder."

## Step 0A — Forcing questions (M1–M7)

Founder's first-pass answers shown in italics; skill pushback in plain text. Step 0.5 findings flow in.

### M1. Audience reality

*Founder: "Backend engineers building auth into their apps. They hang out on HN, r/programming, dev Twitter, maybe r/webdev."*

**Pushback:** "Backend engineers" is a category, not a persona. The actual paying ICP per Step 0.5 is narrower: backend engineer at a 5–25 person team, no dedicated security/identity person, builds in a modern stack (Node/Python/Go), needs auth to work in 30 minutes, will not self-host because they don't want a 3am page. *Specifically* she reads Bytes/JavaScript Weekly/Console.dev, listens to Syntax/Software Engineering Daily, follows @kentcdodds / @theo / @t3dotgg on Twitter, lurks on r/node and Hacker News. Names: "Priya, lead backend at a 12-person Series A health-tech, ships features daily, just got a SOC2 prompt from her first enterprise customer and panicked because auth is brittle."

**Status:** answered after pushback. Founder must validate this persona by interview before launch.

### M2. Discovery path

*Founder: "She'll see my Show HN post, click through, star the repo, set it up."*

**Pushback rejected — "Show HN" cannot be step 1 (rule), and even if it were, conversion from a single touchpoint is near-zero. Realistic 3+ step path:**
1. Priya reads a guest post by founder on a credible backend-engineering newsletter (Bytes / Console / Pragmatic Engineer guest slot) about "we ripped out Auth0 because…"
2. She bookmarks it; two weeks later hits a SOC2-prep moment and Googles "Auth0 alternative open source SOC2."
3. AuthForge ranks (because SEO content was authored deliberately) or she remembers the founder's name from Twitter.
4. She lands on docs, hits Hello World in <10 minutes (per dev-tool benchmark: <10min API call → 3-4x conversion lift), tries OSS for 1 week, hits ops pain, considers hosted.
5. Hosted-tier signup is triggered by an op pain (key rotation, audit log retention, MFA enrollment edge case), NOT by stargazing.

**Status:** answered. Discovery is content-led + recall, not launch-pulse.

### M3. Pre-launch audience

*Founder: "3K Twitter followers (dev focused), blog with ~20K monthly readers."*

**Status:** **REAL audience.** Per skill rules, this is "some audience" — but importantly, it's also *ICP-aligned* (dev/backend). This is the override case where the founder is NOT marketing-naive about audience-building (they did it via the blog); they ARE marketing-naive about pricing, gate metrics, conversion. Mode A is justified (not Mode C); Section 4 audience-build plan focuses on activating the existing audience, not building from zero.

### M4. Channel honesty

*Founder: "My blog. I write technical posts that get traction. I've had two posts hit HN front page in the last year."*

**Status:** strong answer. Blog + dev Twitter is a credible distribution surface. This is the channel to lean into.

### M5. Competitor traffic source

*Founder: "I don't know — I assume Clerk gets it via Twitter and YC visibility, Auth0 via enterprise sales, Supabase via the bundled DB."*

**Pushback:** acceptable hypothesis but founder must verify before next session. Known patterns from search:
- **Clerk:** premium DX as content (blog comparing every auth provider), strong Twitter game from team, sponsorship of dev influencers (Theo, Web Dev Simplified), YC alum network. Bottom-up adoption via free tier.
- **Auth0 (Okta):** enterprise outbound sales + Okta channel; OSS-attracted devs were the v1 motion but not current motion.
- **Supabase Auth:** comes as a default with Supabase DB; ~zero standalone marketing for auth specifically.
- **Stytch:** content-led, esp. on passwordless; sponsorships of backend-eng podcasts.
- **WorkOS:** enterprise SSO content marketing + extensive docs; courted by Y Combinator companies for B2B.

**Pattern:** none of these won via launch-pulse. All used 1–2 year content compound.

**Status:** answered after pushback.

### M6. First 10 paying customers

*Founder: "GitHub stargazers who upgrade to hosted tier."*

**Pushback strong:** Step 0.5 M0d shows stargazers are structurally the wrong cohort. Real path to first 10 paying hosted customers:
1. Founder personally emails 30 small-team backend engineers in their existing Twitter network ("hey, I'm building this, would love 20 min of feedback") — names matter.
2. Of the 30, ~5–10 will engage; 2–3 will be interested in piloting hosted free for 60 days in exchange for testimonial.
3. Paid conversion happens after 60-day pilot when they realize they're depending on it.
4. The other 7–8 paying customers in the first 10 come from: a guest post on a high-quality dev newsletter, a podcast appearance, and one well-targeted Show HN that the founder's network amplifies.
5. **Critical: founder must do concierge onboarding of first 10 hosted customers personally** (Superhuman/Vohra precedent). This means real-time setup help in Slack/Discord/Zoom for each one.

**Status:** answered after total rewrite.

### M7. Time allocation

*Founder: "Maybe 10% on audience-building right now; I'm heads-down on the SDK."*

**Pushback:** wrong ratio. Skill rule is ≥30% pre-launch. For an OSS dev tool launched into a saturated category by a first-time commercial founder, recommend **40–50%** of pre-launch time on content + outreach + concierge calls. The SDK is table stakes; the wedge is trust + reach.

**Status:** acknowledged gap. Founder commits to reallocation in this-week action items.

### Completion criteria — DONE. All 7 answered after pushback.

## Step 0B — Mode selection

**Selected: Mode A — Full Marketing Review.**

**Reasoning:**
- Founder has substantial AND ICP-aligned existing audience (3K dev Twitter + 20K blog readers). This rules out Mode C (Audience-Build Sprint) — audience exists.
- Competitive landscape exists and was web-researched in Step 0. Founder named direct competitors correctly.
- Multiple Step 0.5 premise failures + first-time commercial founder → benefits from full-coverage review, not focused.
- Time budget is not unduly constrained per the design doc.

Mode A runs all 9 sections.

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | Founded | Pricing | Apparent traffic source | User complaints (HN/Reddit signal) | Honest read |
|---|---|---|---|---|---|
| **Auth0 (Okta)** | 2013 | Free 25K MAU; Essentials $35/mo; Enterprise custom. $0.07/MAU at scale. | Enterprise outbound sales; Okta channel; legacy SEO. | "Expensive at scale", "complex pricing", "Okta acquisition hurt DX." | Winning at enterprise; losing indie/SMB mindshare. |
| **Clerk** | 2020 | Free 10K MAU; Pro $25/mo + $0.02/MAU. | Premium-DX content blog, dev Twitter team presence, sponsorships of Theo/WDS, YC alumni network. | "Vendor lock-in", "pricing creeps", "UI components opinionated." | Winning the indie-SaaS/Next.js segment. |
| **Supabase Auth** | 2020 | Bundled w/ DB; $0.00325/MAU after 50K free. | Build-in-public on Twitter, Launch Weeks, Postgres-fan crossover. | "Couples auth to DB choice", "less polished than Clerk for pure auth." | Winning the "I already use Supabase" segment. |
| **Stytch** | 2020 | 10K MAU free; passwordless-led pay-per-MAU. | Content marketing on passwordless; podcast sponsorships. | "Niche-feeling", "fewer prebuilt UIs." | Modest win in passwordless vertical. |
| **WorkOS** | 2019 | AuthKit 1M MAU free; SSO per-connection. | B2B SSO content + extensive docs; YC company default for "enterprise-readiness". | "Built for the B2B-enterprise step, not for early auth." | Winning the "we just landed our first enterprise customer" segment. |

**The shape of the market:** Auth0 owns enterprise procurement. Clerk owns indie polish. Supabase owns "I'm already there." WorkOS owns "we need SSO for our first enterprise." Stytch owns passwordless. Where does AuthForge fit? The design doc's answer ("simpler + more flexible + OSS") is vague. **Recommended re-positioning surfaced in Section 6.**

### 1b. Canonical-success comparables (motion class: OSS-core + hosted, dev infra)

| Product | Founded | Scale | Primary acquisition channel | Onboarding model | Launch gate | Delta vs AuthForge plan |
|---|---|---|---|---|---|---|
| **HashiCorp (Terraform)** | 2012 | $5B+ valuation pre-IBM, IPO'd | Community-led: HashiCorp User Groups (HUGs), HashiConf, blog/docs compound. Slow burn 4+ years before commercial scale. | Self-serve OSS; enterprise touch sales for paid. | Adoption-curve (waited for OSS critical mass before commercial push). | AuthForge has no community plan, no conference, no patience. |
| **Sentry** | 2008 | ~$200M ARR, FSL-licensed | Documentation compound; integration-per-framework strategy; dev conference sponsorships; podcast. | Self-serve hosted; SaaS-first revenue. | Slow compound over decade. | AuthForge has no integration matrix plan, no docs-as-marketing plan. |
| **Supabase** | 2020 | Last raise ~$2B valuation | Launch Week as recurring narrative moment; build-in-public on Twitter from founder + team; Postgres community crossover. | Self-serve hosted, generous free tier. | Launch Week cadence (every quarter). | AuthForge plans 1 launch event, not recurring. |
| **PostHog** | 2020 | ~$50M+ ARR | Open core + extremely generous free tier (key — 100x competitor); transparent pricing as marketing; product-led growth. | Self-serve hosted + self-host option. | Continuous, no single launch. | AuthForge has a Day-60 calendar gate. |
| **Cal.com** | 2021 | $30M+ raised | Meme-driven dev marketing, transparent finances, the "Calendly alternative" wedge, community contributor model. | Self-serve hosted + self-host. | Community-momentum gated. | AuthForge has no clear wedge to anchor the meme. |
| **Plausible** | 2018 | ~$2M ARR bootstrapped | Content marketing + values-positioning (privacy); **refused free tier entirely** (counter-pattern). | Self-serve trial → paid. | Bootstrapped — gated by org capacity, not calendar. | AuthForge could learn from Plausible's refusal of freebie. |

### 1c. Pattern surface

**What canonical successes have in common that AuthForge's plan lacks:**
1. **Slow compound (6 months–4 years) before scaled commercial revenue.** AuthForge's 60-day gate ignores this.
2. **A clear, narrow wedge** (infra-as-code, error tracking, Postgres-bundled, privacy, etc.). AuthForge has three wedges that contradict.
3. **A recurring narrative moment** (HashiConf, Launch Week, conference circuit) — sustains attention vs single launch.
4. **Docs/integrations as primary marketing surface** — not "tutorials" mentioned offhand.
5. **Community-led growth investment** — HUGs, Discord, contributor docs, public roadmap.

**Where direct competitors diverge from canonical patterns:**
- Clerk and Auth0 are *not* OSS-core; they're closed-source SaaS. So they're not the right precedent for AuthForge's OSS-core motion. The right precedents are HashiCorp/Sentry/Supabase/PostHog/Cal.com — none of which AuthForge's plan references.

**Current plan is implicitly following the SaaS launch-day playbook (Show HN + viral) — wrong precedent class.** It should follow the OSS-core slow-compound playbook (community + content + recurring narrative moments + concierge-onboarded paid tier).

**Founder action:** read founder interviews of Mitchell Hashimoto (HashiCorp), Paul Copplestone (Supabase), James Hawkins (PostHog), and the Cal.com OSS post. Record specific patterns to import.

## Section 2 — ICP specification

### Persona: "Priya, lead backend at a 5–25 person Series A team"

**Five+ specific attributes:**
1. 4–8 years backend experience, comfortable in Node/Python/Go, has shipped a half-dozen production services.
2. **No dedicated security/identity engineer on the team** — auth is "her job by default."
3. Just got a SOC2 (or HIPAA-prep) ask from a first enterprise prospect; auth audit gap is now urgent.
4. Currently using Auth0 (annoyed at cost), Supabase Auth (annoyed at coupling), or rolling her own (annoyed at maintenance) — has at least one painful auth-related incident in the last 6 months.
5. Time-poor — does not want to evaluate 5 auth tools; wants an opinionated recommendation from a source she trusts.
6. Reads on commute; pays for ChatGPT Plus, GitHub Copilot, sometimes Linear personally.

**Where she spends attention (≥5):**
- Newsletters: Bytes, JavaScript Weekly, Console.dev, Pragmatic Engineer
- Podcasts: Syntax, Software Engineering Daily, Changelog
- Twitter: @kentcdodds, @theo, @t3dotgg, @rauchg, @adamwathan
- Communities: r/node, Hacker News (lurker, not commenter), the Reactiflux Discord, sometimes Indie Hackers
- Conferences: doesn't go to many, but watches recorded talks from React Conf and similar

**What she currently pays for in adjacent categories:**
- GitHub team plan, Vercel/Render, Linear, Sentry, sometimes Posthog, Datadog at work
- Anchor pricing for "infra I trust": $20–$100/mo per seat is normal; $100–$500/mo per workspace for shared services

**What she complains about in those tools:**
- "Pricing creeps unpredictably" (Auth0, Datadog complaint)
- "Setup is more painful than the docs imply" (most tools)
- "Vendor lock-in is real" (Auth0 export pain)
- "Support is non-existent below enterprise tier" (every SaaS)

**Specific objections she will raise to AuthForge:**
1. "OSS-core means I bet on a 1-person project — what's your runway? what happens if you stop?"
2. "Why would I pay $99/mo when Clerk's free tier covers my MAU?"
3. "How do I migrate off Auth0 — what's the data-export story?"
4. "SOC2-readiness? Audit logs? MFA?"
5. "Is this opinionated or configurable? I need an answer."

**Specific reasons she will convert (from OSS user → paid hosted):**
- Has been using OSS in production for 30+ days and hit her first ops pain (key rotation, audit-log retention, SLA).
- Just landed an enterprise customer who's asking for audit reports she can't easily generate.
- Founder personally onboarded her and she trusts the team.
- Hosted tier removes a 3am-page risk she now owns.

**Output:** see `icp.md` for the standalone version.

## Section 3 — Distribution channel-by-channel

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Verdict |
|---|---|---|---|---|---|---|
| **Founder's blog (20K monthly readers)** | High & ICP-aligned | Time only | High (qualified) | **Excellent — existing asset** | Med (need to write deliberate auth content) | **TIER 1 — primary channel** |
| **Founder's Twitter (3K dev followers)** | Medium & ICP-aligned | Time only | Med | **Excellent — existing** | Low (consistent posting) | **TIER 1** |
| **Show HN at launch** | High lottery | Free | Low (~0.05–0.2% to paid) | Strong (ex-Stripe credibility helps comments) | Low to post / High to prep | **TIER 2 — single moment, not strategy** |
| **r/programming + r/node** | Medium | Free | Low; mod risk | Medium | Low | **TIER 2 — cross-post only, not primary** |
| **Guest posts on Bytes / Console / JS Weekly** | High & ICP-aligned | Time | High | Strong (writing track record) | High (pitch + write) | **TIER 1 — high leverage** |
| **Podcast guesting (Syntax, Changelog, SEDaily)** | Medium-high & ICP-aligned | Time | High | Strong (ex-Stripe story) | Med (pitch effort) | **TIER 1** |
| **Sponsorship of dev influencer content** | High & ICP-aligned | Cash ($1–10K/spot) | Med-high | N/A | Low (just $) | **TIER 2 — once revenue justifies** |
| **SEO content (comparison posts, "Auth0 alternative")** | Compound | Time | High over time | Strong (writer) | High (months) | **TIER 1 — long compound, start now** |
| **Product Hunt** | Medium | Time | Low for dev infra | Med | Med | **TIER 3 — optional, low priority** |
| **Indie Hackers** | Low for paid hosted tier | Free | Low | Med | Low | **TIER 3** |
| **LinkedIn organic** | Low for dev tools | Free | Low | Weak | Low | **CUT** |
| **Cold email outreach to small-team CTOs** | Medium | Time | Med (with personal connection) | Strong (network) | High | **TIER 2 — for first 10 paying** |
| **Conferences / meetups** | Medium-high | Cash + Travel | High in person | Med | High | **TIER 3 — year 2** |
| **Paid ads (Google, Twitter)** | Medium | $$$ | Low for dev | N/A | Med | **CUT — not yet** |
| **Affiliate program** | Low pre-traction | Time | Low | Weak | Med | **CUT — premature** |
| **Discord community of own** | Low at start | Time | Med (trust building) | Strong | Med | **TIER 2 — build alongside first 10 customers** |

**Top 3 channels (focus here):**
1. **Founder's blog + Twitter (existing audience activation)** — write 2 high-quality auth-focused pieces, surface them to existing audience, ride to broader pickup.
2. **Guest posts on Bytes/Console/JS Weekly + podcast guesting** — multiply reach into adjacent-but-larger audiences using founder's writing chops + ex-Stripe story.
3. **Concierge outreach to ~30 named small-team CTOs/lead engineers** — the only realistic path to first 10 paying hosted customers.

**Demoted:** Show HN (still useful, but as a moment within a larger sequence, not as the strategy).

**Cut:** LinkedIn, paid ads, affiliate, conferences (all premature).

## Section 4 — Pre-launch audience-building plan

Founder already has audience; this is *activation + extension* not cold start.

### Day 1–30
- **2 long-form blog posts/month** on auth-adjacent topics: (a) "Why I left Stripe to fix open-source auth", (b) "What I learned auditing 12 startup auth implementations." Posts must be SEO-aware (target queries like "Auth0 alternative open source", "Clerk vs Supabase Auth", "SOC2 auth checklist").
- **Twitter cadence:** 3 posts/week — build-in-public progress, ex-Stripe nuggets, hot takes on auth news. 1 thread/week.
- **Newsletter setup:** start an email list TODAY (founder doesn't yet); landing page that captures email with "AuthForge launch + auth deep-dives" promise.
- **Concierge outreach:** identify and personally email 30 small-team backend leads in network/extended network. Ask for feedback, not sale.
- **Podcast pitching:** pitch 5 podcasts (Syntax, Changelog, SEDaily, Backend Banter, JS Party). Need 3+ hits in next 90 days.

### Day 31–60
- **Continue blog cadence (2/month).** Layer in: comparison pieces ("AuthForge vs Auth0", "AuthForge vs Clerk", "Why we're refusing the freebie pattern" — Plausible-style values content).
- **Twitter:** sustain 3/week + 1 thread; start commenting on auth-related threads from competitors (Clerk team, Supabase team) to insert presence.
- **Newsletter:** weekly email — should have 200–500 subs by day 60 if blog promotion is consistent.
- **Concierge:** of 30 outreach, 5–10 will have engaged. Convert 3 to "design partner" pilot — free hosted tier in exchange for product feedback + future testimonial.
- **Recorded podcast episodes drop:** amplify each on Twitter + blog.

### Day 61–90 (overlaps launch)
- **Launch sequence kicks off** (see Section 5 / `launch_playbook.md`). Audience-build does NOT stop — it intensifies.
- **Launch content:** 1 deep-dive technical blog timed with launch, 1 retrospective post 30 days after.
- **Newsletter:** dedicated launch email to subscribers (warmest cohort).
- **Twitter:** launch thread, daily updates for first week, founder reachability for questions.

### Specific weekly commitments (founder must commit)
- 2 hours: blog writing
- 1.5 hours: Twitter
- 2 hours: concierge outreach + interviews
- 1 hour: podcast prep / pitching
- 0.5 hours: newsletter
- **Total: ~7 hours/week minimum on audience-build. This must be ≥40% of pre-launch time.**

Tracked weekly in `audience_build_journal.md` (template artifact).

## Section 5 — Launch playbook (summary; full sequenced version in `launch_playbook.md`)

### 5a. Launch gate — calendar vs PMF-signal

**Design doc gate:** "100 GitHub stars + 5 hosted-tier signups by day 60." This is *partially* PMF-signal-shaped (the 5 hosted signups are real). But:

- **100 stars is a vanity gate** — easy to reach via the founder's existing audience and effectively meaningless as a paid signal (M0d).
- **5 hosted signups in 60 days is a *real* gate** but the path to it is not specified.
- The gate is also calendar-mixed (60 days).

**Recommended adjustment:** drop the star count. Replace with:
- **Adoption gate:** 3 of 5 design-partner pilots report dependence (use ≥3x/week for 4 consecutive weeks) — a Vohra-style "very disappointed" test adapted for SDK dev tools.
- **Conversion gate:** at least 2 of 5 design partners convert to paid hosted after 60-day pilot.

If either fails, do NOT do the broad Show HN launch. Iterate the product or the wedge first. This is the concierge-first cohort pattern from Superhuman/Readwise.

### 5b. Default sequence (customized — see `launch_playbook.md` for hour-by-hour)

The default sequence in the skill template is roughly correct for dev tools, with these AuthForge-specific customizations:

- **Day -90 to -30:** content + concierge sprint (see Section 4)
- **Day -30:** soft-pre-announce to newsletter subscribers
- **Day -14:** publish "the why" essay on founder blog (this is the post that gets HN traction independently)
- **Day -7:** email to ~50 personal network ("launching next week, here's the pitch, would mean a lot if you shared")
- **Day -3:** build-in-public Twitter thread previewing launch (founder has the followers to make this real)
- **Day 0 morning Pacific:** Show HN post — title formula: "Show HN: AuthForge – Open-source auth without the Auth0 bill"
- **Day 0 +2hr:** Twitter launch thread cross-linking HN
- **Day 0 +4hr:** post in r/programming + r/node (separately, with community-appropriate framing — NOT a copy of the HN post)
- **Day 0 +24hr:** newsletter blast to mailing list
- **Day 0 +48hr:** podcast guest spots starting to drop (pitched weeks ago)
- **Day 0 +7d:** Product Hunt launch (separate event)
- **Day 0 +30d:** retrospective post with real numbers ("we launched, here's what happened") — this post often outperforms the launch itself for trust-building

### Risk callouts
- **HN miss = soft outcome, not catastrophic.** Existing audience absorbs even if HN flops. This is the asymmetry the founder should bank.
- **Wrong wedge in the Show HN title = self-inflicted dud.** "Yet another auth library" gets buried; "Auth0 alternative without the bill" gets clicked.
- **r/programming mod ban = real risk** — must post as participant not as marketer. Read sub rules.

## Section 6 — Pricing & packaging

### 6a. Pricing-band question

**Design doc:** $99/mo flat + $0.001/MAU above 10K.

**Where does this band come from?** Almost certainly competitor-anchored (between Clerk's free tier and Auth0's enterprise) and not from ICP willingness-to-pay evidence. There is no evidence in the design doc that the ICP has been asked what they would pay.

**ICP-WTP evidence we can assemble:**
- Priya pays Sentry ~$30–80/mo for error tracking. Datadog ~$200+/mo. Linear $10/seat. Sentry team plan around $100/mo for a small team.
- Per RevenueCat-style benchmark data: $5–9 is the documented LTV-penalty band; tools at $10–30/mo retain meaningfully better; tools that price to a *workspace* (not per-seat) often land $50–200/mo for small teams.
- For trust-led infra categories (auth, payments, monitoring), buyers do NOT price-shop at the bottom. They trust-shop near the top. Cheapening signals commodity.

**Pricing critique:**
1. **$99/mo flat** is in a reasonable band, but the $0.001/MAU overage is **suspiciously cheap** — undercutting Clerk by 20x signals "commodity" to a trust-led category and creates margin-impossible economics.
2. **The flat $99 + cheap overage** means the worst-case customer (huge MAU, low ARR per MAU) is the most expensive to serve. Reverse selection.
3. **No annual option mentioned** — annual billing typically increases retention 2x+. Missing.
4. **No enterprise tier** — for an auth product, "enterprise" (custom SLA, SOC2 audit report, audit log retention, MFA enforcement, SAML) is where margin lives. Missing the entire upside.

### 6b. Standard packaging recommendation

**Proposed tier structure:**

| Tier | Price | Target | Includes |
|---|---|---|---|
| **OSS / Self-host** | Free (MIT) | Self-hoster, learner, evaluator | Full SDK; community support |
| **Hosted Starter** | $49/mo or $490/yr (16% off annual) | Solo dev, prototype, side project | 10K MAU, basic audit logs (30d), email support |
| **Hosted Team** | $199/mo or $1,990/yr | Series A team (Priya) | 50K MAU, audit logs (1yr), priority support, MFA, basic SSO (Google/GitHub) |
| **Hosted Business** | $799/mo or $7,990/yr | Late-stage team needing SOC2/HIPAA | 250K MAU, SAML SSO, SCIM, audit-log retention (3yr), uptime SLA, named support |
| **Enterprise** | Custom (starts ~$24K/yr) | Procurement-driven buyer | Custom MSA, on-prem option, dedicated support, security review |
| **MAU overage** | $0.01/MAU (10x current spec) | All paid tiers | — |

**Rationale:**
- $0.01/MAU is the floor — matches Clerk's $0.02 directionally. $0.001 was self-sabotaging.
- Annual discount mandatory for retention.
- Team tier is **the ICP tier** ($199/mo) — anchored to "Priya can expense this without approval."
- Business tier captures SOC2/SSO upside.
- Enterprise tier ensures there's a path to $100K+ ARR per customer.

### 6c. Trial mechanic (revisit M0d freebie-disqualifier)

**Recommendation:** *avoid free hosted trial* for the Team tier (M0d failure mode). Instead:
- OSS is the "free" — anyone can self-host indefinitely.
- Hosted: **14-day money-back guarantee** (not free trial). Card required up-front.
- For first 10 paying customers: founder-personal concierge onboarding instead of self-serve trial. Vohra/Superhuman pattern.

This refuses the freebie pattern (Plausible precedent) for the paid tier specifically, while still allowing OSS to do its top-of-funnel work.

**Force the founder to defend:** if they want to keep the original $99/mo flat single tier, they must explain (a) how it serves both a 12-person Series A and a 200-person enterprise, (b) why the $0.001 overage isn't margin-destroying, (c) why there's no annual discount.

## Section 7 — Post-launch growth loops

| Loop | Compounds? | AuthForge specifics |
|---|---|---|
| **Referral mechanics (in-product invite)** | Linear at small scale | Auth product → team invites are natural; add "Powered by AuthForge" badge on hosted login pages (small founder credit) — opt-out, not opt-in. |
| **Content compounding (SEO)** | Strong compound (6–18mo) | Comparison posts ("AuthForge vs X"), tutorial library per framework, "auth checklist" type posts. Long ramp. |
| **Integration matrix (Sentry-style)** | Compound — every new integration = new SEO surface + new referrer | Build first-party integrations: Next.js, Remix, SvelteKit, Astro, Hono, NestJS, FastAPI, Django, Rails. Each one is a docs page + a blog post. |
| **Network effects** | None inherent | Auth is single-tenant — no network effects in the product itself. Acknowledge. |
| **Brand compounding** | Strong if consistent | Founder voice + consistent values (open-source, no-creep pricing) is the brand. Compound over 2–3 years. |
| **Retention → word-of-mouth** | Strong for dev tools | Devs talk to other devs. Best growth loop available. Concierge onboarding amplifies. |
| **Open-source contributors** | Compound for dev presence | Contributor docs, "good first issue" labels, recognition for community PRs. HashiCorp HUG-style. |

**Honest read:** AuthForge has 4 strong loops (content, integration matrix, brand, WoM). No network effect — that's fine for dev infra; not the right loop class. Acquisition-treadmill risk is *low* if content + integrations compound, but they require sustained investment.

## Section 8 — Metrics & instrumentation

### Track weekly

| Metric | Why | Source |
|---|---|---|
| Hosted-tier paying customers | The only true revenue signal | Stripe / billing |
| MRR + ARR | Revenue growth | Stripe |
| Hosted free trial → paid conversion | Funnel health | Internal analytics |
| Time-to-Hello-World (P50, P90) | DX quality leading indicator (10min threshold = 3-4x conversion lift) | Instrumented in SDK / docs |
| Active OSS users (estimated via opt-in telemetry or download counts) | Top of funnel | Telemetry (with consent) |
| Channel attribution (UTM) for paid signups | Where money comes from | UTM + Stripe |
| Newsletter growth | Owned-audience asset | Newsletter platform |
| Docs page views (with-vs-without conversion) | Docs as marketing | GA / Plausible |

### Track monthly
- LTV / CAC by channel (once enough data)
- Cohort retention (M1, M3, M6) for paid tiers
- Concierge onboarding outcomes (signup → 30d retention)

### Vanity — do NOT optimize against
- GitHub stars (decoupled from paid conversion per M0d)
- HN upvotes
- Twitter follower count
- Total signups (without retention context)

### Dashboards
- Weekly: revenue + funnel + DX
- Monthly: cohort + LTV/CAC
- Quarterly: channel mix shift

## Section 9 — Risk analysis

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| **Show HN flops** | Medium-high (single launch is lottery) | Low — existing audience absorbs | Don't bet everything on it; sequence around it. |
| **Wedge confusion ("simpler AND more flexible") prevents word-of-mouth** | High | Medium — slows compound | Force a one-sentence positioning before launch. Section 6 / Section 1c. |
| **OSS users don't convert to hosted (M0d)** | Very high | High — kills business model | Concierge first 10; build paid funnel separate from OSS funnel; consider Plausible-style trial-only. |
| **Pricing mispriced ($99 + $0.001 overage)** | High | High | Adopt tier structure in 6b. |
| **Auth0/Clerk launch competing OSS** | Low-medium | High | First-mover on values positioning (transparent, no-creep pricing) — make the price predictability part of the wedge. |
| **Channel concentration (>60% from blog/Twitter)** | High | Medium | Diversify into podcast + newsletter + SEO compound by month 6. |
| **Founder burnout (40% audience-build + 60% build)** | Medium | High | Pace; consider 1 part-time contractor for content distribution by month 3. |
| **SOC2 audit cost blocks Business tier** | Medium | Medium | Plan SOC2 Type 1 audit by month 6 ($15–30K typical); price Business tier to cover. |
| **Trust risk — "1 person, no funding" objection** | High initially | Medium | Public roadmap + transparent revenue ("$ARR live" page) + accept investment if needed to convert trust. |
| **Algorithm/platform risk (Twitter shifts)** | Medium | Medium | Newsletter (owned audience) priority. |

---

## Outside voice — independent marketing critique

Simulated outside critique (would be run via codex or sibling Claude in real use):

1. **Biggest risk inside review may have missed:** the founder is solving an *auth* problem in a market where buyers are deeply risk-averse about auth specifically. Trust is built over years, not months. A 1-person OSS project asking for $99/mo to host critical-path auth is a fundamentally hard sell *regardless of distribution.* Outside voice would push: have you considered being open-source-only for 12 months to build trust, with no hosted tier? Charge for support/migration consulting instead. Defer hosted to month 12+ when there's brand equity.

2. **Weaker-than-positioned channel:** "Founder's 20K-monthly-readers blog" is real, but the *conversion* assumption from blog reader → AuthForge user is unverified. A backend-eng blog readership may not include the actual "team lead with no security person" ICP. Founder should audit blog analytics for what posts the audience engages with — if it's mostly career/process content, that audience is not the auth-buyer ICP.

3. **Audience claim lacking evidence:** "3K Twitter followers" — is the engagement rate real? 3K low-engagement followers from years ago is different from 3K active followers. Check: median like count on dev-content tweets. If <50, the audience is dormant.

4. **Provocative reframe the founder might not have considered:** **Don't compete in auth. Compete in "SOC2-readiness as a service" for early-stage teams.** Auth is one piece. The Priya persona's *real* pain is the SOC2 audit ask, not auth specifically. AuthForge could be positioned as "SOC2-ready auth + audit-log + access management for Series A teams" — a much narrower wedge with much higher willingness to pay ($500–2000/mo, not $99). This is the "narrow wedge" canonical successes used (Plausible = privacy analytics, not "analytics"; Cal = Calendly alternative, not "scheduling"; Linear = design-led for engineering teams, not "project management"). The current wedge is too broad.

**Recommended discussion with founder:** the reframe in #4 is the biggest potential pivot. Worth a 30-min conversation before locking the plan.

---

## This-week action items (founder commits)

Force pick THREE to commit to THIS week:

1. **Rewrite positioning to a single sentence.** "AuthForge is open-source auth for [specific ICP] that [specific value]." Currently three positionings; pick one. Section 1c + 6b.
2. **Audit blog analytics + Twitter engagement** to verify the audience asset is real and ICP-aligned (outside-voice #2 + #3). Spend 1 hour, document findings.
3. **Email 10 named small-team backend leads** (from network) this week asking for 20-min auth-pain interviews. Use the ICP doc as the screen. This is the start of the concierge path to first 10 customers.

Stretch (if time):
4. Set up landing page + newsletter capture (currently zero).
5. Draft outline for "Why I left Stripe to fix open-source auth" blog post.

---

## Schedule self-check
Re-run `/plan-cmo-review` in 30 days. Specifically:
- Were the 10 interviews done? What did they say?
- Has the positioning been narrowed?
- Has the pricing-tier structure been adopted or defended?
- Newsletter subs at day 30?

## Follow-up skills
- `/office-hours` — if outside-voice reframe (#4) is taken seriously, the positioning has shifted enough to warrant re-running office-hours.
- `/plan-ceo-review` — pricing changes in Section 6 are business-model changes; CEO review will pressure-test the tier structure.
- `/plan-eng-review` — referral mechanics + telemetry + audit-log infrastructure are product implications of this marketing plan.

---

## Version note
Generated by `plan-cmo-review` v0.2. Premise audit (Step 0.5) was the highest-value step under the marketing-naive default; 3 of 5 premises failed and shaped Sections 1, 5, and 6 substantially. Score target: ≥5/7 on regression rubric.
