# AuthForge Marketing Plan — CMO Review v0.2 (Run 3)

**Date:** 2026-06-01
**Skill:** plan-cmo-review v0.2
**Founder profile:** ex-Stripe engineer, ~3K Twitter followers, technical blog ~20K monthly readers, no prior shipped products
**Product:** AuthForge — open-source auth/identity SDK (MIT) + hosted tier ($99/mo + $0.001/MAU above 10K)

---

## Working notes
This file is written progressively as the review runs. Sections appear filled as work completes.

## TABLE OF CONTENTS
- Step 0 — Pre-review system audit
- Step 0.5 — PREMISE AUDIT (M0a–M0e)
- Step 0A — Forcing questions (M1–M7)
- Step 0B — Mode selection
- Section 1 — Competitive landscape
- Section 2 — ICP specification
- Section 3 — Distribution channel-by-channel
- Section 4 — Pre-launch audience-building plan
- Section 5 — Launch playbook
- Section 6 — Pricing & packaging
- Section 7 — Post-launch growth loops
- Section 8 — Metrics & instrumentation
- Section 9 — Risk analysis
- Outside voice critique
- This-week action items

---

## Step 0 — Pre-review system audit

### Marketing-naive default check
Founder is **ex-Stripe engineer**. Stripe is the canonical developer-first infrastructure success — exposure to Stripe's DX patterns, docs-as-marketing, developer-relations playbook. **This is real evidence-of-marketing-context, not just an engineering credential.** That said, the founder has zero prior shipped products and zero prior launches, so the actual marketing *operational* track record is unproven.

**Verdict:** marketing-naive default partially flips. Founder gets credit for:
- ICP-aligned existing audience (3K dev-Twitter + 20K monthly blog readers = both backend-engineer-adjacent)
- Exposure to a canonical-success developer-first playbook (Stripe internal)

But marketing-naive default still applies to:
- Pricing strategy (no prior product to anchor against)
- Launch sequencing (no prior launch experience)
- Conversion mechanics (Stripe scale ≠ solo OSS scale)

Premise audit (Step 0.5) is still load-bearing — just less aggressive than pure naive default.

### Existing audience inventory (load-bearing)
| Surface | Size | ICP relevance |
|---|---|---|
| Twitter/X | ~3,000 followers (dev-Twitter) | HIGH — backend engineers in feed |
| Technical blog | ~20,000 monthly readers | HIGH — same ICP, deeper trust signal than Twitter |
| GitHub stars on prior projects | Unknown — needs founder to surface | TBD |
| Newsletter | None stated | N/A |
| Discord/Slack presence | None stated | N/A |

**Read:** 20K monthly blog readers is a SIGNIFICANT distribution surface for a solo dev-tool launch. Most solo dev-tool founders launch with <1K total reach. This founder is in the top decile of pre-launch audience for solo OSS. Plan must EXPLOIT this, not bury it under "Show HN" thinking.

### Competitive landscape (researched in Step 0 web searches)
Top direct competitors identified: **Auth0, Clerk, Supabase Auth, Stytch, WorkOS, Better Auth, Kinde, MojoAuth.** Pricing data captured for Section 1.

Canonical OSS-to-paid successes researched: **HashiCorp, Sentry, Supabase, PostHog, Cal.com, Plausible.** Sentry explicitly cited as Supabase's reference playbook. PostHog: 97% word-of-mouth growth, open-source as wedge to first 1K users.

### Step 0 activation rule outcome
Substantial prior audience + competitive analysis exists → **Mode A — Full Review** is the right starting frame. Confirm in Step 0B.

---

## Step 0.5 — PREMISE AUDIT (load-bearing)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong-because hypothesis |
|---|---|---|---|
| P1 | Show HN + r/programming as primary launch channels | Distribution Plan | r/programming is a HIGH self-promo-bans risk; Show HN dev-tool fit is correct but oversold as PRIMARY |
| P2 | "GitHub stargazers who upgrade to hosted tier" = first 10 customers | First 10 customers | GitHub stars → paid conversion is 0.5–3% industry benchmark; expecting 10 paid from stars implies needing ~500–2K stars first |
| P3 | Validation gate: 100 stars + 5 hosted signups by day 60 | Validation gate | Calendar-driven, low-bar gate; says nothing about retention/dependence; classic vanity-metric gate |
| P4 | "Simpler than Auth0, more flexible than Supabase Auth, open-source unlike both" | Differentiation | Supabase Auth IS open-source (self-hostable); founder claim is factually wrong; Clerk (the real growth threat for indie devs) isn't even mentioned |
| P5 | $99/mo hosted + $0.001/MAU above 10K | Distribution model | Pricing inherited from "competitor band" thinking; vs Clerk $25 base + $0.02/MAU and Supabase $0.00325/MAU, this is a confused band — too cheap for enterprise, too expensive for indies |
| P6 | "Show HN + post on r/programming + write integration tutorials" is the plan | Distribution Plan | Three channels listed but no sequence, no audience-first ordering, ignores founder's actual leverage (20K blog readers) |
| P7 | "Backend engineers building auth into their apps" as ICP | Target users | Too broad. Backend engineers at YC startups ≠ backend engineers at Fortune 500 ≠ solo indie hackers. These three buy auth completely differently. |

### M0a — Launch-platform audience-class fit

**Question:** Is HN + r/programming the right audience class for AuthForge?

**Web-search-supported analysis:**
- Show HN is documented as STRONG for dev tools. Fly.io is the canonical top Show HN dev-tool launch. (markepear.dev, dev.to launch guides confirm)
- Authentication is squarely a backend-engineer concern. HN's audience is ~70% technical, heavily backend-tilted. Audience class match is GOOD.
- r/programming is more fraught: heavy self-promo policing, frequent bans for product posts; cross-posts often get auto-removed. The CHANNEL fit is right, the EXECUTION risk is high.

**Verdict: PREMISE SURVIVES (with nuance).** HN is the right audience class for AuthForge — this is NOT the tldrof pattern (consumer subscription on HN = category error). HN dev-tool launches have strong precedent. The premise is correct.

**Nuance:** "Show HN as the entire plan" is still wrong, but for different reasons than tldrof:
- HN lottery odds still apply (most Show HNs get <20 upvotes)
- r/programming auto-removal risk is real
- Single-shot HN ignores the founder's 20K blog readers — which is a BIGGER and HIGHER-TRUST surface than HN front page traffic
- The actual issue is OVER-INDEXING on HN as primary when founder's blog should be primary

**Cascading implication:** M2 (discovery path) should NOT refuse "Show HN as step 1" outright — it should refuse "Show HN as the WHOLE plan" and push toward sequencing where founder's blog/Twitter pre-warms the launch.

### M0b — Canonical-success comparable

**Question:** What canonical-success products prove the open-source dev-tool playbook? What did they do that this plan doesn't?

**Web-search findings:**
- **Sentry** — explicit playbook reference for Supabase. OSS-first, monetize via hosted + enterprise SSO. Sold $3B+ category.
- **HashiCorp** — OSS infra (Terraform, Vault) → enterprise. Conversion rate "on the lower end" of 0.5-3% per OSS SaaS benchmark.
- **Supabase** — OSS-first, hosted tier; Auth specifically: 50K MAU free, $0.00325/MAU after. Generous free tier as adoption wedge.
- **PostHog** — 190K+ customers, 97% word-of-mouth growth, **6 pivots in 9 months** before PMF, OSS as wedge to first 1K users.
- **Clerk** — NOT open source but is the indie-dev darling. $25 base + $0.02/MAU. Won via DX + React UI components, not OSS.
- **Cal.com** — OSS scheduling. Strong founder presence on Twitter (Peer Richelsen ships in public daily).
- **Plausible** — OSS analytics. Slow-compound content marketing + Twitter founder presence.

**Pattern these have in common that AuthForge plan LACKS:**
1. **Founder ships in public DAILY** — Cal.com, PostHog, Plausible founders are constant public voice. AuthForge plan has no founder-content cadence.
2. **OSS first, hosted as convenience tier** — AuthForge has this structurally but pricing is misaligned (see P5/M0d).
3. **Documentation-as-marketing** — Sentry, Supabase, Stripe (founder's alma mater!) all treat docs as primary acquisition surface. Plan mentions "integration tutorials" but doesn't elevate this to primary channel.
4. **Community presence** — Discord/Slack/community-first feedback loops. PostHog explicitly credits open source for community-led growth. AuthForge plan = zero community surface.
5. **OSS to paid conversion is 0.5-3%** — AuthForge needs ~167-1000 hosted-tier-relevant OSS users to get 5 paid signups by day 60. Plan doesn't acknowledge this funnel math.

**Verdict: PREMISE FAILS.** Plan doesn't anchor on canonical OSS-to-paid successes. Differentiation claim ("open-source unlike both" — factually wrong vs Supabase) suggests founder hasn't deeply studied Supabase's playbook. Cascading: Section 1 must add canonical-success table; Section 3 must elevate docs + founder-blog + community as primary channels.

### M0c — Anti-feature surface

**Question:** Which in-scope features contradict positioning, trust model, or business model?

Reading the design doc's stated positioning: "Simpler than Auth0, more flexible than Supabase Auth, open-source." The hosted tier is $99/mo for a managed instance + $0.001/MAU above 10K.

**Anti-feature candidates:**
1. **Hosted tier at $99/mo flat for a SINGLE managed instance** — this is enterprise pricing wrapped in indie packaging. Indie buyers (solo devs, YC startups) won't pay $99/mo for auth when Clerk is $25+usage. Enterprise buyers won't take a "single instance" seriously (need SSO, audit logs, SOC2). This pricing serves NEITHER segment well. It's a positioning anti-feature.
2. **No SSO / SOC2 / enterprise features mentioned** — but $99/mo invites enterprise comparison. Either go lower price + indie-fit, or add enterprise muscle.
3. **Hosted tier exists at all in v1** — for an OSS-first launch, hosted complicates the story. Sentry, HashiCorp added managed tier LATER, after OSS adoption proved the funnel. Shipping both in v1 splits founder attention and product story.
4. **"More flexible than Supabase Auth"** — flexibility is an anti-feature for "simpler than Auth0." Pick one positioning. Flexibility + simplicity is the dream every auth product claims and none deliver.

**Verdict: PREMISE FAILS** (4 candidates surfaced, all real). Cascading: Section 6 must reframe pricing; Section 2 must force a single positioning. Founder owes themselves a "kill, defer, or restrict to enterprise tier" decision on the hosted-v1 question.

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the acquisition tactic select for the wrong segment?

The OSS SDK is free (MIT). The hosted tier is $99/mo. Validation gate is "100 GitHub stars + 5 hosted-tier signups."

**Selection-bias analysis:**
- **MIT OSS SDK** → attracts time-rich/money-poor users (indie hackers, hobby projects, students). These users *self-host*, never pay.
- **Star-the-repo signal** → costs zero, signals zero purchase intent (GitHub stars benchmark: stars reflect curiosity, not buying). At 0.5-3% OSS conversion, 100 stars yields ~0.5-3 paid signups expected — gate of "5 hosted signups by day 60" requires either >150 stars OR a wildly above-benchmark conversion rate.
- **Hosted tier at $99/mo** → priced for someone whose time is worth >$99/mo of saved auth-management effort. This is post-seed YC startup territory or small Series A teams, NOT the indie hacker who stars the repo.

**Mismatch confirmed:** the OSS distribution surface attracts indies who won't pay; the hosted tier targets a different segment (small-team SaaS) that doesn't browse Show HN looking for auth SDKs — they ask their CTO, evaluate Clerk vs Auth0, and decide on a Friday.

**Verdict: PREMISE FAILS.** The validation cohort (OSS users, HN browsers) and the paying cohort (small-team SaaS CTOs) are different humans. Cascading: M5/M6 must add high-trust acquisition mechanics (direct outreach to specific named SaaS teams, content targeted at CTOs, NOT generic HN/Reddit promotion).

### M0e — Dogfood audience-class match

**Question:** Is the dogfood audience = paying ICP?

Founder is ex-Stripe engineer building auth. **The founder IS the dogfood audience** (backend engineer who needs auth for their own projects). The paying ICP per the plan is also "backend engineers building auth into their apps."

**Surface match:** identical.

**Deeper match:** suspect. Founder = elite ex-Stripe engineer who can self-host anything trivially. Paying ICP = backend engineer at a startup who CAN self-host but chooses not to because their time is worth more than $99/mo. These are different psychographics:
- Founder will tune for power, flexibility, depth ("more flexible than Supabase Auth")
- Paying ICP wants speed, defaults, "just works" (this is what Clerk's $25/mo + $0.02/MAU customers buy)

**Verdict: PREMISE INCONCLUSIVE — leaning fail.** The titles match but the time-cost/skill-tier psychographics don't. Cascading: M1 must force the founder to name a SPECIFIC paying ICP persona that is meaningfully different from the founder's own profile.

### PREMISE-LEVEL FINDINGS BLOCK (≥2 failed, surface at top)

> **Step 0.5 verdict: M0a survives with nuance, M0b FAILS, M0c FAILS, M0d FAILS, M0e INCONCLUSIVE-LEANING-FAIL.**
>
> **The 4 highest-leverage findings before any tactical work:**
>
> 1. **The differentiation claim is factually wrong and strategically thin.** Supabase Auth IS open-source. Clerk is the real growth threat for indie/small-team SaaS and isn't mentioned. The plan inherits competitive framing without verifying it.
>
> 2. **The OSS funnel math doesn't support the validation gate.** Industry-benchmark OSS-to-paid conversion is 0.5-3%. 100 stars → 0.5-3 expected paid signups, not 5. Gate is either unrealistic or requires above-benchmark conversion the plan doesn't engineer.
>
> 3. **Pricing is split-segment incoherent.** $99/mo flat is enterprise-style for solo-team value, but lacks SSO/audit/SOC2 to win enterprise. Indies won't pay it, enterprises won't take it seriously. Either go $19-39 self-serve indie tier, or build the enterprise muscle for $99-499 multi-tier.
>
> 4. **Founder's 20K blog readers + 3K dev-Twitter are the load-bearing distribution surface, NOT Show HN.** Plan currently demotes the founder's actual leverage to a footnote and elevates a lottery channel to primary. Order is inverted.

---

## Step 0A — Forcing questions (M1–M7) with naive founder answers + skill challenges

### M1 — Audience reality

**Skill question:** Name a specific person who would actively seek out AuthForge. Where do they hang out RIGHT NOW?

**Naive founder answer:** "Backend engineers building startups. They're on Twitter and HN."

**Skill challenge:** Refused. "Backend engineers" is a category, not a person. "Twitter and HN" is where the founder hangs out, not necessarily where the paying ICP hangs out. M0e flagged the dogfood-vs-buyer mismatch.

**Forced concrete answer:**
- **Persona:** "Maya, 28, senior backend engineer at a 12-person seed-stage SaaS that just raised. CTO told her 'figure out auth this sprint, we're getting design-partner deals next month.' She has ~10 days to ship a working sign-in + Google OAuth + invite-team flow. She CAN self-host but won't — she'd rather spend $50-100/mo of company money than 3 days of her time."
- **Where Maya hangs out NOW:** (1) GitHub trending + her CTO's shared bookmarks, (2) the YC Bookface alumni Slack auth-channel discussions, (3) Indie Hackers (lurks), (4) Hacker News (~weekly), (5) specific Twitter accounts she follows: @t3dotgg, @leeerob, @rauchg, @shadcn, (6) "How to do auth in [her stack]" blog posts that rank on Google.
- **What she pays for in adjacent categories:** Vercel, Supabase, Linear, PostHog, Resend — all in the $20-100/mo/seat range for tools that save engineer time.
- **What she complains about:** "Auth0 pricing cliff at 7K MAU is brutal." "Supabase Auth is fine but limits OAuth provider customization." "Clerk is great but vendor lock-in scares my CTO."

**Status:** PASS after challenge. Specific persona + 5+ attention surfaces + specific competitor friction points.

### M2 — Discovery path

**Skill question:** How does Maya discover AuthForge? Minimum 3 steps. Step 1 is NOT "she sees my Show HN."

**Naive founder answer:** "She sees AuthForge on HN front page and clicks through."

**Skill challenge:** Refused per rule. Also: per M0a nuance, HN can be in the funnel but cannot be step 1 if there are higher-leverage entries via the founder's existing surfaces.

**Forced concrete answer (3-path):**
- **Path A (highest probability, leverages founder's actual leverage):** Maya reads founder's technical blog (she's in the 20K monthly readers) → founder writes "I left Stripe to build the auth tool I wish existed" post → she bookmarks it → 2 weeks later she's tasked with auth → returns to blog → clicks to AuthForge.
- **Path B (community/intermediary):** @t3dotgg or @leeerob (or other React/Next-Twitter influencer) tweets about AuthForge after founder DMs them a polished demo → Maya sees the tweet → clicks through.
- **Path C (HN as confirmation, not discovery):** Maya sees AuthForge on HN front page → checks GitHub stars (>500 = serious) → checks founder's blog (ex-Stripe = serious) → bookmarks for evaluation.

Realistic time-to-discovery: 2-4 weeks from launch for path A/C, days for path B if influencer plays ball.

**Status:** PASS after challenge. Three specific paths, named intermediaries, realistic timing.

### M3 — Pre-launch audience

**Skill question:** Show evidence of audience you ALREADY have. Specific numbers.

**Naive founder answer:** "I have ~3K Twitter followers and a popular blog."

**Skill challenge:** "Popular blog" is vague. Numeric?

**Forced concrete answer:**
- Twitter/X: ~3,000 followers, dev-Twitter (backend/infra concentration based on bio)
- Blog: ~20,000 monthly readers
- Newsletter: zero (significant gap)
- GitHub stars on prior projects: unknown — founder needs to surface
- Discord/Slack identity-engineer community presence: zero

**Status:** PASS. Numbers exist. Both surfaces are ICP-aligned. Newsletter gap noted as a fix-this-now item.

### M4 — Channel honesty

**Skill question:** Name ONE distribution channel where you have a credible advantage over a generic founder.

**Naive founder answer:** "I'm good at writing technical content. People read my blog."

**Skill challenge:** This one ACTUALLY passes the bar — 20K monthly readers IS demonstrated capability with a track record.

**Forced concrete answer:** Founder's **technical blog (20K monthly readers, ICP-aligned)** is the credible distribution advantage. Secondary: dev-Twitter (3K followers, decent but not massive). The blog is the single biggest leverage point in the entire plan.

**Status:** PASS. Real channel + real evidence.

### M5 — Competitor traffic source

**Skill question:** Where do Auth0, Clerk, Supabase Auth, Stytch, WorkOS actually get their users from?

**Naive founder answer:** "I don't really know. Probably ads and SEO?"

**Skill challenge:** "I don't know" is acceptable IF coupled with commitment to research. Web-search findings I can offer:
- **Auth0:** SEO dominant on "auth0 vs", paid Google ads, enterprise sales, developer-conference sponsorships
- **Clerk:** dev-Twitter founder presence (Colin Sidoti, Braden Sidoti), React/Next.js ecosystem placement (Vercel docs reference), heavy YouTube/dev-influencer partnerships, conversion-optimized homepage with copy-paste components
- **Supabase Auth:** ride-along on Supabase's broader content + community + YC network + Y Combinator dev-Twitter (Paul Copplestone). Their growth is Supabase's growth.
- **WorkOS:** B2B content + SDR-led enterprise sales, "User Management" page seo, conference sponsorship
- **Stytch:** developer content + integrations marketplace, less consumer-visible

**Pattern:** Every winner has FOUNDER PRESENCE + CONTENT INFRASTRUCTURE + COMMUNITY. Paid ads alone never built these.

**Status:** PASS with research-assist. Founder commits to deeper SimilarWeb analysis pre-launch.

### M6 — First 10 paying customers

**Skill question:** Name the specific path to first 10 paying customers. Not "viral on HN."

**Naive founder answer:** "GitHub stargazers who upgrade to hosted tier."

**Skill challenge:** REFUSED. Per M0d, this is freebie-disqualifier failure — OSS stargazers ≠ $99/mo buyers. Also passive language. Per OSS conversion benchmarks (0.5-3%), need 333-2000 stars to expect 10 paid; gate of "100 stars by day 60" doesn't support it.

**Forced concrete answer (real path to 10):**
- 5 from **direct named outreach**: founder personally emails/DMs 30-50 small SaaS CTOs (YC W25/S25 batch, Bookface alumni, dev-Twitter connections) offering free 3-month managed instance in exchange for case study. Convert 5 to paid after trial.
- 3 from **influencer-amplified blog post**: founder writes "Why we built AuthForge" blog post; gets 2-3 dev-Twitter influencers (@t3dotgg, @leeerob, @theo) to retweet (founder has the social capital from ex-Stripe + blog). Blog post drives 50-100 evaluation signups; 3 convert.
- 2 from **HN/community organic**: Show HN + IndieHackers post drive some traffic; conversion from these is ~1-2 customers (per OSS-to-paid math).

Total: 10 customers, with the BULK from high-trust outreach + influencer amplification, NOT from organic OSS stargazing.

**Named 10 to email tomorrow:** founder should list 10 specific small-team SaaS CTOs in their network/extended network this week. (Founder action item.)

**Status:** PASS after challenge. Path is concrete, sequenced, realistic.

### M7 — Time allocation

**Skill question:** What percentage of pre-launch time is on audience-building vs building?

**Naive founder answer:** "Probably 90% building, 10% writing the occasional blog post."

**Skill challenge:** Per the skill, <30% on audience = wrong ratio. Per the marketing-naive default + the fact that the founder's BIGGEST LEVER is the blog audience, the ratio should arguably be higher than 30% — closer to 40-50% for this founder because the audience-leverage is their primary moat.

**Forced commitment:** rebalance to 60% building / 40% audience-building during the next 60 days. Named audience activities:
- 2 blog posts/week on auth-specific topics (positioning content, technical deep-dives, "why we built X")
- 1 build-in-public Twitter thread/week with screenshots
- 1 outreach session/week: 10-20 cold DMs to specific small-team SaaS CTOs
- 1 community presence/week: substantive comments in 2-3 relevant Discord/Slack identity-engineer channels

**Status:** PASS only with rebalance. Original 10% is a known risk; corrected to 40%.

### Forcing-question score: 7/7 PASS (after challenges applied)

---

## Step 0B — Mode selection

Founder has REAL ICP-aligned audience (20K blog + 3K dev-Twitter) + competitive context now exists (web-searched in Step 0). Per skill rules: **Mode A — Full Marketing Review.** All 9 sections run.

Mode A confirmed. Proceeding.

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | Founded | Pricing (2026) | Apparent traffic sources | Common user complaints | Positioning vs AuthForge | Winning? |
|---|---|---|---|---|---|---|
| **Auth0 (Okta)** | 2013 | Free 25K MAU, Essentials $35/mo, B2C/B2B custom, ~$0.07/MAU at scale | SEO-dominant ("auth0 vs"), Google paid, enterprise SDR, conferences | "Pricing cliff at MAU thresholds is brutal", "feels enterprise-bloated for indie", lock-in | Enterprise incumbent; AuthForge MUST not anchor here for indie/small-team buyers | Yes for enterprise; losing indie share to Clerk/Supabase |
| **Clerk** | 2019 | Free 50K MAU (raised from 10K in Feb 2026), Pro $25 + $0.02/MAU, Enterprise custom | Founder dev-Twitter (Sidoti brothers), React/Next.js ecosystem placement, YouTube dev-influencers, copy-paste components on homepage | Closed-source = vendor lock-in concern; pricing creeps at scale | The dominant indie/small-team React-stack auth choice. AuthForge's biggest growth threat for the EXACT segment AuthForge wants. | Yes — dominant winner of the React indie/small-team segment |
| **Supabase Auth** | 2020 | 50K MAU free, then $0.00325/MAU; self-hostable OSS | Rides Supabase platform growth (YC alumni, dev-Twitter, OSS community) | Limited OAuth provider customization; tightly coupled to Supabase platform | OSS + cheap + part of broader platform. AuthForge's claim "open-source unlike both" is FACTUALLY WRONG vs Supabase Auth. | Yes for Supabase-stack users; not a standalone winner |
| **Stytch** | 2020 | 10K MAU free, pay-per-MAU after; passwordless + OAuth specialty | Developer content, integrations marketplace, less consumer-visible | Niche positioning; smaller community than Clerk | Passwordless-specialist; not direct AuthForge competitor unless AuthForge picks that wedge | Moderate; specialist play |
| **WorkOS** | 2019 | AuthKit 1M MAU free, SSO per-connection paid | B2B content, SDR-led enterprise, "User Management" SEO | Pricing opacity; enterprise-focused | B2B enterprise specialist; orthogonal to AuthForge's stated indie/small-team aim | Yes for enterprise SSO |
| **Better Auth** | 2024-2025 | OSS framework, self-host (no hosted tier shown publicly) | Dev-Twitter, OSS community, indie-React-stack | Newer, less battle-tested | Closest analog to AuthForge's OSS-first positioning; emerging competitor | Emerging; momentum strong |
| **Kinde** | 2022 | Free tier, low per-MAU | Content marketing + B2B SaaS targeting | Younger community | Indie/SMB SaaS positioning | Moderate |

**Read:** AuthForge's segment is the most CROWDED segment in identity (indie + small-team SaaS, React-stack tilt). Clerk dominates UX. Supabase Auth dominates OSS + platform-bundled. Better Auth is the closest direct OSS-first analog and already has momentum. **AuthForge must pick a sharper wedge than "simpler + more flexible + open-source" — those three are NOT a positioning, they're a wishlist.**

### 1b. Canonical-success comparables (the part most plans skip)

| Canonical | Founded | Pricing | Primary acquisition channel | Onboarding model | Launch gate | Specific delta from AuthForge plan |
|---|---|---|---|---|---|---|
| **Sentry** | 2012 | OSS free; hosted $26/mo (Team), $80/mo (Business), enterprise custom | OSS adoption → hosted upsell as scale hits; docs-as-marketing; community | Self-serve hosted with strong docs; OSS self-host for the technical | Built OSS adoption FIRST; hosted came after community proved funnel | AuthForge ships hosted v1 alongside OSS; Sentry waited for OSS proof |
| **HashiCorp** | 2012 | OSS free; enterprise Vault/Consul/Terraform at significant $$ | OSS adoption → enterprise sales; conferences (HashiConf); strong written content | OSS self-serve; enterprise concierge | Years of OSS adoption before enterprise GTM scaled | AuthForge has no enterprise muscle; can't follow this path exactly but the "OSS-first, monetize narrow" pattern applies |
| **Supabase** | 2020 | Free 50K MAU, Pro $25, Team $599, Enterprise custom | YC network + dev-Twitter founder presence + OSS community + content | Self-serve cloud + OSS self-host | Calendar-paired-with-traction; iterated publicly | AuthForge could mirror this BUT founder needs to commit to public-iteration cadence Supabase founders did |
| **PostHog** | 2020 | Free tier with usage-based paid | OSS as wedge to first 1K users, then 97% word-of-mouth; transparent everything | Self-serve cloud + OSS self-host | Iterated publicly; 6 pivots in 9 months before PMF | AuthForge plan has NO explicit pivot tolerance; treats day-60 gate as success criterion |
| **Cal.com** | 2021 | OSS free; hosted tiers | Founder daily ships-in-public on Twitter (Peer Richelsen); OSS community | Self-serve + OSS | Continuous public iteration | AuthForge plan lacks founder-presence cadence equivalent |
| **Plausible** | 2019 | OSS free; hosted $9-49/mo | Slow-compound content marketing + founder Twitter (Uku Taht) | Self-serve hosted; OSS self-host | Slow-compound, no big-bang launch | AuthForge gates on big-bang day-60 metric; Plausible-style slow-compound was the playbook |
| **Stripe** (developer-first reference) | 2010 | API per-transaction | Docs-as-marketing, developer-relations, integration partnerships | Self-serve with copy-paste examples | Continuous; no single launch | Founder is ex-Stripe — has internal exposure to this playbook. PLAN doesn't reflect Stripe-tier docs investment. |

### 1c. Pattern surface

**What canonical successes have in common that AuthForge plan lacks:**
1. **Founder presence is treated as primary distribution.** Cal.com (Peer Richelsen), PostHog (James Hawkins), Supabase (Paul Copplestone), Plausible (Uku Taht), Sentry (David Cramer) all ship in public continuously. AuthForge plan has zero stated founder-cadence commitment.
2. **OSS is the wedge to FIRST 1K users; hosted comes after.** PostHog explicit on this. AuthForge ships both in v1 — splits attention.
3. **Docs as the conversion surface.** Sentry, Stripe (founder's alma mater!), Supabase all invest heavily in docs as primary conversion. AuthForge plan says "integration tutorials" as an afterthought.
4. **Continuous iteration with public pivot tolerance.** PostHog 6 pivots in 9 months. AuthForge has day-60 gate as binary success/fail — too rigid.
5. **Community presence (Discord/Slack).** Every winner has an active community surface. AuthForge plan has none.

**What AuthForge's plan is implicitly following:** the "build the OSS tool, post Show HN, hope it goes viral" pattern. This is the canonical FAILURE mode for OSS dev tools — it's what produces the long tail of <500-star repos that ship to silence. Canonical successes systematically DO MORE than this.

**Action:** rewrite Section 4 (pre-launch audience) and Section 5 (launch playbook) to elevate founder content + docs + community to primary channels, with HN/r/programming/PH as secondary amplification.

---

## Section 2 — ICP specification

See standalone artifact: **`icp.md`** (Maya persona — senior backend engineer at seed-stage SaaS, sub-month auth-shipping deadline).

Tight summary:
- **Primary ICP:** Maya (senior BE engineer at 5-15 person seed/A-stage SaaS, React/Next stack, has 1-3 weeks to ship auth, can self-host but trades $ for time, decision authority for $50-200/mo tools)
- **NOT the ICP:** indie hackers shipping side projects (free OSS users who never pay), Fortune 500 (needs SSO + SOC2 + compliance AuthForge doesn't have in v1), agency contractors (use whatever client mandates)
- **Where Maya is now:** GitHub trending, YC Bookface auth-channel, IH lurker, weekly-HN visitor, follows specific React-Twitter (Theo, Lee Robinson, Guillermo Rauch, Shadcn), Google for "[stack] auth" tutorials.

---

## Section 3 — Distribution channel-by-channel

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Ranked Leverage | Verdict |
|---|---|---|---|---|---|---|---|
| **Founder's technical blog (20K/mo)** | High & ICP-aligned | Already paid (time) | Highest-trust signal of any channel | EXCELLENT — proven track record | Med (writing cadence) | **#1** | PRIMARY — load-bearing |
| **Dev-Twitter (founder's 3K + outreach to influencers)** | Med | Low | High when influencer-amplified | GOOD — exists | Med | **#2** | PRIMARY |
| **Docs-as-marketing (Stripe-style)** | Compounds via SEO over time | High one-time investment | Very high conversion at evaluation moment | EXCELLENT — founder knows Stripe DX | High | **#3** | PRIMARY (investment now, compounds) |
| **Direct outreach to small-team SaaS CTOs** | Low (volume) | High (time) | Very high (50%+ trial→paid in target segment) | GOOD — founder has YC/Stripe network | High | **#4** | PRIMARY for first-10-customer push |
| **GitHub presence (README + examples + good Issues hygiene)** | Med | Low | Quality-signal for evaluators | EXCELLENT — engineer's home turf | Med | **#5** | PRIMARY (table stakes) |
| **Show HN** | High variance (lottery) | Low | Medium when it hits | OK — every founder posts | Low (one shot) | **#6** | SECONDARY — amplification event, not primary |
| **r/programming** | Med if not auto-removed | Low | Low (self-promo bans common) | Low | Low | **#9** | CUT or only as cross-post via accounts with karma |
| **IndieHackers** | Niche but ICP-tangent | Low | Low (segment mismatch — IH is for indie devs not small-team CTOs) | OK | Low | **#10** | CUT or one-time launch cross-post only |
| **Product Hunt** | Med | Low | Low for OSS dev tools (PH audience tilts consumer/no-code) | Low | Med | **#11** | CUT for v1 |
| **Substack/newsletter** | Currently 0 | Low | High retention if built | Founder doesn't have one yet | High to start | **#7** | START NOW, slow compound |
| **Discord/identity-engineer communities (Reactiflux, T3, Theo's Ping)** | Niche but high-trust | Low | High conversion when authentic | OK (founder must show up) | Med | **#8** | START NOW — at least show up 2-3 times/week |
| **Podcast guesting (Software Engineering Daily, Syntax.fm, JS Party)** | Med | Low | Med (slow compound) | Founder profile (ex-Stripe) is podcastable | Med (outreach effort) | **#12** | DAY 30+ after some traction |
| **YouTube tutorials** | High compound | High effort | High | Founder doesn't have video presence | Very high | DEFER | Don't start in first 90 days |
| **Paid ads** | Variable | High | Med (auth keywords are expensive — Auth0 outbids) | None | High | DEFER | v2+ |
| **SEO (programmatic "[stack] auth" pages)** | High over 6-12mo | Med | High (intent-aligned) | Founder can write | High to start, compounds | **PARALLEL TRACK** | START NOW — 1 evergreen post/week |

**Top 4 channels to actually ship (refusing "we'll do them all"):**
1. **Founder's blog** (cadence + topical relevance to auth)
2. **Founder's Twitter + influencer amplification** (DMs to Theo/Lee/Rauch with demo before launch)
3. **Stripe-tier docs + GitHub README** (this IS marketing for dev tools)
4. **Direct outreach to 30-50 named small-team SaaS CTOs**

HN/PH/r/programming are amplification events on the launch day sequence, NOT the strategy.

---

## Section 4 — Pre-launch audience-building plan (30/60/90)

Founder already has 20K blog readers + 3K Twitter, so this is less "build audience" and more "ACTIVATE the audience around the AuthForge story."

**Day 1-30: Activate**
- 2 blog posts/week on auth topics: "What I learned about auth at Stripe", "Why every React startup builds the same broken auth flow", "OAuth providers ranked by pain", positioning content.
- 1 build-in-public Twitter thread/week with screenshots, decisions, tradeoffs.
- Launch a newsletter (currently zero) — convert ~5% of blog readers to subscribers = ~1000 subscribers in 30 days if blog promotes signup. Lead magnet: "The auth checklist for React startups."
- Show up in 2-3 Discord communities (Reactiflux, T3, Indie Hackers) — substantive comments, not promo.
- DM 5-10 dev-Twitter influencers offering early access + asking for feedback (Theo, Lee Robinson, Rauch, Shadcn, Vercel devrel).
- Set up GitHub repo (even pre-launch); README quality > code quality at this stage.

**Day 31-60: Amplify**
- Continue 2 blog posts + 1 Twitter thread weekly.
- 1 podcast pitch/week (Software Engineering Daily, Syntax, JS Party, ChangeLog, MFM-dev-edge).
- Outreach: 10 named small-team SaaS CTOs/week → personal email offering free 3-month managed instance + a brief co-build call.
- Start drafting Show HN post + Twitter launch thread + LinkedIn post. Get feedback from 5 trusted people.
- Identify Product Hunt hunter (defer the actual launch — see Section 5).

**Day 61-90: Launch + post-launch sustain**
- Launch sequence per Section 5.
- Weekly retro blog post: "AuthForge week N: what we learned" — converts launch into compounding content.
- Open Discord for AuthForge users.
- First case-study post with a paying customer.

**Required cadence commitment:** 40% founder time on audience/content, 60% on product. (Per M7 challenge.) If this slips below 30%, the plan is failing silently — recurring check.

---

## Section 5 — Launch playbook

### 5a. Question the launch gate FIRST

**Current gate:** "100 GitHub stars + 5 hosted-tier signups by day 60." Calendar-driven + low-bar + vanity-metric tilted.

**Challenge:** dev tools BENEFIT from a launch moment (unlike consumer subscriptions where Vohra-style PMF gates are paramount). HN/PH/Show HN reward calendar-driven moments. So calendar-gating is DEFENSIBLE for AuthForge.

**However**, the gate METRICS are wrong:
- 100 stars = vanity. PostHog, Sentry, Supabase all had >1K stars before serious paid conversion.
- 5 hosted signups = too small to indicate anything. Need to know: do they USE it? Do they RENEW month 2? Are they referring colleagues?

**Replace gate with:**
- Calendar: launch day = day 60 (locked, dev-tool benefit of calendar moment)
- Quality gate: ≥500 GitHub stars, ≥1 customer who unprompted refers a colleague, ≥3 customers who complete full integration (auth flow live in prod), retention proxy = 3-of-5 hosted signups active week 2.
- If quality gate fails: launch the SDK publicly, KEEP hosted tier in private beta until the quality bar hits.

This is the **concierge-first cohort** pattern: founder personally onboards first 5-20 hosted customers, doesn't widen hosted GA until dependence is verified. Sentry / Vercel / Linear all did this.

### 5b. Sequenced launch playbook

See standalone artifact: **`launch_playbook.md`** with hour-by-hour Day 0 sequence + Day -30 to Day +30 schedule.

Top-line sequence:
- **Day -30:** Begin audience-build cadence per Section 4. Start pre-warming.
- **Day -14:** Soft email to ~50 personal network. "Here's what I'm shipping in 2 weeks; want a beta invite?"
- **Day -7:** Twitter build-in-public thread previewing AuthForge (decisions, screenshots).
- **Day -3:** Blog post drafted: "Why I left Stripe to build AuthForge" — embargoed, post on Day 0.
- **Day 0 (Monday morning Pacific):** Show HN post; blog post live; Twitter launch thread; email to all 50 network preview people asking for upvote/comment if genuine.
- **Day 0 +2hr:** Reach out to influencers (Theo, Lee, Rauch) with link asking for retweet if they like it.
- **Day 0 +4hr:** LinkedIn long-form post (different audience overlap).
- **Day 0 +24hr:** Cross-post to IndieHackers (HN-first to avoid duplicate-content penalty).
- **Day 0 +48hr:** Compliant cross-post to r/SideProject (NOT r/programming — too high ban risk).
- **Day 0 +7d:** Product Hunt launch event (separate audience).
- **Day 0 +14d:** Podcast outreach to 5 podcasts.
- **Day 0 +30d:** Retro blog post with traction numbers.

**Risk callouts:**
- HN miss = recovery still possible because blog + Twitter + outreach are independent channels (this is the multi-channel benefit)
- r/programming auto-remove risk → CUT from sequence entirely
- Single-influencer dependence → outreach to 5-10 influencers, expect 1-2 to amplify

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing BAND first

**Current pricing:** $99/mo flat hosted + $0.001/MAU above 10K.

**Band-inheritance analysis:**
- $99/mo flat doesn't match any direct competitor band. Clerk Pro = $25 base + $0.02/MAU. Supabase Pro = $25 + usage. Auth0 Essentials = $35. WorkOS AuthKit = free.
- $99/mo flat looks like founder picked a "professional services" feeling number, not a band-justified number.
- $0.001/MAU is suspiciously cheaper than Supabase ($0.00325/MAU) and Clerk ($0.02/MAU). This is "match the cheapest competitor" reflex per anti-pattern #7 — wrong move for trust-led indie/small-team segment.

**ICP willingness-to-pay evidence (from Section 2 ICP):**
- Maya pays $20-100/mo for tools that save her engineering time (Vercel, Supabase, Linear, PostHog).
- Maya's CTO authorizes $50-200/mo tool spend without escalation.
- The right band for Maya = $25-79/mo entry tier with usage scaling.

**Verdict: band is wrong both directions.** Too high ($99 flat) for indie-tier price-sensitive buyers; too low ($0.001/MAU scaling) to capture serious enterprise spend. Pricing is split-segment incoherent.

### 6b. Recommended pricing restructure

**Three-tier alternative:**
1. **Free (self-host OSS)** — full SDK, MIT, no support, unlimited self-host. The wedge.
2. **Starter hosted: $29/mo** — managed instance + 10K MAU + email support + 1 SSO connection. Matches Clerk's $25 anchor. Indie/small-team-friendly.
3. **Team hosted: $99/mo** — 50K MAU + priority support + 3 SSO connections + audit logs. Where small-team SaaS lands.
4. **Enterprise: custom** — SSO unlimited, SOC2, dedicated support. Defer to v2 / post-traction.

**MAU overage:** $0.005/MAU (between Supabase $0.00325 and Clerk $0.02) — premium-discount band, not race-to-bottom.

**Annual billing:** 20% discount; required for retention per RevenueCat-style subscription benchmarks.

**Trial mechanic:** 14-day free trial of Team tier with credit card required (selects against time-rich/money-poor freebie-hunters per M0d). Or alternative: founder-onboarded concierge cohort for first 20 customers, no trial mechanic needed.

---

## Section 7 — Post-launch growth loops

| Loop | Compound or linear? | Plan it |
|---|---|---|
| **Referral mechanics** (in-product "invite team" generates auth signup for invitee's downstream company) | Compound (low-rate but cheap to ship) | YES — natural for auth product; "Powered by AuthForge" footer on free tier signin pages (optional, off by default) generates inbound |
| **Content compounding (SEO ranking)** | Compound (6-12mo ramp) | YES — 1 evergreen post/week on "[stack] auth" queries |
| **Network effects (product better as more use it)** | Linear (auth doesn't benefit from network) | NO — auth is not network-effect-native |
| **Brand compounding (founder presence)** | Compound (named ex-Stripe = trust capital that grows) | YES — load-bearing for this plan |
| **Retention as growth (word-of-mouth)** | Compound | YES — concierge first cohort = strong WoM; PostHog's 97% WoM is the target |

**Risk if NONE of these compound:** acquisition-treadmill, every customer requires new spend. AuthForge has plausible compounding loops, so this isn't acute — but only if founder commits to content + docs cadence.

---

## Section 8 — Metrics & instrumentation

**Measure (weekly dashboard):**
- New GitHub stars (with source UTM-equivalent if possible via referrer)
- Newsletter signups (with referrer)
- Hosted-tier signups by source (blog / Twitter / HN / outreach / referral)
- Hosted-tier trial → paid conversion %
- Activation: % of hosted signups who complete first auth flow within 7 days (key activation metric)
- Day-7 / Day-30 retention of hosted customers
- Unprompted referrals (count + source)
- Blog traffic + post-level conversion to newsletter
- Twitter engagement on AuthForge-tagged threads

**Do NOT optimize (vanity):**
- Twitter follower count (loose correlation with revenue)
- Total GitHub stars in isolation
- HN upvote count (correlation with revenue near-zero per skill)
- Newsletter signups without activation rate

**Weekly review cadence:** every Friday, founder reviews dashboard + writes 1-paragraph retro (publicly if comfortable — build-in-public extends content cadence).

---

## Section 9 — Risk analysis

| Risk | Likelihood | Severity | Mitigation |
|---|---|---|---|
| Channel concentration on founder's blog | Medium-high (it IS the load-bearing surface) | High if blog momentum stalls | Build newsletter as second compounding surface; influencer relationships as third |
| Clerk + Supabase Auth + Better Auth squeeze the indie/small-team segment | High | High | Pick sharper wedge than "simpler + flexible + OSS"; consider verticalizing (e.g., "auth for React + Vercel + Postgres" specifically) |
| OSS adoption never translates to hosted conversion | Medium-high | Critical (the whole business depends on it) | Concierge first cohort; direct outreach to 30-50 named CTOs is the hedge against organic conversion failure |
| Show HN gets <30 upvotes | Medium | Low if multi-channel; high if HN-dependent | Multi-channel sequence (Section 5) explicitly de-risks single-shot |
| r/programming auto-removal / community backlash | High (if attempted) | Low (cut from plan) | Already cut from plan; use r/SideProject only |
| Founder time underspent on audience | Medium-high (default for technical founders) | High | 40% cadence commitment; weekly Friday retro that tracks ratio |
| Better Auth or other emerging OSS competitor wins the wedge first | Medium | High | Ship docs + founder presence faster; OSS license is MIT (good — no AGPL trust friction) |
| Hosted tier pricing wrong — too expensive for indie, too thin for enterprise | High under current $99 flat | Critical | Restructure to 3-tier per Section 6b before launch |
| Founder burnout from 60% build + 40% audience pace | Medium | High | Set 2 explicit "no work" days/week; treat the cadence as a 6-month commitment not a sprint |

---

## Outside voice — independent marketing critique

Simulated independent critique (would be run via Codex CLI / Claude subagent in real session):

**1. Biggest marketing risk inside review missed:** **The product is undifferentiated in the most crowded segment of identity.** "Simpler than Auth0, more flexible than Supabase Auth" is the literal positioning every auth startup has used since 2018. Inside review surfaced this but didn't push hard enough on the VERTICAL or USE-CASE wedge. Real recommendation: pick a stack (e.g., "auth for the Next.js + Vercel + Postgres stack, with React Server Components first-class") OR a use case (e.g., "auth for B2B SaaS that needs team-invites + role-based access from day 1"). Generic horizontal auth in 2026 is graveyard territory.

**2. Channel mentioned weaker than positioned:** **Direct outreach to 30-50 named small-team SaaS CTOs.** This SOUNDS leveraged but DM cold-conversion to small-team CTOs is genuinely brutal — these people get 20+ pitches/week. Realistic conversion: 5-10% reply rate, 1-2% trial conversion. To get 5 paid customers from this channel, founder needs to send 250-500 high-quality personalized DMs. That's 4-6 weeks of dedicated outreach time. Inside review under-priced this effort.

**3. Audience claim lacking evidence:** **"20K monthly blog readers, ICP-aligned" — what fraction are buyers vs other engineers?** 20K monthly readers includes a lot of other engineers reading for craft, not for buying decisions. The conversion-relevant subset is the ones who happen to be at companies with auth-buying authority RIGHT NOW. Could be 5-10% of the 20K = 1-2K buyer-adjacent. Still material but smaller than the headline suggests.

**4. Provocative reframe:** **Should AuthForge be a hosted product at all in v1?** Sentry, HashiCorp, Supabase, PostHog ALL built OSS adoption first, then added hosted. AuthForge is splitting attention v1 across OSS SDK + hosted instance + pricing model + enterprise positioning. The Sentry playbook would be: ship the OSS SDK only in v1, do not offer hosted, build to 5K GitHub stars + a vibrant Discord, THEN announce hosted in v2 (month 6-9) with a waiting list of self-host users who want to upgrade. This trades short-term revenue (zero) for sharper product story + faster OSS adoption.

---

## THIS WEEK action items (force founder to commit)

1. **Rewrite the positioning.** Drop "simpler than Auth0, more flexible than Supabase Auth, open-source unlike both" (factually wrong + ungrounded). Pick ONE wedge by Friday: stack-specific (Next.js + Vercel) OR use-case-specific (B2B SaaS team invites + RBAC from day 1).
2. **Decide hosted-tier-in-v1 vs OSS-only-v1.** Per outside voice reframe, this is the single biggest strategic call. If hosted-in-v1 stays, restructure pricing to 3-tier per Section 6b. If OSS-only-v1, defer hosted to v2 and pivot validation gate to "1K GitHub stars + active Discord by day 90."
3. **Start the newsletter THIS WEEK.** Currently zero subscribers — biggest fixable audience gap. Add signup CTA to founder's blog (20K readers); even 5% conversion = 1K subscribers in 30 days. The newsletter compounds across launch + post-launch in a way Twitter does not.

---

## Follow-up skills

- `/office-hours` if positioning shifts after action item #1
- `/plan-ceo-review` if hosted-tier-in-v1 decision changes business model
- `/plan-eng-review` if newsletter + in-product referral mechanics require product spec updates
- Re-run `/plan-cmo-review` in 30 days against actual progress



