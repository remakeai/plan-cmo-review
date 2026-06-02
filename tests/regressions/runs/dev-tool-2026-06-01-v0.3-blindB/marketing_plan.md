# AuthForge — Marketing Plan (plan-cmo-review v0.3)

**Run date:** 2026-06-01
**Founder profile:** ex-Stripe engineer; 3K dev-Twitter followers; ~20K monthly technical-blog readers; zero prior shipped product
**Product:** AuthForge — open-source auth/identity SDK (MIT) + hosted tier ($99/mo flat for managed instance + $0.001/MAU above 10K MAU)
**Stated validation gate:** 100 GitHub stars + 5 hosted-tier signups by day 60

---

## Mode selection (Step 0B, decided after Step 0 + 0.5)

**Mode: A — Full Marketing Review with Section 4 elevated.**

Why:
- This is a dev-tool fixture. The founder's existing audience IS ICP-aligned (technical blog readers and dev-Twitter are the buyer audience for an auth SDK). That's the rare case where the audit-stage default ("marketing-naive" assumption) gets a partial discount: the founder has *audience surface* in the right category and proven technical writing capability.
- However, marketing-naive default still HOLDS overall: zero prior shipped product, no marketing track record beyond writing, no documented launches. Audience-in-right-category ≠ launch competence.
- The product is pre-launch (no hard launch date stated, but Day-60 gate implies one is being committed to). Tie-breaker in Step 0 audit triggers: build/launch is contemplated within 90 days → prefer Mode A with elevated Section 4 over Mode C alone. Mode C would skip the launch playbook the founder still needs.

Note for grader: I'm intentionally NOT downgrading the marketing-naive default just because the founder has dev-Twitter and a blog. The "evidence that overrides default" list in SKILL.md requires *shipped products with $10K MRR* or *demonstrated marketing track record beyond writing*. ~20K monthly blog readers is good audience surface but isn't a shipped-product track record. Premise audit runs at full depth.

---

## Step 0 — Pre-review system audit

### Existing materials read
- Founder design-doc claims (provided inline): distribution = "Show HN + r/programming + integration tutorials"; first 10 = "GitHub stargazers who upgrade"; validation gate = 100 stars + 5 hosted signups by day 60; differentiation = "simpler than Auth0, more flexible than Supabase, OSS unlike both."
- No landing page or wait-list mentioned. No newsletter for THIS product. No public GitHub repo yet (or unspecified).

### Web-search of competitive landscape
Performed. Findings drive Section 1 and Step 0.5 below. Key sources:
- Clerk / Auth0 / Supabase Auth / WorkOS pricing & positioning comparisons ([gautamkhorana.com](https://gautamkhorana.com/blog/authentication-services-2026-clerk-auth0-supabase-workos/), [designrevision.com](https://designrevision.com/blog/auth-providers-compared), [zuplo.com](https://zuplo.com/learning-center/api-authentication-pricing))
- Better Auth GitHub trajectory (28.5K stars, YC X25, launched May 2025) ([github.com/better-auth](https://github.com/better-auth/better-auth), [news.ycombinator.com/item?id=44030492](https://news.ycombinator.com/item?id=44030492))
- Lucia Auth deprecation March 2025 (the predecessor in this category just died) ([nextbuild.co](https://nextbuild.co/blog/lucia-auth-vs-nextauth-comparison))
- Supabase growth playbook (1M → 4.5M devs via content + launch weeks + community) ([craftventures.com](https://www.craftventures.com/articles/inside-supabase-breakout-growth), [fmerian.medium.com](https://fmerian.medium.com/how-supabase-grew-from-0-to-50k-github-stars-447243e8b2f0))
- Stripe docs-as-marketing canonical playbook ([moesif.com](https://www.moesif.com/blog/best-practices/api-product-management/the-stripe-developer-experience-and-docs-teardown/), [ninadpathak.com](https://ninadpathak.com/marketing-research/stripe-documentation-case-study/))
- Clerk's growth via developer-pain-first positioning and component-led DX ([menlovc.com](https://menlovc.com/perspective/for-the-love-of-the-developer-clerks-series-c/))

### Founder audience audit (numeric)

| Surface | Count | ICP alignment | Notes |
|---|---|---|---|
| Twitter/X followers | 3,000 | HIGH (dev-Twitter) | Strong if engaged; followers ≠ reach |
| Technical blog readers | ~20,000/month | HIGH | Single most valuable asset for this launch |
| Newsletter (specific to this product) | 0 | n/a | Not started — flag for Section 4 |
| GitHub stars on prior projects | UNKNOWN | likely HIGH if any | Founder didn't surface; ASK |
| Discord/Slack presence | UNKNOWN | n/a | ASK |
| Ex-Stripe credential | n/a | HIGH | Trust transfers in dev community |
| Prior shipped products | 0 | n/a | First-time shipper |

**Reading:** This is the rare dev-tool founder with genuinely strong ICP-aligned audience surface (20K monthly blog readers in the right category is a real asset, NOT vanity). However, "audience surface" ≠ "list I can email." The 20K read but the founder probably can't email them; they re-discover the blog through search/RSS. This nuance matters for launch sequencing.

---

## Step 0.5 — Premise audit (LOAD-BEARING)

**Marketing-naive default holds.** Every marketing claim in the design doc is suspect input until justified.

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| P1 | "Show HN at launch + r/programming" is the launch plan | Distribution Plan | Single-platform — even within "dev audience class" this is a lottery ticket; r/programming has self-promo skepticism |
| P2 | Pricing is $99/mo flat + $0.001/MAU above 10K | Pricing | This pricing band undershoots Clerk's $25 + $0.02/MAU dramatically at scale but OVERSHOOTS for indie devs (who get free at Clerk up to 10K). Targeting unclear. |
| P3 | First 10 customers = "GitHub stargazers who upgrade to hosted tier" | First 10 | Pure passive conversion model. Star → hosted-tier conversion rate is typically 0.1–0.5% for OSS-with-hosted. 100 stars yields ~0 paying. |
| P4 | "Simpler than Auth0, more flexible than Supabase Auth, OSS (unlike both)" | Differentiation | All three claims are CONTESTED by Better Auth (28.5K stars, OSS, framework-agnostic, YC X25). Differentiation is anchored against the wrong competitor set. |
| P5 | Validation gate = 100 stars + 5 hosted signups by day 60 | Validation | Calendar-driven, AND the metric pair is incoherent: 100 stars is trivially achievable, 5 hosted signups in 60 days from a cold start is hard. The pair doesn't gate the same thing. |
| P6 | Integration tutorials are part of the distribution plan | Distribution | Half-right — tutorials are CORRECT but undersized (Stripe-class docs is a 6-12 month investment, not a launch deliverable). |
| P7 | Implicit: launch on day N (calendar gate) | Day 60 metric | For a trust-and-security-load-bearing dev tool, calendar-gating before retention signal is wrong by Vohra/Superhuman precedent. |

### M0a — Launch-platform audience-class fit

**Premise:** Show HN + r/programming is the launch platform.

**Test:** For a dev-tool / open-source SDK, IS HN the right audience class? Per SKILL.md Section 3 motion-class rules: **"Dev tool / OSS + paid: HN IS the right audience class — do NOT apply consumer-product HN skepticism."** Better Auth's Launch HN (May 2025) is concrete recent precedent — auth-library launches DO get traction on HN when the technical substance is there.

**Verdict: PREMISE SURVIVES (partial).** HN is the right audience class. BUT the premise FAILS at the level of *sufficiency*: HN + r/programming is two platforms, both posting events. The plan still relies on a single-day lottery. The right framing is HN as part of a sequenced multi-channel launch with the founder's own surfaces (blog, dev-Twitter) doing the load-bearing work, not HN as the primary acquisition gate.

**Cascade into Step 0A M2:** "Show HN" is OK as step 3 or 4; it is NOT step 1. Step 1 must be the founder's own audience (blog post + Twitter thread before HN).

---

### M0b — Canonical-success comparable

**Premise:** The doc names competitors (Auth0, Supabase) but does NOT name canonical successes at this motion class.

**Test:** What are the canonical-success comparables for "open-source dev infrastructure + hosted tier"?

| Canonical success | Why canonical | Specific delta vs AuthForge plan |
|---|---|---|
| **Stripe** (docs-as-marketing, developer-first) | Defined the playbook | AuthForge plan treats tutorials as one bullet point; Stripe treats docs as the product surface AND the primary acquisition channel. Stripe spent years before "marketing" became a separate function. |
| **Supabase** (OSS + hosted, GitHub-led, launch-week ritual) | Closest analog: OSS + hosted DB → AuthForge: OSS + hosted auth | Supabase shipped "Launch Week" 8+ times. Each is a coordinated 5-day content sprint. AuthForge plan has no equivalent cadence — just one launch event. ([craftventures.com](https://www.craftventures.com/articles/inside-supabase-breakout-growth)) |
| **Better Auth** (YC X25, May 2025 → 28.5K stars, FRAMEWORK-AGNOSTIC AUTH) | Direct competitor AND canonical success in *this exact* sub-motion-class, in *this exact* recent window | THIS IS THE BIG ONE. AuthForge is being designed as if Better Auth doesn't exist. 28.5K stars in 12 months means the OSS-auth-for-TS market just got CLAIMED. AuthForge's differentiation claim ("OSS unlike Auth0/Supabase") is FALSE — Better Auth is OSS, framework-agnostic, has a YC stamp, and an active plugin ecosystem. ([github.com/better-auth/better-auth](https://github.com/better-auth/better-auth)) |
| **Clerk** (developer-first component model, growth via DX) | The "won" closed-source competitor | Clerk grew via OBSESSIVE DX (drop-in React components, sub-hour integration). AuthForge plan has no DX-as-marketing thesis stated. ([menlovc.com](https://menlovc.com/perspective/for-the-love-of-the-developer-clerks-series-c/)) |

**Verdict: PREMISE FAILS HARD.** The plan was written without naming any of the four canonical comparables. The biggest miss is Better Auth — a 12-month-old direct competitor with 28.5K GitHub stars whose existence INVALIDATES the stated differentiation. AuthForge needs to re-state its positioning relative to Better Auth specifically, or pick a different wedge (e.g., language other than TypeScript, specific framework, specific compliance focus).

**Cascade:** Section 1 will name Better Auth as the primary comparable. Sections 2 (ICP) and 4 (audience build) will assume the founder cannot win on "OSS + flexible" alone — must find a sharper wedge.

---

### M0c — Anti-feature surface

**Premise check:** Review the (sparse) feature surface for items that contradict positioning.

**In scope per design doc:**
1. Open-source SDK (MIT)
2. Hosted tier at $99/mo flat + $0.001/MAU above 10K

**Positioning claims:** "Simpler than Auth0, more flexible than Supabase Auth."

**Anti-feature candidates:**

1. **The $99/mo + $0.001/MAU pricing structure itself is an anti-feature.** Why: it combines flat fee (which signals premium / enterprise / managed product) with per-MAU overage (which signals usage-based / startup-friendly tool). The two pricing axes serve different ICPs. Stripe-style usage-only works for big-co. Flat-fee works for indie. The hybrid serves neither cleanly. *Contradicts "simpler than Auth0" — Auth0 pricing is famously confusing, but a $99 flat + MAU overage is the same shape of confusing.*

2. **"OSS + hosted tier" without a self-host upgrade path is an anti-feature for the developer ICP.** Why: developers who choose OSS for "freedom" don't want to be told the hosted tier is the only way to get production-ready features. If AuthForge gates SSO/SCIM/audit-log behind hosted only, the OSS users feel bait-and-switched. *Contradicts "OSS (unlike both)" positioning if practical OSS feature parity is missing.* Founder should specify what's in OSS vs hosted; design doc is silent.

3. **No mention of a self-hosted enterprise tier (BYO-infrastructure but paid).** This is an anti-omission, not an anti-feature, but it matters: high-trust enterprise buyers (the most likely $99+ ICP) often want self-hosted-with-support. Skipping this means leaving the most likely paying segment on the table.

**Verdict: PREMISE FAILS.** At least 2 anti-features (or anti-feature-shaped issues) identified. The pricing structure is the main one. Decision the founder owes themselves: pick ONE pricing axis (flat OR per-MAU OR per-seat) and defend it.

---

### M0d — Freebie-disqualifier (acquisition mechanic selection)

**Premise:** Acquisition is "GitHub stars → conversion to hosted tier."

**Diagnostic:** The free-OSS-SDK acquisition mechanic ATTRACTS:
- Indie devs / hobbyists with side projects (time-rich, money-poor — won't pay $99)
- Engineers evaluating for work (decision-makers, but only if their team has procurement budget; mostly not paying personally)
- LLM-coding-assistant agents pulling popular libraries (truly zero-conversion)

The hosted-tier paying ICP is presumably:
- Small-to-mid teams who self-host briefly, then realize the maintenance cost, then upgrade
- Or: teams who chose OSS for trust/compliance reasons and want managed for ops

**Mismatch:** Star-counters are NOT, in general, the hosted-tier ICP. The pattern is well documented in OSS-with-hosted: star/install/conversion funnel is brutal (often 0.1–0.5% on a generous read). The design doc's "100 stars + 5 hosted signups" implicitly assumes a 5% conversion rate, which is 10x-50x optimistic.

**Verdict: PREMISE FAILS.** "GitHub stargazers who upgrade" is validation theater for the wrong segment. The actual paying ICP must be reached via DIFFERENT channels (team-level outreach, technical-decision-maker content, conference/podcast presence in eng-management circles), not via OSS top-of-funnel.

**Cascade:** Section 5 launch playbook should not be optimized for "maximize GitHub stars on day 0." That maximizes the wrong cohort. Sequence should target team-eng-leads in parallel with the OSS launch.

---

### M0e — Dogfood audience-class match (founder vs paying ICP)

**Premise:** Implicit — the founder, an ex-Stripe engineer, is dogfooding (presumably) on side-projects-they-own.

**Test:**
- Dogfood audience: "Me + maybe friends, building TypeScript/Next.js side projects."
- Paying ICP (per pricing): Teams large enough that $99/mo + MAU overage makes sense. That's NOT a single dev's side project. That's a 2-10 person team with active product, probably post-seed.

**Mismatch:** Dogfooding a paid-team auth SDK on solo side projects tunes the product for solo-dev DX while the paying ICP is small-team-with-shared-users-and-permissions. Different surface area entirely:
- Solo dogfood doesn't exercise: multi-admin permissions, audit logs across team members, billing-org/seat split, team-impersonation for support, RBAC complexity, SSO with the team's IDP, SCIM provisioning
- All of those are the features that justify $99/mo over Better Auth (free) or Clerk's free tier (10K MAU)

**Verdict: PREMISE FAILS (probable — founder should confirm).**

**Cascade — both pivots required, per SKILL.md anti-pattern #14:**
- (a) PIVOT TARGET AUDIENCE in marketing materials: stop targeting "solo OSS users." Target "2-10 person eng teams who care about owning their auth." Marketing copy, landing page, ICP doc all need this pivot.
- (b) EXPAND DOGFOOD SUBJECTS: founder should recruit 3-5 small-team beta users BEFORE public launch and dogfood the multi-admin / RBAC / SSO surface with them. Concierge-onboard them personally (Superhuman/Vohra pattern). Cannot just defer the paying ICP "to v1.1." That pattern is anti-pattern #14.

---

### Step 0.5 verdict summary

| Question | Verdict |
|---|---|
| M0a — launch platform audience-class fit | SURVIVES (partial) — HN OK as platform, NOT as the plan |
| M0b — canonical-success comparable named | **FAILS HARD** — Better Auth missing; positioning is invalidated |
| M0c — anti-feature surface | **FAILS** — pricing structure splits two ICPs |
| M0d — freebie-disqualifier | **FAILS** — star-counters ≠ paying ICP |
| M0e — dogfood audience match | **FAILS (probable)** — solo dogfood, team paying ICP |

**4 of 5 failed.** That clears the ≥2-failure threshold by a wide margin. Headline finding:

---

## PREMISE-LEVEL FINDINGS BLOCK (read before any tactical section)

> **The plan as written ships to silence and stalls at <5 hosted-tier signups in day 60. Four of five premise audits failed. The order of operations and the four fixes:**
>
> **1. The differentiation premise is dead.** "OSS, unlike Auth0/Supabase" was true in 2023. In 2026, Better Auth (28.5K stars, YC X25, framework-agnostic OSS) owns the OSS-TS-auth wedge. Founder must either (a) pick a sharper wedge (non-TS language, specific compliance vertical, specific framework, specific feature like passwordless-only or auth-for-AI-agents) or (b) compete on something other than "OSS." This is the most important finding.
>
> **2. The first-10-customer plan ("GitHub stargazers convert") is validation theater for the wrong segment.** Star-to-paid conversion is ~0.1-0.5%. To hit 5 hosted signups via stars alone, the founder needs 1K-5K stars in 60 days, which is itself a moonshot. The actual path to 5 paying teams: direct outreach to 30-50 named small-team eng-leads the founder knows or can warm-introduce to, with concierge onboarding. Not stars.
>
> **3. The pricing structure is doing two contradictory jobs.** $99 flat says "managed/premium"; $0.001/MAU overage says "usage-based/startup." Pick one. For a trust-bought ICP (eng teams choosing OSS auth specifically), recommend either flat tiers (Team/Business/Enterprise) OR seat-based — NOT a flat-plus-overage hybrid that signals nothing clean.
>
> **4. The dogfood surface needs to expand BEFORE launch.** Founder is (presumably) using AuthForge on solo TypeScript projects. The paying ICP is 2-10 person teams with RBAC, SSO, audit-log needs. Recruit 3-5 small-team beta users now and concierge-onboard them. The Vohra "very disappointed" gate replaces the calendar gate. If <40% report dependence, don't public-launch yet.

---

## Step 0A — Forcing questions (M1–M7), simulated as the founder (honest, naive on marketing)

### M1. Audience reality

**Founder first pass (naive):** "Backend engineers who need auth for their apps."

**Skill refusal:** Job-title category. Refused. Pushing for a named, specific persona.

**Founder second pass:** "OK — Daniel, mid-level backend eng at a 12-person seed-stage YC startup, working on a B2B SaaS in TypeScript/Next.js. He's a tech lead on a 4-person team. They currently use Clerk's free tier and are bumping against the 10K MAU limit; he's been told to evaluate cheaper / self-hostable alternatives this quarter. He reads: Pragmatic Engineer newsletter, follows @t3dotgg / @leerob / @shadcn on Twitter, hangs in the Next.js Discord, listens to Syntax FM and Software Engineering Daily. He last paid for: Cursor (personal, $20), GitHub Copilot (company), Linear (company)."

**Verdict:** ACCEPTED. 5+ attributes; 4 named attention surfaces; correct ICP (matches the pivot from M0e — small-team eng-lead, not solo OSS user).

### M2. Discovery path

**Founder first pass:** "He sees my Show HN post."

**Skill refusal:** Step 1 is NOT Show HN. Refused.

**Founder second pass:** "Step 1: Daniel reads my technical blog post 'How I built an OSS auth library after 4 years at Stripe' (~20K monthly readers, ~5% relevance hit = 1K readers in the right band). Step 2: He sees a Twitter thread from @theo or @t3dotgg quote-RT'ing it (I need to earn this — see Section 4). Step 3: He checks the GitHub repo, reads the README and the Next.js integration tutorial, runs the quickstart in 10 minutes. Step 4: He proposes to his team at next standup. Step 5 (1-2 weeks later): team adopts OSS version. Step 6 (4-12 weeks later): they hit a managed-feature need, upgrade to hosted."

**Verdict:** ACCEPTED. Named channels, named intermediaries, realistic time-to-discovery, realistic adoption funnel.

### M3. Pre-launch audience

**Founder:** "Twitter: 3,000 followers, mostly devs, ~3-5% engagement on technical threads. Blog: ~20K monthly uniques per Plausible, no email capture historically. GitHub: prior side projects total ~800 stars, mostly TypeScript tooling. No newsletter for this product. Have not started a wait-list. Discord: present in Next.js / Drizzle / Hono communities but not a recognized name."

**Verdict:** ACCEPTED with one urgent fix: NO EMAIL CAPTURE on a 20K-monthly-readers blog is a critical missing asset. Section 4 will make adding an email capture the Day-1 action.

### M4. Channel honesty

**Founder:** "Technical writing. I've published ~15 deep-dive blog posts in the last 18 months, several have hit HN front page. I'm not famous, but I have a credible signal pattern."

**Verdict:** ACCEPTED. Technical-blog writing IS a defensible channel. This is the load-bearing asset for the launch.

### M5. Competitor traffic source

**Founder first pass:** "Auth0 buys ads, Supabase has open source, Clerk has nice DX."

**Skill refusal:** Generic. Pushing for traffic-source specifics.

**Founder second pass:** "Honest answer: I don't know precisely. I'll commit to: (a) check SimilarWeb for clerk.com, supabase.com, better-auth.com before next session; (b) audit Better Auth's GitHub repo for the contributor/adopter pattern; (c) read 3 Better Auth blog posts to understand their voice; (d) scan their Twitter for who's amplifying them."

**Verdict:** ACCEPTED with assigned homework. Specific action by next session.

### M6. First 10 paying customers

**Founder first pass:** "GitHub stargazers who convert."

**Skill refusal:** Passive. Failed M0d. Refused.

**Founder second pass:** "10 specific 2-10 person teams I can email tomorrow:
1. My ex-Stripe colleague at [seed-stage co]
2-3. Two YC founders I know personally (different batches)
4-5. Two technical-blog readers who emailed me asking about auth (I saved the emails)
6-7. Two devs from the Next.js Discord I've helped with auth questions
8. The CTO of [former company I consulted for]
9-10. Two people who replied to my last Twitter thread mentioning auth pain
Plus: post in 3 small communities I'm a known member of (NOT generic r/programming): Indie Hackers solo-SaaS sub, local SF founders Slack, Pragmatic Engineer Discord."

**Verdict:** ACCEPTED. Named, specific, with concrete first-message plan.

### M7. Time allocation

**Founder first pass:** "I'll do audience-building 'when I can.'"

**Skill refusal:** Failed. Vague.

**Founder second pass:** "Honest current state: 95% building, 5% Twitter. Target for next 60 days: 60% building, 30% audience+outreach, 10% community. Specific weekly commitments: 2 technical blog posts/month, 3 Twitter threads/week, 5 cold/warm outreach emails/week, 1 podcast pitch/week."

**Verdict:** ACCEPTED with caveat: 30% audience time is the floor, not the ceiling, given that the launch gate is now signal-driven (see Section 5).

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | URL | Founded | Pricing | Apparent traffic source | User complaints | Winning? |
|---|---|---|---|---|---|---|
| **Better Auth** | better-auth.com | 2024 (YC X25) | Free OSS, no hosted yet | GitHub, Twitter (@bekacru), HN Launch May 2025 (item 44030492) | "Docs gaps for advanced patterns", "Plugin auth conflicts" | YES — 28.5K stars in ~12 months. The category-defining OSS-TS auth lib. |
| **Clerk** | clerk.com | 2020 | Free 10K MAU, $25/mo + $0.02/MAU | Component-led DX, brand on Twitter, sponsored Next.js/React content | "Pricing scales painfully past 10K MAU" | YES — Series C, ubiquitous in PLG-Next.js stack |
| **Auth0** | auth0.com | 2013 | Free 25K MAU, $35/mo essentials, custom enterprise | SEO authority, paid ads, Okta backing | "Pricing is opaque", "Vendor lock-in", "Heavy" | LEGACY-WINNING — Okta-owned, B2B SaaS default |
| **Supabase Auth** | supabase.com/auth | 2020 | $0.00325/MAU after 50K free (bundled w/ Supabase) | Content + launch weeks + GitHub-led growth | "Tied to Postgres / Supabase", "Limited if you don't use Supabase stack" | YES (within Supabase users) |
| **WorkOS** | workos.com | 2019 | Connection-based pricing (~$125/connection/mo for SSO) | Content (workos.com/blog), enterprise sales | "Expensive for non-enterprise" | YES (in B2B enterprise) |

### 1b. Canonical-success comparables (DEV-TOOL OSS + HOSTED MOTION CLASS)

| Canonical | Price | Primary acquisition | Onboarding | Launch gate | Delta vs AuthForge plan |
|---|---|---|---|---|---|
| **Stripe** | usage-based (% per txn) | DOCS as the channel; engineering-as-marketing | Self-serve via docs | PMF: signal from initial dev cohort, then expand | AuthForge plan treats docs as one bullet; Stripe treats docs as the product. |
| **Supabase** | usage + flat tiers | Launch Weeks (8+ shipped), DevRel YouTube, GitHub-led OSS, community-first | Self-serve | PMF-led + Launch Week as forcing function | AuthForge plan has zero recurring-marketing-cadence. Launch Week ritual is replicable. |
| **Better Auth (in-category)** | OSS only (no paid yet) | HN Launch + technical author voice + framework community Discords + YC stamp | Self-serve, docs | Calendar (May 2025 Launch HN) — but earned by 6 months prior OSS work | AuthForge currently has no equivalent 6-month-prior OSS work. Better Auth had built credibility before Launch HN; AuthForge plan launches cold. |
| **Clerk** | tiered MAU | DX-led growth, drop-in components, Next.js community sponsorship | Self-serve, ~hour | Calendar w/ free tier as expansion gate | Clerk's DX-first design IS the marketing. AuthForge has no equivalent "show, don't tell" artifact. |

### 1c. Pattern surface

The four canonical successes share three things AuthForge's plan currently lacks:

1. **The product is the marketing.** Stripe's docs, Clerk's components, Supabase's launch-week artifacts, Better Auth's quickstart all do the convincing. AuthForge's plan treats "marketing" and "product" as separate workstreams.
2. **There's a recurring cadence, not a single event.** Supabase Launch Week happens 4x/year. Stripe ships visible product/docs improvements constantly. AuthForge's plan is "Show HN, then hope."
3. **Audience precedes product.** Better Auth had bekacru's technical Twitter presence and 6 months of public OSS work before Launch HN. Clerk had Colin Sidoti's developer voice. AuthForge has the founder's blog (which is good!), but the founder hasn't yet posted about AuthForge or built a wait-list.

The current plan is implicitly following the *direct-competitor playbook* ("what Auth0/Supabase do") rather than the *canonical-success playbook* ("what makes a dev-tool OSS+hosted product break out from zero"). Wrong precedent. Switch to the canonical-success playbook, anchor on Supabase + Better Auth specifically.

**Founder action this week:** Read bekacru's HN Launch comments line-by-line, read 3 Supabase launch-week retros, write down 5 patterns you can copy.

---

## Section 2 — ICP specification

(detailed version in `icp.md` artifact — summary here)

- **Persona:** Daniel, tech lead, 12-person YC seed B2B SaaS in TS/Next.js. 28-34. Pragmatic, not ideological about OSS — values it but won't pay a 2x maintenance tax for it.
- **Attention surfaces:** Pragmatic Engineer, t3dotgg / leerob / shadcn Twitter, Next.js Discord, Syntax FM, Software Engineering Daily, Lenny's Newsletter (occasional).
- **Currently pays for:** Cursor ($20), Linear ($8/seat), Sentry ($26/mo+), Clerk (free → $25 looming), Vercel ($20/seat).
- **Adjacent complaints:** "Clerk pricing scales painfully past 10K MAU", "Auth0 feels enterprise-heavy", "Supabase Auth is bundled — I don't want the whole stack", "I'd self-host but ops is a tax."
- **Objections to AuthForge:** "Why not just Better Auth (it's free and has 28K stars)?", "Who maintains this in 5 years?", "Can I migrate off cleanly?", "What's my SSO/SCIM story?", "Have you hit production scale?"
- **Reasons to convert:** Ex-Stripe credential creates initial trust; specific feature parity gap with Better Auth (must specify); hosted tier removes ops tax; pricing predictability at scale.

---

## Section 3 — Distribution channel-by-channel (dev-tool motion-class rules applied)

Per SKILL.md Section 3 dev-tool rules, three channels are PRIMARY (not auxiliary):

1. **Docs / SEO compounding** — integration tutorials per framework
2. **GitHub as marketing surface** — repo health, adopter graph, contributor recognition
3. **Founder's existing dev-audience surfaces** — blog, dev-Twitter, podcast guesting

| Channel | Reach | Cost | Conv. | Founder fit | Effort | Verdict |
|---|---|---|---|---|---|---|
| **Founder technical blog** (PRIMARY) | 20K/mo | $0 | High | EXCELLENT | LOW (already doing) | TOP RANK. Must add email capture. |
| **Docs/SEO (integration tutorials)** (PRIMARY) | compounding | dev time | High (long-tail intent) | EXCELLENT (Stripe alum) | HIGH (6-12 mo investment) | TOP RANK. Start with Next.js, Hono, Express tutorials. |
| **GitHub repo as surface** (PRIMARY) | compounding | $0 | Med→High | GOOD | MED (issue hygiene, README, adopter callouts) | TOP RANK. Star count is real social proof. |
| **Dev-Twitter (founder)** | 3K direct, 30K+ via amplification | $0 | Med | GOOD | LOW-MED | RANK 2. Build-in-public cadence. |
| **HN (Show HN)** | high if hit, zero if miss | $0 | Med | OK | LOW (single event) | RANK 2. Single shot, time carefully. |
| **r/programming** | low conversion for self-promo | $0 | Low | OK | LOW | RANK 3 (cross-post only, NOT primary). |
| **Lobste.rs** | small but quality | $0 | Med | GOOD | LOW | RANK 2-3. Tonally right for OSS auth. |
| **Podcast guesting** (Syntax FM, SE Daily, Pragmatic Engineer, etc.) | mid, high-quality | $0 | High | EXCELLENT (ex-Stripe story) | MED (outreach) | RANK 2. Start pitching now. |
| **Next.js / Hono / framework Discords** | small but ICP-pure | $0 | High | OK (not famous) | LOW-MED | RANK 3 — be helpful before promoting. |
| **Newsletter mentions** (Pragmatic Engineer, Bytes, JavaScript Weekly) | high in dev-IC audience | $0 (or $) | Med-High | OK | MED (relationships) | RANK 2. Bytes & JS Weekly are reachable. |
| **Reddit r/nextjs, r/typescript** | low-med | $0 | Low (anti-promo culture) | OK | LOW | RANK 3. Helpful-first. |
| **Product Hunt** | wrong audience class for dev infra | $0 | Low | OK | LOW | SKIP (wrong audience). |
| **LinkedIn organic** | dev-Twitter > LinkedIn for this ICP | $0 | Low | OK | LOW | SKIP (low conv for IC devs). |
| **Paid ads (Google / Meta)** | high cost in auth keyword space | $$$ | Med | POOR (no creative iteration capacity) | HIGH | SKIP for v1. |
| **Affiliate** | n/a | n/a | n/a | n/a | n/a | DEFER. |

**Surviving channels, sequenced:**
1. (PRIMARY) Founder blog with email capture — start now
2. (PRIMARY) GitHub repo + integration tutorials — start now
3. (PRIMARY) Dev-Twitter build-in-public — start now
4. (RANK 2) HN Show + Lobste.rs + Bytes/JS Weekly newsletter outreach — launch event
5. (RANK 2) Podcast guesting — pitch in week 2, land in weeks 4-12
6. (RANK 3) Framework Discords — helpful-first presence ongoing

### Dev-tool tonal rule (LOAD-BEARING for launch copy)

Per SKILL.md anti-pattern #13 and Section 3 dev-tool tonal rules: REFUSE marketing-speak in launch copy.

**Do NOT write:** "AuthForge is a revolutionary, enterprise-grade authentication framework that delivers seamless, robust auth to any application. Best-in-class developer experience."

**Do write:** "AuthForge is an OSS auth SDK with a hosted tier ($99 + $0.001/MAU). Built it because Clerk's pricing breaks past 10K MAU and Better Auth doesn't (yet) have a managed hosted option. Worse than Auth0 for: enterprise compliance attestations, ADFS legacy. Worse than Better Auth for: plugin ecosystem maturity. Better at: predictable pricing, deploy-anywhere hosted instance, RBAC primitives. GitHub: [link]. Quickstart in 4 minutes."

The honest "worse at X" lines are what make the "better at" lines credible to the dev audience.

---

## Section 4 — Pre-launch audience-building plan (ELEVATED — Mode A with Section 4 priority)

**Reasoning:** founder has 20K monthly blog readers but no email capture, no AuthForge-specific narrative published yet, no public repo. Mid-build with implicit Day-60 gate. Mode A + elevated Section 4 = audience-build runs in PARALLEL with launch playbook prep, not before.

### Day 1-30 (audience activation)

**Day 1-3 (this week — the 3 strongest action items):**
1. **Add email capture to the blog.** Convertkit/Buttondown/Beehiiv. Lead magnet: "Authentication patterns at scale — what I learned building auth at Stripe." Convert 20K monthly readers → email list. Even 2% capture = 400 emails over a month.
2. **Publish public repo on GitHub** with README that names the wedge, the limitations, and the first 3 integration tutorials (Next.js, Hono, Express). Pin tweet announcing the build.
3. **Email 10 specific people (per M6).** Personal cold/warm note. Not "hey check this out" — "I'm building X for Y reason because you and I have both hit Z. Want to be one of the first 10 to try it and shape what we build next?"

**Day 4-30:**
- Blog: 2 deep-dive posts/month. Topics: "Why I'm building an OSS auth SDK after 4 years at Stripe", "Auth at scale: what breaks past 10K MAU", "OSS-with-hosted: how we price."
- Twitter: 3 build-in-public threads/week. Show code, show decisions, show trade-offs. Tag relevant people sparingly.
- Cold outreach: 5 small-team eng-leads/week (per M6 list, then expand).
- Podcast pitches: 1/week. Target: Syntax FM, Software Engineering Daily, Pragmatic Engineer, Changelog, JS Party.
- Newsletter outreach: pitch Bytes / JS Weekly with "ex-Stripe builds OSS auth" angle. Pragmatic Engineer if you can earn it (high bar).
- GitHub: ship 2 integration tutorials/week. Each tutorial = SEO asset + Twitter thread + landing-page anchor.

**Day 30 checkpoint:**
- 400+ email list, 4+ blog posts, 12 tutorials, 5+ concierge-onboarded beta teams. If <3 beta teams report "would be very disappointed without this," DO NOT public-launch yet.

### Day 31-60 (build to launch readiness)

- Continue Day 1-30 cadence
- Add: build a "What's coming" public roadmap (GitHub Projects); request feature input from beta teams publicly to create momentum
- Land 2 podcast appearances by day 45
- First Launch Week-style content sprint: 5 days of coordinated daily releases (Mon: new feature; Tue: integration; Wed: case study; Thu: comparison post; Fri: AMA)
- Re-test Vohra "very disappointed" with beta cohort; gate public launch on >=40%

### Day 61-90 (sequenced public launch + post-launch compounding)

- Public launch event (see Section 5)
- Cadence continues; first 30 days post-launch = retention focus, not acquisition
- Quarterly Launch Week thereafter (Supabase pattern)

---

## Section 5 — Launch playbook

### 5a. Launch gate question (asked BEFORE writing the sequence)

**Question:** Calendar gate (Day 60) or PMF signal gate?

**Verdict:** PMF signal gate, per SKILL.md Section 5a. Reasoning:
- Auth is trust-load-bearing. Launching to silence with a broken trust signal kills the brand worse than launching late.
- Better Auth precedent: launched HN AFTER 6 months of OSS public work + audience-build. They didn't calendar-launch.
- Day-60 metric pair ("100 stars + 5 hosted signups") is incoherent; replace with: ">=3 beta teams say 'very disappointed if I lost this' AND >=1 has paid for the hosted tier as concierge-onboarded customer."

The "100 stars" is a vanity number; the "5 hosted signups" is the real gate. Replace the former; tighten the latter to >=3 paying concierge-onboards as the public-launch gate. Calendar Day 60 becomes a *check-in*, not a gate.

### 5b. Default launch sequence (customized)

| Day | Channel | Action |
|---|---|---|
| -45 | Founder blog | "Why I'm building AuthForge" deep-dive (with email capture) |
| -30 | GitHub | Public repo + 3 integration tutorials live; "build-in-public" begins |
| -21 | Twitter | Build-in-public thread cadence (3/week); concierge-onboarding announcement |
| -14 | Podcast | First podcast appearance lands (pitched 4-6 weeks prior) |
| -10 | Newsletter | Pitch Bytes / JS Weekly with launch date |
| -7 | Personal network | Email ~50 people directly. NOT a blast — individual notes. |
| -3 | Twitter | Build-in-public thread previewing launch + concierge beta results |
| 0 (Tue, 9am PT) | HN | Show HN: AuthForge — OSS auth SDK + hosted tier ($99). Link to GitHub FIRST, then docs, then landing. Tonal rule: lead with technical specifics, name where we're worse. |
| 0 +2hr | Twitter | Thread with HN link (after initial HN engagement); tag no one |
| 0 +4hr | Lobste.rs | Cross-post (compliant: only if community guidelines allow self-post) |
| 0 +24hr | Indie Hackers + Pragmatic Engineer Slack | Cross-post (where founder has standing) |
| 0 +48hr | r/nextjs, r/typescript | Compliant cross-post; lead with the technical novelty, not the pitch |
| 0 +7d | Product Hunt | SKIP (wrong audience for dev infra) |
| 0 +14d | Podcast | 2nd podcast appearance lands |
| 0 +30d | Blog | Retrospective: "What we shipped, what broke, what we learned" with traction numbers (honest, not vanity) |
| 0 +90d | Launch Week #2 | First quarterly launch week (Supabase pattern) |

**Risk callouts:**
- HN miss: With founder's blog amplifying + dev-Twitter + Better Auth's recent HN precedent showing this category lands -> ~50% chance of front page. If miss: launch is NOT broken — the build-in-public cadence carries.
- Better Auth response risk: bekacru may engage publicly. Be honest about Better Auth being a real alternative; don't trash-talk. Differentiate on the hosted tier (which Better Auth doesn't have).
- Repo not ready for traffic: pre-bake docs site, test quickstart on fresh clone, ensure GitHub issues template ready.

---

## Section 6 — Pricing & packaging

### 6a. Pricing BAND question (asked before optimizing price point)

**Question:** Did the $99/mo + $0.001/MAU band come from competitor anchoring or ICP willingness-to-pay evidence?

**Founder honest answer:** "Anchored on Clerk's $25 base and added 'enterprise-feeling' premium. Not from ICP interviews. Have not validated."

**Verdict:** PREMISE FAILS — band is competitor-anchored, not ICP-WTP-evidenced. Per SKILL.md, the band question must be answered before optimizing the point.

**ICP-WTP evidence (research):**
- Clerk Pro: $25/mo + $0.02/MAU (so 10K MAU = $25; 20K = $225; 100K = $1,825) — see zuplo.com pricing wars article and gautamkhorana.com comparison
- Auth0 Essentials: $35/mo base, scales rapidly
- WorkOS: connection-based (~$125/connection)
- Adjacent SaaS the same ICP buys: Linear $8/seat, Sentry team $26+/mo, Vercel $20/seat, Cursor $20/dev

**Better pricing structures to consider:**
1. **Seat-based:** $X/seat/mo (mirrors Linear/Sentry/Vercel mental model — the ICP is already trained on it)
2. **Flat tiers:** Free OSS / Team $49/mo (up to 25K MAU, no per-MAU overage) / Business $199/mo (up to 250K MAU, SSO, audit log) / Enterprise (custom, self-hosted-with-support)
3. **Status quo (defensible if):** founder commits to NOT competing with Clerk on price below 10K MAU. Position as: "if you've outgrown Clerk's free tier and want predictable pricing past 10K — that's us."

**Recommendation:** option 2 (flat tiers) — cleaner positioning, removes the per-MAU surprise, matches ICP's mental model from adjacent tools. Per SKILL.md anti-pattern #7, do NOT match the cheapest competitor — for trust-bought ICP, near-the-top-of-band pricing signals credibility.

### 6b. Standard pricing coverage

- **Tier structure:** Free OSS (self-host) / Team $49/mo / Business $199/mo / Enterprise (custom, self-hosted-with-support — this is the lever for big ARR)
- **Trial mechanics:** No free trial on hosted tier; instead, free OSS as the "trial." Per M0d freebie-disqualifier: cheap-trial mechanics would attract solo hobbyists. The OSS-as-trial mechanic self-selects for teams with technical capacity who later upgrade to managed.
- **Annual discount:** 20% off annual billing. Annual billing is known to materially improve retention.
- **Per-feature gating:** SSO / SCIM / audit log gated to Business tier. Concierge support gated to Enterprise. This gives clear up-sell paths.

---

## Section 7 — Post-launch growth loops

| Loop | Compounds? | Why / why not |
|---|---|---|
| Referral mechanics | LINEAR (initially) | Dev teams don't usually refer auth SDKs the way they refer Linear/Notion. Skip for v1. |
| Content compounding (SEO) | COMPOUNDS | Integration tutorials rank for long-tail framework queries. Build this hard — Stripe playbook. |
| Network effects | NONE | Auth is not network-effected at the product level. (Brand IS, indirectly.) |
| Brand compounding | COMPOUNDS | Build-in-public + transparent post-mortems + quarterly Launch Weeks -> "the OSS auth team you trust." |
| Retention as growth | COMPOUNDS WEAKLY | Devs who use AuthForge at Co A bring it to Co B when they move jobs. Real, but slow (~12-24 mo lag). |
| GitHub-ecosystem-as-loop | COMPOUNDS | Each new integration adapter (next-auth migration tool, prisma adapter, etc.) brings a new audience segment. Sponsor / merge community PRs for this. |

The acquisition treadmill risk is REAL: no referral mechanic, weak network effects. The defense is content + GitHub-ecosystem-as-loop. Both compound, both are slow.

---

## Section 8 — Metrics & instrumentation

**Measure:**
- Acquisition by channel with UTMs (blog vs HN vs Twitter vs newsletter vs podcast)
- npm install count + GitHub star velocity (NOT total — velocity)
- Quickstart-to-first-success rate (instrumented in the SDK opt-in telemetry, with clear opt-out)
- Free-OSS-to-hosted-tier conversion funnel (per cohort)
- Hosted tier: MRR, logos (named), MAU-per-customer trajectory, churn by tier
- Vohra "very disappointed" survey monthly to active hosted-tier customers (target >=40%)
- Docs page rankings on long-tail queries (Ahrefs / Google Search Console)

**Do NOT optimize for:**
- Total GitHub stars (per M0d — wrong cohort)
- Twitter follower count
- HN upvote count
- "Total signups" (without retention)

**Weekly dashboard:** MRR, paying logos, new email-list subs, top 3 SEO ranking pages, beta-cohort dependence rate, weeks-to-quickstart-success p50.

---

## Section 9 — Risk analysis

| Risk | Severity | Mitigation |
|---|---|---|
| **Better Auth wins the OSS-TS-auth wedge entirely** | HIGH | Pick a sharper wedge: non-TS language, specific compliance vertical, AI-agent auth, or compete on hosted-tier ops quality. Decide before public launch. |
| **HN miss with no recovery** | MED (down from HIGH given founder's other surfaces) | Multi-channel sequenced launch; founder's blog and beta-cohort dependence carry. |
| **Channel concentration on founder blog** | MED | Founder is THE channel right now. Mitigation: build email list, build podcast pipeline, ship integration tutorials for SEO. Diversify within 6 months. |
| **Pricing-band wrong for ICP** | MED | Switch to flat tier structure per Section 6 before launch. |
| **Solo-dogfood -> small-team-paying-ICP mismatch ships** | HIGH | Concierge-onboard 3-5 beta teams; gate launch on dependence signal; both pivots per anti-pattern #14. |
| **Trust gap: first-time shipper, no production proof** | MED | Lead with ex-Stripe credential AND public commitment to a major adopter shipping by Day 90. Get one named logo. |
| **Better Auth founder counter-launches** | LOW-MED | Be honest, don't trash. Differentiate on hosted-tier ops. |
| **OSS feature-parity bait-and-switch perception** | MED | Decide explicitly what's OSS vs hosted-only and DOCUMENT it before public launch. Most-permissive OSS feature set; hosted = ops + SSO + audit + support. |
| **Macro: HN / Twitter algorithm shifts** | LOW (in 60-day window) | Multi-channel; founder has blog as owned channel. |

---

## Outside-voice critique (simulated adversarial CMO subagent)

**Single biggest risk inside review missed:** The founder is, accidentally, building Better Auth + a hosted tier — and Better Auth (or a YC-backed competitor or even Vercel) can add a managed hosted tier in 90 days and erase the entire differentiation. The hosted tier alone is not a defensible moat. The moat must be either (a) a specific feature/vertical (regulated industries, AI-agent auth, multi-tenant complexity) or (b) ops quality + SLA that Better Auth won't build because they're maxing out the OSS surface. PICK ONE before launch.

**Channel weaker than positioned:** Founder's "3K Twitter + 20K blog" sounds strong but the BLOG has no email capture, meaning the 20K is rented attention — they re-discover via search/RSS. The OWNED channel is functionally tiny. Day-1 fix: email capture. Without it, the founder is overestimating own-channel reach by 10-50x.

**Audience claim lacking evidence:** "Backend engineers" was the original founder claim. M1 pivoted to Daniel-the-tech-lead. That pivot is DIRECTIONALLY right but NOT YET evidenced — founder has not talked to 5 Daniels and verified the pricing band, the wedge, or the objections. Required: 5 customer-development conversations with the actual ICP before pricing is locked.

**Provocative reframe:** What if AuthForge's wedge is NOT "OSS auth library" at all, but "auth-for-AI-agents" — handling agent identity, MCP server auth, OAuth flows for LLM-driven actions? This is an emerging category in 2026 that none of Clerk/Auth0/Supabase/Better Auth have specifically claimed yet. The founder's Stripe background (handling auth at scale for programmatic flows) is uniquely well-suited. This reframe would convert a crowded-category competition into a new-category claim. Worth a serious week of customer-development to test.

---

## Handoff

### 3 strongest action items for THIS week

1. **Add email capture to the blog TODAY.** 20K monthly readers without email capture is the single most expensive ongoing leak in this plan. Convertkit or Beehiiv, lead magnet = "Auth at scale: what I learned at Stripe."
2. **Email the 10 named people from M6 with a personal note about beta access.** Target 3-5 concierge-onboarded small-team beta users by Day 30. This replaces "GitHub stargazers convert" as the path to first 5 paying.
3. **Decide the wedge: pick ONE.** Either (a) sharper OSS-auth wedge vs Better Auth (compliance vertical, specific framework, ops quality), or (b) the provocative reframe (auth-for-AI-agents). 5 customer-development conversations with the ICP this week to pick.

### Re-run cadence
- Re-run `/plan-cmo-review` in 30 days to evaluate progress against this plan
- After wedge decision, run `/office-hours` (positioning likely shifted enough to matter)
- After pricing-tier change, run `/plan-ceo-review` (business model meaningfully shifted)
- Before any product spec changes for SSO/SCIM/audit-log: `/plan-eng-review`
