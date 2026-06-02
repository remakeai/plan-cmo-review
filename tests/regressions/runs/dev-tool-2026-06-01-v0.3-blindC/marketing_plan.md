# AuthForge — Marketing Plan (CMO Review)

**Date:** 2026-06-01
**Skill version:** plan-cmo-review v0.3.0
**Mode:** Mode A (Full Marketing Review) — see Step 0B
**Founder default:** Marketing-naive (technical, first-time-at-marketing). Modified DOWNWARD only modestly: founder has 3K dev-Twitter followers + ~20K monthly blog readers (both ICP-aligned), but **no shipped product**. Per skill criteria, "demonstrated marketing track record" requires shipped traction; the founder has audience but no conversion-to-product evidence. Default holds with caveat: existing dev audience is a real advantage and Section 4 audience-build sprint is partially pre-paid, but tactical premise audit remains load-bearing.

---

## Step 0 — Pre-review system audit

### What the design doc gives us

- **Product:** "AuthForge" — open-source authentication SDK (MIT) + hosted tier ($99/mo managed instance, $0.001/MAU above 10K)
- **Target user:** backend engineers building auth into their apps
- **Distribution plan:** "Show HN at launch + post on r/programming + write integration tutorials"
- **First 10 customers:** "GitHub stargazers who upgrade to hosted tier"
- **Validation gate:** 100 GitHub stars + 5 hosted-tier signups by day 60
- **Differentiation:** "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)"
- **Founder:** ex-Stripe engineer, 3K Twitter followers, technical blog with ~20K monthly readers, no prior shipped products

### Founder audience audit (existing distribution surface area)

| Surface | Count | ICP-alignment | Notes |
|---|---|---|---|
| Twitter / X | 3,000 | HIGH (dev-Twitter) | Strong fit; backend devs follow ex-Stripe engineers |
| Technical blog | ~20,000 monthly readers | HIGH | Largest asset; pre-built developer audience that already trusts technical voice |
| Newsletter | unstated | unknown | Critical gap — is there an email capture on the blog? Will ask in M3 |
| LinkedIn | unstated | unknown | Likely partial; ex-Stripe alumni network is high-value |
| GitHub stars on prior projects | none stated | n/a | First shipped product |
| Discord / Slack community presence | unstated | unknown | Need to check |
| Ex-Stripe alumni network | implicit | HIGH | Stripe alumni are concentrated buyers + influencers in dev infra |

**Read:** This founder is in the top decile of dev-tool launchers for pre-built audience. 20K monthly blog readers is roughly equivalent to a mid-size dev newsletter (Pragmatic Engineer is ~700K, but most dev newsletters under 50K). The 3K Twitter following is small-but-ICP-perfect.

**Load-bearing implication:** The audience advantage means Mode A (full plan) is correct, NOT Mode C (audience-build sprint). However, the founder almost certainly does NOT have an email capture / newsletter sign-up on the blog — converting blog readers to direct-relationship subscribers before launch is THE highest-leverage pre-launch action available, and it is invisible from the design doc.

### Web-searched competitive landscape (preview — full version in Section 1)

Direct competitors identified:
- **Auth0** (Okta) — incumbent, $0.07/MAU after free tier, mature, enterprise-focused
- **Clerk** — Next.js darling, $25/mo + $0.02/MAU after 10K free, best DX scoring
- **Supabase Auth** — bundled with Supabase, $0.00325/MAU after 50K free, open-source-but-restricted self-host
- **WorkOS** — B2B SSO-first, enterprise-IT buyer
- **SuperTokens** — OSS competitor, ~12K GitHub stars, YC-backed, Apache 2.0
- **Better Auth** — emerging OSS leader; absorbed Auth.js maintainership Sept 2025; the default new pick for self-hosted Next.js in 2026
- **Kinde** — B2B-focused, aggressive bundle pricing ($25/mo for orgs+roles+MFA+flags+social)
- **FusionAuth** — mature feature-set OSS
- **Hanko** — passkey-first OSS (AGPL v3)
- **Stack Auth** — Next.js-native OSS, closest drop-in to Better Auth

[Sources captured in Section 1.]

**Critical finding from competitor scan:** Better Auth as a category leader is missing from the founder's stated differentiation list. The founder positions against Auth0 and Supabase Auth — both of which are the WRONG comparables in 2026 for a new OSS auth SDK. Better Auth is the live, ascendant OSS competitor that took over Auth.js maintainership in Sept 2025. **If AuthForge launches with positioning that doesn't address Better Auth, evaluators will see it as out-of-date by day one.**

---

## Step 0.5 — Premise audit (M0a–M0e)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| P1 | Show HN + r/programming are the primary launch channels | "Distribution Plan" | Right audience class for dev tools, BUT single-pulse strategy with no recovery. Insufficient as a *plan*. |
| P2 | GitHub stargazers will convert to hosted tier ($99/mo) | "First 10 customers" | Stargazers are evaluators, not buyers. Star-to-paid conversion in OSS+hosted is documented at 0.3-1% for mass-market; closer to 1-3% only with deep activation work. |
| P3 | $99/mo flat hosted tier is the right price point | "Distribution model" | Anchored on what feels reasonable, not on ICP willingness-to-pay. Clerk is $25/mo + per-MAU; Auth0 enterprise is $10K+; the $99 flat sits in a no-man's land. |
| P4 | "Simpler than Auth0, more flexible than Supabase Auth" is the positioning | "Differentiation" | Anchored against 2020-era competitors. Better Auth, Clerk, SuperTokens are the actual 2026 competitive field; this positioning skips them. |
| P5 | 100 GitHub stars + 5 hosted signups by day 60 is the validation gate | "Validation gate" | Mixed-axis metric: 100 stars is achievable on launch day alone; 5 hosted signups is the harder gate but is vague (any signups vs paying signups). Stars-as-vanity-metric risk. |
| P6 | "Write integration tutorials" is sufficient content strategy | "Distribution Plan" | Vague. Stripe-style integration tutorials are a multi-month investment with specific framework targeting. "Write tutorials" without per-framework prioritization is a TODO, not a plan. |
| P7 | The product can be dogfooded by the founder alone (implicit) | n/a (absent) | Founder is ex-Stripe — auth experience is real, BUT solo dogfood of an auth library doesn't surface the polyfill / framework-edge / SSO / migration pain that real integrators hit. Risk of shipping a library that "works for me." |

### M0a. Launch-platform audience-class fit

**Question:** Is Show HN + r/programming the right audience class for an open-source auth SDK?

**Verdict: PREMISE SURVIVES with sequencing caveat.**

Web search confirms: Show HN is the canonical audience-class match for OSS dev tools. Per Daniel King's 188K-post Show HN dataset, dev-tool / library posts get the strongest organic lift on HN of any category. Better Auth, SuperTokens, Hanko, Stack Auth all gained early stars from HN. The dev-tool tonal rule applies (no marketing-speak; lead with code; see Section 5).

**But the single-pulse risk is real:** the same dataset shows median Show HN gives 121 stars at 24h, 289 at one week, then flatlines unless the project has a flywheel. A single Show HN post with no surrounding plan is a one-day pulse, not a launch. The premise survives at the *audience-class* level but fails at the *plan-completeness* level.

Cascading implication: Section 5 keeps Show HN as a centerpiece but rejects "Show HN as the launch." Sequence Show HN inside a multi-channel pulse.

### M0b. Canonical-success comparable

**Question:** Name the canonical-success product in this category at this motion class. What did they do that AuthForge does NOT?

**Verdict: PREMISE FAILS.** The design doc names no canonical-success precedent. It anchors against direct competitors (Auth0, Supabase) only.

The canonical successes for **OSS dev tool + hosted tier (open-core)** motion class:

1. **Stripe** (not OSS, but the canonical developer-first infrastructure success). Playbook: docs as marketing, integration tutorials per framework, "engineering as marketing," founder writing (Patrick Collison long-form). Reportedly drove the bulk of early SEO + word-of-mouth. **AuthForge has the founder profile to attempt the Stripe-style writing play — ex-Stripe employee, has 20K blog readers, has the technical voice. This is the highest-leverage parallel and the design doc misses it.**

2. **SuperTokens** (direct competitor AND canonical success in OSS auth). 12K+ stars, YC-backed, Apache 2.0. Playbook: positioning as Auth0/Firebase/Cognito alternative; transparent feature-comparison charts (including admitting where they LOSE); content marketing on framework-specific guides (React, Express); Discord + GitHub community as primary surfaces. **The transparent "we lose at X" comparison chart is a load-bearing trust move that AuthForge should copy. Founder-default is to claim wins; SuperTokens documents losses, which is what builds dev trust.**

3. **Better Auth** (direct competitor AND the live 2026 OSS auth story). Grew rapidly enough to absorb Auth.js / NextAuth.js maintainership in Sept 2025 — meaning the legacy community migration funnel is being captured by Better Auth, NOT by AuthForge. Playbook: code-first integration, Next.js-native default, immediate session revocation, full ownership positioning. **AuthForge cannot ignore Better Auth and cannot out-Next.js Better Auth; positioning must orient explicitly against it.**

4. **Postiz / Papermark** (open-core SaaS at the scale AuthForge is targeting). Postiz scaled to $17K MRR; Papermark to $75K MRR ($900K ARR) in 18 months via open-core. Playbook: OSS-as-marketing-distribution-channel; the GitHub repo is the top-of-funnel; the hosted tier is the monetization layer. **Documented hosted-tier conversion rate: 0.3-3% of OSS adopters convert. AuthForge's validation gate (5 hosted signups from 100 stars = 5%) is aggressive against the documented base rate.**

5. **Vercel** (canonical dev-tool open-core success). OSS Next.js → Vercel hosted. Playbook: framework authorship as marketing — being the maintainer of the layer underneath gives you definitional power.

**Deltas AuthForge does not yet have:**
- No specific framework-tutorial sequence (Stripe playbook missing)
- No transparent "where we lose" comparison chart (SuperTokens playbook missing)
- No explicit Better Auth positioning (competitive blindness)
- No conversion-rate baseline applied to validation gate (math error)
- No clear "what's the wedge" — "simpler than Auth0" is a tagline, not a wedge

### M0c. Anti-feature surface

**Question:** Name 2+ features in scope that contradict the stated positioning, trust model, or business model.

The design doc does not enumerate features beyond "open-source SDK" and "hosted tier." So this question is forward-looking: what features WILL be in scope, and which will contradict positioning?

**Likely anti-features the founder will be tempted to ship in v1 (based on technical-founder patterns):**

1. **Full SSO / SAML / SCIM in v1.** Founder will be tempted to include because "enterprises need it." But: SSO/SAML/SCIM is the WorkOS positioning. Including it dilutes "simpler than Auth0" — the SAML protocol is the largest single source of complexity in auth. Decision owed: defer SSO to v2 / enterprise tier OR rebrand as "complete auth incl. SSO" (and lose simplicity wedge). **Cannot have both.**

2. **BYO-database adapters for every database under the sun.** Founder will be tempted to support Postgres, MySQL, SQLite, MongoDB, DynamoDB, FaunaDB, etc. because "developers want flexibility." Each adapter is its own maintenance burden and signals "infrastructure project" rather than "fast auth library." Better Auth and Clerk both started narrow (Postgres-first or no-DB-required) and expanded.

3. **Full admin dashboard UI as part of the OSS package.** Tempting because "developers want a UI." But: admin UIs are the hosted-tier differentiator in open-core. If you ship the dashboard in OSS, you cannibalize the hosted tier. Clerk's dashboard is hosted-only; Supabase's full studio is hosted-only.

4. **A "headless mode" AND a "drop-in UI components" mode in v1.** Two product stories at once. Clerk picked drop-in components and won DX; Better Auth picked headless and won flexibility. Picking both means picking neither.

**Verdict: PREMISE FAILS by anticipation.** The feature list is not yet enumerated, but the four temptations above are near-certain based on the founder's likely instincts. Need a line-by-line feature list AND a decision on each before scope is locked.

### M0d. Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the planned acquisition mechanic (OSS download + free GitHub starring + $99 hosted tier) select for the wrong segment?

**Verdict: PREMISE FAILS — partially.**

The OSS-as-acquisition + hosted-as-monetization motion is well-validated (Postiz, Papermark, Vercel, SuperTokens). But the *paying* segment for $99/mo managed auth is NOT the same human as the "starred your repo on HN" cohort.

Selection bias mapping:
- **OSS download + GitHub star** → hobbyists, evaluators, ICs prototyping a side project. Time-rich, money-poor. Will NEVER pay $99/mo because they self-host.
- **$99/mo hosted tier** → small teams / early-stage startups with no DevOps capacity OR a CTO who has put a price on their own ops time. Time-poor, money-medium.
- **Higher per-MAU pricing for production** → growth-stage startups whose MAU passed 10K and who don't want to negotiate Auth0 enterprise.

The validation gate "100 stars + 5 hosted signups in 60 days" implies 5% star-to-signup. The actual base rate for OSS-to-hosted in dev tools is 0.3-3% per Section 1 search. **Math says: to hit 5 paying hosted signups, plan for 200-1,000 stars minimum, not 100.**

More importantly: the people who STAR the repo are mostly NOT the people who PAY for the hosted tier. The two cohorts are different humans. Stars validate community pull; hosted signups validate paying-buyer pull. Stars are a vanity prerequisite at best, not a leading indicator of hosted-tier viability.

**Better alternative:** add a third validation signal — *integrations actually deployed to production by real teams (not just installed locally)*. Concrete: ask hosted-tier signups whether they're using it in dev or prod, target ≥3 prod deployments by day 60 (a much stronger PMF signal than 5 generic signups).

Also: the absence of any contact-capture flow (newsletter on the blog, email gate on the docs, "what framework are you using" form on first install) means AuthForge has no way to identify which stargazers are real prospects. **Add lightweight contact-capture mechanics at install time AND on the docs.**

### M0e. Dogfood audience-class match (founder vs paying ICP)

**Question:** Is the audience the product was dogfooded on the same audience that will actually buy it?

**Verdict: PREMISE FAILS — significant risk.**

The design doc does not specify dogfood subjects. The implicit assumption is "the founder dogfoods it." For an auth SDK, founder-only dogfood is structurally inadequate because:

- Solo dogfood doesn't surface multi-tenant auth flows (paying ICP often has)
- Solo dogfood doesn't surface migration-from-Auth0 / migration-from-Clerk pain (the biggest single conversion driver in this market)
- Solo dogfood doesn't surface enterprise-IT requirements (audit logs, SCIM, role hierarchies)
- Solo dogfood doesn't surface what BREAKS at the seams between auth + payments + email + analytics in real apps

**Paying ICP for $99/mo hosted tier:** small-to-mid team (2-10 engineers) building a SaaS app, currently on Clerk/Supabase/Auth0 trial, looking for an OSS-friendly alternative that doesn't surprise them with bills. They have a real product, real users, and zero DevOps capacity.

**Required fix (per skill: BOTH pivots, not one):**
1. **Pivot target audience documentation** to explicitly center the small-team-SaaS-CTO ICP. Current "backend engineers building auth into their apps" is a category, not a persona.
2. **Expand dogfood subjects** to include 3-5 real teams using AuthForge in real apps BEFORE the public launch. Concierge onboarding of 5 friendly teams as alpha users; collect what they hit; ship fixes before launch. This is the Superhuman / Vohra play applied to dev tools.

Do NOT defer the small-team-SaaS ICP "to v1.1" while shipping a solo-dogfood library. That's the anti-pattern #14 case from the skill. Both pivots simultaneously.

### Step 0.5 verdicts — summary

| Premise | Verdict |
|---|---|
| M0a Launch platform | SURVIVES (with sequencing caveat) |
| M0b Canonical success | FAILS (no precedent anchoring; missing Stripe, SuperTokens, Better Auth lessons) |
| M0c Anti-features | FAILS (anticipated; line-by-line feature decision owed) |
| M0d Freebie-disqualifier | FAILS (validation gate math wrong; stargazers ≠ buyers; need contact capture) |
| M0e Dogfood mismatch | FAILS (solo dogfood inadequate for auth; need 3-5 alpha teams + ICP pivot) |

**4 of 5 premises fail.** Triggers the **PREMISE-LEVEL FINDINGS BLOCK** at top of plan (below).

---

## PREMISE-LEVEL FINDINGS BLOCK (top-priority insights)

> **Read this before any tactical section.** These five findings reshape every downstream decision. If the founder accepts them, the launch sequence, pricing, scope, and validation gates all change.

### Finding 1 — Positioning is anchored against the wrong competitors (2020-era, not 2026)

The "simpler than Auth0, more flexible than Supabase Auth" positioning skips the actual 2026 OSS auth field: **Better Auth, SuperTokens, Clerk, Kinde, Stack Auth, FusionAuth, Hanko**. Better Auth in particular absorbed Auth.js maintainership in Sept 2025 and is the live OSS-Next.js default. **AuthForge cannot launch with Auth0/Supabase-only positioning without looking out-of-date day one.** Rebuild differentiation against the live field.

### Finding 2 — Validation gate is mathematically wrong (5% star-to-paid is 2-15x the documented base rate)

100 stars + 5 hosted signups in 60 days assumes ~5% star-to-hosted conversion. The base rate for OSS-to-hosted dev tools is 0.3-3%. Either the star target needs to be 200-1,500 OR the signup target needs to be lowered to 1-3 OR (better) restructure the gate around production deployments not signups.

### Finding 3 — Stargazers and paying customers are different humans

The implicit theory "stargazers will upgrade to hosted tier" misreads the OSS+hosted motion. Stargazers are evaluators (often hobbyists, ICs prototyping). Paying customers are small-team CTOs who want hosted to avoid DevOps. **These are different cohorts.** Marketing/sales motion has to address both, and the validation gate has to measure the right one (production deployments, not stars).

### Finding 4 — Solo dogfood is structurally inadequate for auth; need 3-5 alpha teams pre-launch

Auth is a multi-tenant, multi-framework, integration-heavy product. Solo dogfooding produces a library calibrated to one person's mental model. Required fix: concierge-onboard 3-5 friendly small teams as alpha users BEFORE public launch. Surface migration pain (from Clerk/Supabase/Auth0), multi-tenant edge cases, SSO requirements. This pairs with **launch-gate-as-PMF-signal** (Section 5).

### Finding 5 — Founder's audience is the strongest asset, and it's being underused

Ex-Stripe + 20K monthly blog readers + 3K dev-Twitter = top-decile founder profile for a dev-tool launch. The design doc treats audience as background context, not as the primary distribution channel. **Reorient: the founder's existing writing surface is the LAUNCH PLATFORM, with Show HN as a single pulse inside a broader founder-led sequence.** Specifically: pre-launch newsletter capture on the blog (likely doesn't exist today), then a multi-week pre-launch content sequence, then HN/r/programming as the formal launch moment.

### Bonus Finding — No content capture, no contact mechanism, no install-time telemetry

The plan has no mechanism to convert anonymous stargazers/downloaders into identified prospects. No newsletter signup on the blog. No "what framework are you using?" form on first install. No docs-side contact gate. **Without this, the funnel is invisible. Fix on Week 1.**

---

## Step 0A — Forcing questions (M1–M7)

Step 0A is informed by Step 0.5 findings. Where premises failed, Step 0A enforces the corrected framing.

### M1. Audience reality (corrected ICP per M0e)

**Named persona — Maya, technical co-founder at a 6-person B2B SaaS:**
- 32 y/o; Staff/Senior IC at a previous Series A; now CTO of a seed-stage SaaS (2-engineer team, 4 total headcount)
- Stack: Next.js, TypeScript, Postgres, hosted on Vercel/Render
- Currently on Clerk's free tier; eyeing the $25/mo Pro jump but worried about per-MAU costs as her B2B users add coworkers
- Has used Auth0 at her previous job; remembers SAML rollout taking 6 weeks
- Hates vendor lock-in; would prefer an OSS option but won't self-host for time reasons
- Where she spends attention: **Pragmatic Engineer newsletter** (~1.1M subs, no sponsorships available — read as discovery surface only), **Lenny's Newsletter** (PM/eng leadership), **ByteByteGo**, **Next.js GitHub releases**, **Theo (t3.gg) YouTube**, **dev-Twitter**, **/r/nextjs**, **/r/sveltejs**, **/r/programming**, **HackerNews front page**, **Indie Hackers** (occasionally), **Web Dev Show / Syntax podcast**, **Software Engineering Daily podcast**, **Bytes newsletter** (~200K JS devs).

5+ attributes: time-poor, money-medium, ICP-aware, OSS-preferring-but-not-OSS-dogmatic, trust-shops near top-of-band when vetted.

Discovery places (≥3 named): Bytes newsletter, /r/nextjs, Theo's YouTube, Software Engineering Daily, dev-Twitter, Hacker News.

### M2. Discovery path (corrected per M0a — HN is real but NOT step 1)

**Walkthrough — how Maya discovers AuthForge:**

1. **Week -3:** Maya reads the founder's technical blog post titled something like "We rewrote auth from scratch at [previous company]; here's what we learned" — driven by **subscriber email** because she's been on the blog's list for 18 months. Blog post mentions "I've been building an OSS auth library; alpha access here."
2. **Week -1:** Theo (t3.gg) tweets a thread about Better Auth alternatives in response to a follower question; founder's library is mentioned because the founder reached out two weeks earlier.
3. **Week 0 (launch day):** Maya sees Show HN post on HN front page (founder's audience helps it get past the initial-vote critical-mass threshold). Recognizes the founder's name from the blog. Clicks through.
4. **Week 0:** Repo + docs are the conversion surface. Code-first; framework-specific quickstart for Next.js renders the "5-minute aha." Newsletter signup on docs captures her email.
5. **Week 1-2:** Newsletter follow-up sequence: "How AuthForge differs from Better Auth," "AuthForge with Postgres in 5 lines," "Migration from Clerk."
6. **Week 4-6:** Maya tries it on a side project, hits a migration question, joins Discord, gets answer from founder personally (concierge support). Decision to migrate company stack made.
7. **Week 8:** Hosted-tier upgrade.

Explicit channels: founder's blog list, Theo's Twitter, HackerNews, founder's docs + newsletter, Discord, hosted-tier signup form.

### M3. Pre-launch audience

**Numbers:**
- Twitter / X: 3,000 followers (ICP-aligned)
- Blog: ~20,000 monthly readers
- Newsletter (email): **UNKNOWN — almost certainly close to zero formal signups despite 20K monthly readers, because there is no email capture mechanism on the blog stated**. This is the load-bearing gap. **Action: install newsletter capture on the blog by end of Week 1.**
- LinkedIn: unstated
- GitHub stars on prior projects: zero (first shipped product)
- Discord / community presence: unstated
- Ex-Stripe alumni network: implicit but real (high-value)

**Verdict:** Existing audience surface is real and ICP-aligned (passes M3) BUT the email-capture gap is the bottleneck — 20K monthly readers with no signup form is 20K monthly missed conversion opportunities.

### M4. Channel honesty

**Channel where founder has demonstrable advantage:** Writing / technical blogging. ~20K monthly blog readers is real evidence. Founder fit is HIGH for the docs-as-marketing / Stripe-style playbook.

**Secondary candidate:** ex-Stripe alumni network for warm intros (founder credentials transfer here; "former Stripe engineer building OSS auth" carries trust).

**Honest "I don't have one yet" for:** Podcast presence (founder hasn't appeared on dev podcasts), YouTube (no channel), Discord community ownership (no existing community).

### M5. Competitor traffic source

Per Section 1 research:

- **Auth0:** SEO + paid + enterprise outbound. Massive SEO domain authority on "[X] authentication" queries. Paying for SDK-tutorial placements.
- **Clerk:** Next.js community + DX-driven word of mouth + heavy YouTube/Twitter presence (Brad Frost, Theo, Lee Robinson endorsements). Strong docs SEO. Conference sponsorships.
- **Supabase Auth:** Rides Supabase's larger DB/backend acquisition; auth is a bundled feature, not a primary acquisition lever.
- **SuperTokens:** HN, dev-Twitter, Discord community, integration tutorials per framework, YC alumni network.
- **Better Auth:** GitHub + Next.js community + Theo's endorsement + absorbing the Auth.js / NextAuth.js migration funnel (largest single traffic source in Sept 2025 onward).
- **Kinde:** B2B-focused content marketing + bundle-pricing positioning + paid LinkedIn for CTOs.

**Implications for AuthForge:** the playbook with highest founder-fit is the **content-led** path (Stripe / SuperTokens). The playbook with most leverage (Better Auth's Next.js + Auth.js migration funnel) is closed by virtue of Better Auth's acquisition of that funnel. Founder needs to identify and OWN a different funnel — see Section 5.

### M6. First 10 paying customers

**Refusing "GitHub stargazers will upgrade" per Finding 3.** Concrete first-10-customers list:

1. 3-5 alpha teams concierge-onboarded pre-launch (per Finding 4) — converted to paying hosted-tier when product hits PMF gate
2. 5-10 named ex-Stripe alumni who run their own startups (warm intro list — founder writes 10 named emails this week)
3. Friendly customers from founder's blog: send a personal email to top 50 commenters / engaged readers offering early access
4. 5 podcast hosts whose podcasts founder will appear on (founder names them; appears on 3 of the 5 in launch window; each podcast appearance can directly source 1-2 paying customers)
5. Twitter DM outreach to 20 small-team CTOs in founder's Twitter network who follow back

Total addressable named-prospect list: roughly 80-100 specific humans the founder can name and contact this week. From those, the first 10 paying customers should emerge by day 60.

### M7. Time allocation

**Founder's current ratio (likely):** 90% building, 10% audience. This is the technical-founder default and is wrong.

**Required:** ≥30% audience-building, structured as:
- 10% — blog writing (one technical post / week, leveraging existing readership)
- 10% — DM/outreach (10 personal messages/week to named ICP humans; ex-Stripe alumni, blog commenters, Twitter network)
- 5% — community presence (Discord, /r/nextjs, /r/sveltejs)
- 5% — podcast outreach + appearances

This is non-negotiable. The audience asset compounds before launch; building without audience-building means launching to silence.

---

## Step 0B — Mode selection

**Mode: A (Full Marketing Review) with Section 4 elevated.**

Rationale: founder has ≥1K ICP-aligned attention surface (3K Twitter + 20K blog readers) AND product is mid-build / pre-launch with ambitious validation gate (60 days). Per the v0.3 Mode A vs C tie-breaker: mid-build with hard launch date + some ICP-aligned audience + launch playbook required → Mode A with Section 4 elevated, NOT Mode C. The founder needs both an audience-build acceleration AND a sequenced launch.

All 9 sections run below.

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | Founded | Pricing (2026) | Traffic sources | Public complaints | Read |
|---|---|---|---|---|---|
| **Auth0** (Okta) | 2013 | Free to 7.5K MAU; Essentials $35/mo; Pro $240/mo; Enterprise custom; ~$0.07/MAU at scale | SEO (massive), enterprise outbound, dev paid ads | "Upgrading gives you less"; enterprise pricing trap; documentation drift since Okta acquisition | Incumbent; pricing-and-complexity attack vector wide open |
| **Clerk** | 2020 | Free to 10K MAU; Pro **$25/mo** + $0.02/MAU; Pro+SSO **$99/mo**; Enterprise custom | Next.js community, Theo/t3 endorsement, YouTube/Twitter, strong docs SEO | Per-MAU cost spike at scale ($1,825/mo at 100K MAU); B2B/orgs features cost extra | Dominant for Next.js DX; **AuthForge's $99/mo collides directly with Clerk's $99/mo SSO tier — direct price-feature comparison will be brutal** |
| **Supabase Auth** | 2020 | Free to 50K MAU; ~$0.00325/MAU after | Bundled with Supabase DB; auth is secondary | Self-host feature restrictions (`IS_PLATFORM` flag limits OSS version); "open-source-but-not-really" complaints | Cheap but only works if you're on Supabase stack |
| **SuperTokens** | 2020 | Free OSS (Apache 2.0); managed ~$0.02/MAU; pricing in same band as Clerk | HN, Discord community, framework-tutorial content, YC alumni | Lower polish than Clerk; smaller adapter ecosystem | **Most direct OSS comparable**; 12K+ GitHub stars; AuthForge competes for the same OSS-self-host audience |
| **Better Auth** | 2024 | Free OSS (MIT-ish); managed tier TBD | GitHub + Next.js community + Theo + **Auth.js maintainership absorption (Sept 2025)** | New; less battle-tested at enterprise scale | **The live 2026 OSS auth story; default new pick for self-hosted Next.js per LogRocket Aug 2026** |
| **WorkOS** | 2019 | Per-SSO-connection; ~$125/connection/mo | Enterprise IT outbound, B2B content | Limited for non-SSO use cases | Different motion (enterprise SSO-first); not a direct AuthForge competitor for $99/mo tier |
| **Kinde** | 2023 | Bundle $25/mo (orgs+roles+MFA+social+flags) | Content, LinkedIn paid, early-stage CTO targeting | Newer; smaller ecosystem | **Aggressive bundle-pricing positioning; competes for same early-stage SaaS CTO Maya** |
| **FusionAuth** | 2018 | Community Edition free; enterprise from ~$125/mo | SEO; "Auth0 alternative" comparison content | Heavier than Clerk; Java-based; older-school | Mature feature set; older positioning |
| **Hanko** | 2022 | AGPL v3 OSS; managed tier | Passwordless / passkey-first content | AGPL license limits commercial adoption | Passkey-first wedge; narrower positioning |
| **Stack Auth** | 2024 | OSS; managed tier | Next.js community | Newer; smaller adoption than Better Auth | Closest drop-in upgrade from Better Auth |

### 1b. Canonical-success comparables (motion class: OSS dev tool + hosted tier / open-core)

| Comparable | Price | Founded | Scale | Primary acquisition | Onboarding | Launch gate | Delta vs AuthForge plan |
|---|---|---|---|---|---|---|---|
| **Stripe** | usage % | 2010 | $1T+ valuation; revenue $10B+ | Docs as marketing, Patrick Collison writing, "engineering as marketing," per-framework integration content | Self-serve API keys, copy-paste docs | None — built relationships before launching | AuthForge has the same founder profile (ex-Stripe; technical writing track record) but does NOT have Stripe's per-framework integration tutorial sequence planned |
| **SuperTokens** | OSS free + managed | 2020 | 12K+ stars; YC-backed | HN, framework tutorials, transparent comparison charts (including where they lose), Discord | Self-host OR managed | OSS-first; managed came later | AuthForge's "100 stars in 60 days" is below SuperTokens' early trajectory; SuperTokens shipped honest competitor-comparison content. AuthForge plan does NOT include transparency-on-loss content. |
| **Better Auth** | OSS free + managed TBD | 2024 | Absorbed Auth.js maintainership | GitHub + Theo + community migration funnel | Code-first integration | OSS launch, community-led | Better Auth captured the largest single migration funnel (Auth.js/NextAuth.js). AuthForge needs to identify a different migration funnel to own (Auth0-pricing-refugees? Supabase-self-host-frustrated?). |
| **Postiz** | OSS + hosted | 2024 | $17K MRR; 5M+ downloads | OSS-as-marketing | Self-host OR hosted | Open-core, no gate | Documented 0.3-3% OSS-to-hosted conversion — AuthForge's 5/100 = 5% target is 2-15x base rate |
| **Papermark** | OSS + hosted | 2023 | $75K MRR / $900K ARR in 18mo | OSS-as-marketing; content on DocSend alternative pain | Hosted-first easy; self-host as option | Open-core | Same pattern; AuthForge should plan for 18-month ramp to $75K MRR, NOT 60-day validation as the real PMF gate |
| **Vercel** | OSS Next.js + hosted | 2015 | $9B+ valuation | Framework authorship (Next.js as marketing) | Hosted-first, OSS as background | Hosted-first | AuthForge isn't building a framework — has less definitional leverage; needs another wedge |

### 1c. Pattern surface

**What canonical successes have in common that AuthForge plan lacks:**
- **Founder writing as primary distribution.** Stripe (Patrick Collison), Vercel (Guillermo Rauch), SuperTokens (consistent technical blog). AuthForge has the writing asset but isn't deploying it as primary distribution.
- **Per-framework integration content as evergreen funnel.** Stripe has a tutorial for every framework. Clerk has Next.js-specific everything. AuthForge plans "write integration tutorials" — too vague.
- **Transparent loss documentation.** SuperTokens explicitly says "here's where we lose to Auth0." Builds trust with the dev audience that hates marketing-speak. AuthForge plan has none of this.
- **Long-horizon thinking on conversion.** Papermark took 18 months to $75K MRR. AuthForge's 60-day gate is a smoke-test, not a PMF gate.

**Where direct competitors diverge from canonical patterns:**
- Auth0 succeeded with enterprise outbound, NOT OSS — different motion class entirely
- Clerk succeeded with closed-source + premium DX + Next.js partnership, NOT OSS — different motion class
- Better Auth succeeded with OSS but rode the Auth.js community capture, a one-time event AuthForge can't replicate

**Which pattern is the current plan implicitly following?** Show HN + r/programming + "write tutorials" reads as **lottery-ticket motion**, not as the **content-led-compounding motion** the founder is actually best-equipped to execute. The founder's profile (ex-Stripe, 20K blog readers) maps to a Stripe-style content motion that the current plan doesn't deploy.

**Founder action:** read Patrick Collison's writing on Stripe's early years; read SuperTokens' comparison content (e.g., their "SuperTokens vs Auth0" page); read Better Auth's GitHub README + recent blog. Output: write one positioning paragraph per direct comparable in `icp.md`.

---

## Section 2 — ICP specification (→ `icp.md`)

Full ICP doc written to `icp.md`; summary here:

- **Named persona:** Maya, CTO at a 6-person B2B SaaS (per M1 above)
- **Adjacent paid products in her stack:** Vercel ($20-150/mo), Linear ($8/user/mo), Sentry ($26/mo), Resend ($20/mo), PostHog ($0-450/mo), GitHub Team ($4/user/mo). Spends $200-800/mo on dev infra.
- **Adjacent-category complaints:** Auth0 enterprise sticker shock; Clerk per-MAU surprise bills as B2B customers add seats; Supabase self-host feature restrictions; "I just want auth that doesn't have a salesperson"
- **Objection patterns:** "Is this safe at scale?" / "What happens to my migration path if you pivot/shut down?" / "Why not just use [Better Auth / Clerk / Supabase]?" / "Who else trusts this in production?"
- **Conversion reasons:** OSS-with-real-managed-tier (escape hatch from vendor); ex-Stripe credibility (engineering taste); transparent comparison content (signals honest); SDK-quality + Next.js Quickstart that works in 5 minutes; community presence signaling production-readiness

---

## Section 3 — Distribution channels (dev-tool motion class)

Per v0.3 motion-class rules, the dev-tool primary channels are: **(1) Docs/SEO compounding, (2) GitHub as marketing surface, (3) Founder's existing dev-audience surfaces.** All three are ranked above generic launch channels.

### Channel-by-channel scoring (1-5, weighted for founder fit)

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Composite | Verdict |
|---|---|---|---|---|---|---|---|
| **Docs / SEO (per-framework tutorials)** | 5 | low | 4 | 5 (writer) | 4 (sustained) | **PRIMARY** | Build "Auth in [Next.js/SvelteKit/Remix/Astro/Hono/Express/FastAPI]" pages. 6-12 month SEO compound. Stripe playbook. |
| **GitHub repo as marketing surface** | 4 | low | 4 | 4 | 3 | **PRIMARY** | Repo health, README quality, transparent comparison chart, visible adopters in dependency graph, contributor recognition. Star count materially affects evaluator conversion. |
| **Founder's blog (20K monthly readers)** | 4 | zero | 5 | 5 | 2 (already writing) | **PRIMARY** | Highest-leverage existing asset. Add newsletter capture immediately. |
| **Founder's Twitter (3K)** | 3 | zero | 4 | 4 | 2 | **HIGH** | Build-in-public thread cadence; Stripe-engineering-to-OSS-auth narrative |
| **Show HN** | 4 (one-shot) | zero | 3 | 4 (right audience class) | 2 (one post) | **HIGH (single pulse)** | Use as ONE channel inside a sequence; not the plan |
| **/r/nextjs, /r/sveltejs (vertical reddit)** | 3 | zero | 4 | 3 | 2 | **HIGH** | Compliant launch posts AFTER demonstrated repo activity; not on launch day |
| **/r/programming** | 3 | zero | 2 | 3 | 1 | MEDIUM | Mixed-audience; less ICP-tight than vertical subs |
| **Podcast guesting** | 3 | zero | 5 | 3 (no track record) | 4 | **HIGH** | Software Engineering Daily, Syntax, JS Party, Devtools.fm. Slow ramp; deep audience. Founder needs to pitch starting now. |
| **Pragmatic Engineer (sponsorship)** | 5 | n/a | n/a | n/a | n/a | **N/A — no sponsorships available**; treat as discovery surface only via earned mentions / podcast guesting on PE Podcast (500K-650K views/episode) |
| **Bytes / JavaScriptWeekly sponsorship** | 4 | $$ | 3 | 2 | 2 | **MEDIUM** | If budget allows post-launch; not pre-launch |
| **Lenny's Newsletter** | 4 | $$$ | 2 | 1 (wrong audience — PM/leadership) | 3 | **LOW — wrong audience** for dev-tool sale |
| **Discord (own community)** | 3 | low | 5 | 3 | 4 (sustained) | **MEDIUM** | Build alongside launch; needed for hosted-tier support trust |
| **LinkedIn organic** | 2 | zero | 3 | 2 | 2 | LOW | Weak fit for OSS dev tool |
| **Product Hunt** | 3 | zero | 2 | 2 | 2 | LOW | Single-shot; weaker for dev tools than for consumer; do AFTER Show HN as separate event |
| **YouTube** | 4 | zero | 4 | 1 (no channel) | 5 | LOW | Could matter long-term; founder needs to start with podcast guesting first |
| **Cold outreach (named ex-Stripe alumni)** | 2 (small reach) | zero | 5 | 5 | 2 | **HIGH** | Highest-conversion channel for first 10 paying customers |
| **Indie Hackers** | 2 | zero | 2 | 2 | 1 | LOW | Wrong ICP for B2B-CTO sale |
| **Theo (t3.gg) / Lee Robinson / dev-influencer DMs** | 4 | zero | 4 | 3 | 3 | **HIGH** | Cold-warm DM with working repo; if they tweet, can drive 1-2K stars in a day |
| **Paid ads (Google, Twitter, LinkedIn)** | varies | $$$ | 2-3 | 1 | 3 | LOW | Skip pre-launch; consider post-PMF only |
| **Conference sponsorships** | 3 | $$$$ | 3 | 2 | 4 | LOW | Skip until $50K MRR |
| **Affiliate / partner integrations** | varies | low | 4 | 2 | 4 | MEDIUM-deferred | Vercel template / create-next-app integration is high-leverage once stable; defer to v1.5 |

### Prioritized channel set (the 3-5 to actually ship)

1. **Founder's blog + new newsletter capture** (PRIMARY — week 1 fix is install email capture)
2. **Docs/SEO per-framework tutorials** (PRIMARY — Next.js, SvelteKit, Remix, Hono, Express, FastAPI in priority order)
3. **GitHub repo as marketing surface** (PRIMARY — README, transparent comparison chart, visible adopters)
4. **Twitter build-in-public + ex-Stripe + dev-influencer DMs** (HIGH leverage)
5. **Show HN + /r/nextjs as the formal launch pulse** (HIGH — one of three channels on launch day)
6. **Podcast guesting** (HIGH — start pitching now; lands in post-launch window)
7. **Cold outreach to named ex-Stripe alumni** (HIGH — for first 10 paying customers)

### Dev-tool tonal rule (load-bearing for Section 5 copy)

Per v0.3 skill rule: REFUSE marketing-speak in launch copy. Specifically:

**DO NOT use:** "revolutionary", "best-in-class", "enterprise-grade", "world-class", "game-changing", "seamless", "robust", "10x faster", "next-generation"

**DO use:**
- Architecture specifics ("uses HTTP-only cookies + rotating refresh tokens; we made these specific trade-offs because...")
- Honest losses ("Better Auth is more mature at Next.js App Router edge cases right now; here's what we do differently")
- Code-first framing (link to repo + code snippet BEFORE the landing page on HN)
- "Engineer wrote this for engineers" register

This is THE most common dev-tool launch failure pattern. Founder's instinct will be to write copy that "sells"; the dev audience reads selling as adversarial.

---

## Section 4 — Pre-launch audience-building plan (ELEVATED per Mode A tie-breaker)

### Day 1-30 (foundational; this week through end-of-June)

**Single biggest action:** Install newsletter capture on the technical blog. THIS IS THE BOTTLENECK. 20K monthly readers with no email signup is the largest lever in the entire plan. ConvertKit / Buttondown / Beehiiv — pick one this week.

**Weekly cadence:**
- 1 long-form blog post / week, leveraging the existing 20K reader funnel. Topics: "Why I'm building an OSS auth library," "What I learned shipping auth at Stripe," "AuthForge: the design decisions" (these prime the launch narrative)
- 5 Twitter threads or build-in-public posts / week
- 10 named DMs / week to ex-Stripe alumni, blog commenters, dev-Twitter contacts (curate the "first 10 paying customers" funnel)
- 1 podcast pitch / week (Software Engineering Daily, Syntax, JS Party, Devtools.fm, ShopTalk, ChangeLog, Dev Tools FM, Web Dev Show)
- Daily presence in /r/nextjs (answer auth-related questions; build name recognition; do NOT self-promote yet)
- Open the Discord (private alpha channel for the 3-5 alpha teams)

**Concierge alpha-team onboarding:** Identify 3-5 small SaaS teams (preferably in founder's network) who are evaluating auth or unhappy with current solution. Personally onboard them. Collect what breaks. Ship fixes. THIS IS THE PMF GATE for the launch.

### Day 31-60

**Cadence holds.** Scale where signal appears:
- If newsletter is growing: increase frequency to 2 posts/week, segment by framework interest
- If podcast pitches landed: schedule 2-3 podcast appearances for launch window
- If Discord is growing: weekly office hours
- If alpha-team feedback surfaces a specific framework gap: prioritize that framework's tutorial

**Continue concierge alpha-team onboarding.** Target: 3-5 teams in production by end of day 60.

**Hardening week (days 50-60):** lock the v1 feature set per M0c anti-feature decision (defer SSO/SAML, defer admin dashboard, defer the second product story).

### Day 61-90

**Launch sequence (see Section 5)** runs in days 61-75; days 76-90 are post-launch follow-up content + outreach + analyzing real conversion data.

---

## Section 5 — Launch playbook (→ `launch_playbook.md`)

### 5a. Question the launch gate (calendar vs PMF signal)

**The design doc commits to a calendar-driven gate: "100 GitHub stars + 5 hosted-tier signups by day 60."** Per skill v0.3 Section 5a, for retention-driven products the gate should be PMF-signal-driven.

**Is auth retention-driven?** YES, intensely. Auth is the foundation of every authenticated request. Switching cost is high. Failures are catastrophic (locked-out users). The product MUST be indispensable to its first cohort before public launch, or churn from launch-day-noise users will mask actual PMF.

**Recommended gate (replaces the design doc gate):**

> **PMF gate:** ≥3 alpha teams running AuthForge in production AND ≥2 of those teams answer "very disappointed" to the Vohra question ("how would you feel if you could no longer use AuthForge") before formal public launch. Public launch fires ONLY when both conditions met.

> **Soft launch gate (parallel, but does NOT replace PMF gate):** founder is willing to do public Show HN at any point but should NOT do hosted-tier marketing until PMF gate is met. Public OSS launch can precede PMF gate; hosted-tier marketing CANNOT.

If founder defends the calendar gate, surface the Vohra/Superhuman precedent and the Postiz/Papermark 18-month ramp data. The 60-day calendar gate fires whether or not the product is indispensable.

### 5b. Sequenced launch playbook

**Acceptable reason to keep some calendar discipline:** dev-tool launches benefit from time-bounded marketing moments (Show HN gets a single shot). So the recommendation is **PMF gate for the hosted-tier marketing push, calendar discipline for the OSS launch pulse.**

Detailed schedule below assumes Day 0 = formal public launch day after PMF gate clears (approximate target: end of July 2026, which is ~60 days from now if alpha-team onboarding starts this week).

| Day | Channel | Specific action | Notes / tonal rules |
|---|---|---|---|
| -30 | Blog | Long-form post: "What I learned shipping auth at Stripe" (warms audience; primes narrative; NOT a product post yet) | Founder-voice; technical |
| -30 | Newsletter | Email blog readers asking for "auth pain stories" — collect insight + opt-in signups | Conversion mechanic |
| -21 | Twitter | Build-in-public thread #1: "I'm building an OSS auth library. Here's why." | Honest about scope; mentions Better Auth, Clerk, SuperTokens by name with respect |
| -14 | Blog | "AuthForge: design decisions" post — architecture-first; states explicit trade-offs (what AuthForge does WORSE than Better Auth at) | Trust-builder via transparency |
| -14 | Personal email | Email 30 named ex-Stripe alumni: "I'm doing this; would love your take." | Soft pre-announce; warm intro flywheel |
| -10 | Discord (private) | Alpha-team Discord channel goes semi-public | Community seed |
| -7 | Twitter | Build-in-public thread #2: "10 days to launch. Here's what's in v1, here's what's NOT." Explicit anti-feature list. | Tonal: honest scope |
| -7 | DM | Cold-warm DM Theo, Lee Robinson, dev-influencers: "Repo's open; would love your take" (NOT "would you tweet about it") | No ask; show, don't ask |
| -3 | Blog | Pre-launch post: "Why I think the auth market has room for one more OSS library" | Positioning post; explicit comparison to Better Auth, SuperTokens, Clerk |
| **0 (07:00 PT)** | **Hacker News** | **Show HN post with link to GitHub repo (NOT to landing page). Title: "Show HN: AuthForge – open-source auth library with $99/mo hosted tier"** | **Code-first link; no marketing-speak; lead with architecture trade-offs in the body comment** |
| 0 +2h | Twitter | Thread linking to HN post, but lead with technical specifics ("we went with HTTP-only cookies + rotating refresh tokens; here's why"). One sentence near the end mentions HN link. | Tonal: engineering-first |
| 0 +4h | Founder's blog | Launch post pinned to top. Includes: 5-minute Next.js quickstart, transparent comparison chart, code samples | Conversion surface |
| 0 +4h | Newsletter | Email to entire newsletter list: "AuthForge is out" | Owned channel |
| 0 +6h | /r/nextjs | Compliant post following sub rules (check Wiki; some subs allow OSS releases, some require waiting). NOT a duplicate of HN copy | Vertical reddit |
| 0 +12h | Personal emails | Email 50 named ex-Stripe alumni + blog commenters: "It's out; here's the link" | Warm-network pulse |
| 0 +24h | /r/programming | Cross-post (HN-first to avoid Reddit duplicate penalty) | Lower priority than /r/nextjs |
| 0 +48h | /r/sveltejs, /r/golang, /r/node | Vertical subreddits for each supported framework | Compliant; check Wiki |
| 0 +72h | Indie Hackers | Cross-post with "what I learned launching" angle | Lower-priority audience |
| Day 7 | Discord | Open Discord to public; weekly office hours announcement | Community |
| Day 7-14 | Podcast | First scheduled podcast appearance (pitched starting day -30) | Software Engineering Daily / Syntax target |
| Day 7-14 | Product Hunt | Separate launch event (different audience overlap) — only if PMF gate is met | Optional pulse |
| Day 14-30 | Blog | "AuthForge launch retrospective: what worked, what didn't, real numbers" | Trust + traction signal |
| Day 14-30 | Per-framework tutorials | Ship 1 per week: Next.js, then SvelteKit, then Remix, then Hono, then Express, then FastAPI | SEO compound start |
| Day 30+ | Founder writing cadence | 1 post/week sustaining content rhythm | Compounds |

### 5c. Risk callouts

- **HN miss:** if Show HN gets <50 upvotes, do NOT re-launch within 2 weeks (HN rules). Fallback: lean harder on owned channels (newsletter, blog, Twitter) + Theo/dev-influencer DMs + podcast appearances. Show HN is one channel; the founder's owned audience is the others.
- **All-on-Twitter risk:** mitigated by blog + newsletter + Discord + GitHub presence; Twitter is HIGH but not primary.
- **Single Reddit subreddit ban:** mitigated by multiple vertical subs; check Wiki rules for each.
- **Better Auth counter-launch:** Better Auth could ship a managed tier announcement same week. Mitigation: own a distinct positioning (post-Stripe taste + transparent comparison + concierge-team migration support).
- **Alpha team withdraws before PMF gate:** mitigation: 3-5 teams, not 1-2; concierge support keeps churn down.

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing BAND before the price point

**The design doc anchors $99/mo flat for hosted tier + $0.001/MAU above 10K.** Where did $99 come from? Most likely from "feels right for a managed dev tool" — i.e., competitor-anchored against Clerk-style pricing without ICP willingness-to-pay evidence.

**Critical price collision discovered:** **Clerk's Pro+SSO tier is also $99/mo.** AuthForge launching at the exact same flat price as Clerk's premium tier sets up a direct head-to-head comparison that AuthForge will likely lose on feature count (Clerk has SSO, SAML, mature UI components, B2B orgs). The pricing point inherits from competitor-anchoring AND collides with a specific competitor.

**ICP willingness-to-pay evidence:**
- Maya's stack: Vercel $20-150/mo, Linear $8/user/mo, Sentry $26/mo. Adjacent dev infra spend is $200-800/mo total.
- For a CTO with 4-10 paying customers in early SaaS, $99/mo is ~5-12% of total dev infra. Defensible IF the value prop is clearly "this saves me from Auth0 enterprise OR from Clerk per-MAU spike."
- For an early-stage team WITHOUT MAU pain yet: $99/mo competes against Clerk's free 10K tier — and loses on the "why pay $99/mo when Clerk's free tier covers me?" question.

**Pricing-band failure mode:** the $99 flat tier prices AuthForge OUT of the early-stage CTO who isn't yet feeling pain and IN with the growth-stage CTO who's already evaluating Clerk Pro+SSO ($99) or Auth0 Pro ($240). In that growth-stage comparison, AuthForge needs a clearly-better story than Clerk Pro+SSO, OR a clearly-cheaper story.

**Recommendations:**

Option A (recommended): **Restructure to $0 / $29 / $199 tiers, not flat $99.**
- **Free / OSS self-host:** unlimited, no MAU cap, fully MIT (drives community adoption)
- **Starter Hosted $29/mo:** managed instance up to 10K MAU; aimed at early-stage CTO who wants hosted but isn't at scale (sits below Clerk's effective $25/mo + per-MAU spike; clear "predictable bill" wedge)
- **Pro Hosted $199/mo:** managed instance with SLA, included higher MAU, support priority; positioned ABOVE Clerk Pro+SSO at $99/mo with clear differentiation (better SLA, OSS escape hatch, ex-Stripe team)
- **Enterprise:** custom; SSO/SAML, audit logs, multi-region

This gives THREE pricing wedges (predictable bill at low end, OSS escape at all levels, premium SLA at top) instead of one collision-with-Clerk price point.

Option B: **Keep $99 flat but reposition strongly.** Only viable if AuthForge can claim a specific Clerk-Pro+SSO-can't-do-this feature. Hard to defend.

### 6b. Standard pricing & packaging coverage

- **Trial mechanics:** free OSS self-host IS the trial. Per M0d freebie-disqualifier finding: the OSS-stargazer cohort is NOT the paying cohort. Trial mechanic for HOSTED tier should be different: offer a 14-day free hosted trial with required credit card (filters time-rich/money-poor) OR free for first 30 days with concierge-onboarding session (signals serious intent). Recommend: 14-day free trial with credit card required, with explicit concierge-onboarding for paying tier.
- **Annual discount:** ~20% off annual billing; documented in RevenueCat State of Subscription Apps as the single strongest retention lever. Add at launch.
- **Per-seat vs per-feature vs per-usage:** AuthForge's per-MAU model is the SaaS-standard but competes directly with Clerk/Auth0 pricing fatigue. Consider a per-team / per-instance flat-rate model for the hosted tier (e.g., $199/mo for unlimited MAU on a managed instance up to N requests/sec) — differentiates against per-MAU-spike pain that drives Clerk-to-self-host migration.
- **Migration program:** offer free migration concierge from Clerk / Auth0 / Supabase to AuthForge hosted tier. Documented migration tooling. This is the "Better Auth captured Auth.js migration funnel; AuthForge captures Clerk-pricing-refugee migration funnel" play.

---

## Section 7 — Post-launch growth loops

What compounds:
- **Docs/SEO** — per-framework tutorials rank for long-tail "[framework] auth" queries; 6-12 month ramp; durable compounding
- **GitHub stars + visible adopters** — social proof compounds; star count gates evaluator conversion
- **Founder writing cadence** — owned channel; readers compound; newsletter list compounds
- **Discord community** — once seeded, community answers questions for free
- **Migration testimonials** — each Auth0/Clerk → AuthForge migration is a marketing asset
- **Open-source contributors** — each external contributor signals project health AND brings their audience

What's linear:
- Per-team hosted-tier signups (sales motion is largely 1:1)
- Podcast appearances (each appearance is a discrete event)
- Cold outreach (each email is 1:1)

**Acquisition-treadmill risk:** medium. The OSS-as-marketing motion does compound (SEO + stars + community), so AuthForge is NOT acquisition-treadmill if those compound. Risk emerges if all three of those compound poorly AND the founder relies on launch-day pulses to keep signups flowing.

**Specific in-product growth loops to add at launch:**
- **"Powered by AuthForge" footer on hosted-tier login UI** (optional toggle; default on for free tier, removable on paid; classic Mailchimp-style viral mechanic for B2B SaaS)
- **Referral program:** $50 credit for each customer referred who reaches paid tier
- **Open issue/PR recognition:** highlight contributors in CHANGELOG and on website (HashiCorp HUG playbook)

---

## Section 8 — Metrics & instrumentation

### What to measure (weekly dashboard)

**Acquisition (by channel, with UTMs):**
- New GitHub stars / week (by source: HN, Twitter, blog, Reddit, organic)
- Newsletter signups / week (by source: blog, docs, launch event)
- Hosted-tier signups / week (by source: docs, blog, referral, direct)
- npm downloads / week (or equivalent SDK install count)

**Activation:**
- Definition: "user installs AuthForge AND completes the 5-minute quickstart AND successfully authenticates at least one user." Telemetry needed in the SDK (anonymous; opt-out).
- Activation rate among installers
- Time-to-first-successful-auth (target <5 minutes)

**Retention (cohort-tracked):**
- Day-7 / day-30 retention of hosted-tier signups
- Day-30 retention of OSS installers (measured via opt-in telemetry on continued use)
- Production-deployment count: how many hosted-tier accounts have a verified production deployment

**Conversion:**
- OSS install → hosted-tier signup rate (target: 0.5-2% per Section 1 base rate)
- Free-trial → paid conversion rate
- Free OSS → paid hosted conversion (the open-core motion's main metric)

**PMF signal:**
- Vohra "very disappointed" % among active hosted-tier users (target: ≥40% pre-formal-launch)
- Net Promoter Score (target: ≥50)
- Unprompted referrals from first cohort (count)

**LTV / CAC:** track once there's 6+ months of data; not actionable in first 90 days

### Vanity metrics to AVOID

- Twitter follower count
- Total signups without retention
- HN upvote count
- GitHub star count alone (without correlated production deployments)
- Newsletter open rates (CTR is more meaningful)

### Concrete dashboard tools

- PostHog for product analytics (founder's stack)
- Plausible / Fathom for site analytics (privacy-respecting; matches OSS positioning)
- GitHub Insights for repo metrics
- ConvertKit / Beehiiv built-in for newsletter
- Manual weekly tracker spreadsheet (founder's responsibility) for the synthesis above

---

## Section 9 — Risk analysis

| Risk | Likelihood | Severity | Mitigation |
|---|---|---|---|
| **Channel concentration on HN** | Medium | High | Multi-channel launch sequence per Section 5; owned newsletter as backstop |
| **Better Auth ships managed tier same quarter** | Medium-High | High | Differentiated positioning: post-Stripe taste + concierge migration support + transparent comparison; do not try to out-Next.js Better Auth |
| **Clerk drops a price competitor at the $99 tier** | Low | Medium | Pricing restructure per Section 6 avoids head-to-head collision |
| **Auth0 ships an OSS edition** | Low | Medium | Unlikely (Okta would not OSS-pivot); not a top-risk |
| **Solo dogfood ships a library that breaks at real-team scale** | High (without mitigation) | Critical | Concierge-onboard 3-5 alpha teams before launch (per Finding 4) |
| **Founder's $99 flat-tier prices out early-stage CTO** | High (under current plan) | High | Restructure to $0 / $29 / $199 tiers (Option A) |
| **Validation gate (5% star-to-paid) fires false negative or false positive** | High | Medium | Replace gate with production-deployment count + Vohra signal (per Section 5a) |
| **Email capture not installed; 20K monthly readers wasted** | High (current) | High | Install newsletter capture by end of Week 1 |
| **Founder spends <30% time on audience-building** | High (default for technical founders) | High | Explicit time budget per Section 4; weekly self-audit |
| **Dev-tool tonal slip ("revolutionary auth library")** | Medium | Medium | Copy review for marketing-speak per Section 3 tonal rules; review every public post |
| **CAC inflation on paid ads** | n/a | n/a | Not planning paid ads pre-PMF |
| **Trust risk from new project without traction** | High | Medium | Ex-Stripe credibility + transparent comparison content + visible alpha-team adopters + Discord activity |
| **Macro / platform risk (HN algorithm change, X visibility collapse)** | Low-Medium | Medium | Owned channels (blog, newsletter, docs/SEO) are platform-independent |
| **License risk (MIT chosen over AGPL)** | Low | Low | MIT is appropriate for adoption; consider business-source-license for hosted-tier-only features only if AWS-clone risk materializes |
| **Acquisition-treadmill** | Low (compounders exist) | Medium | Per Section 7 — SEO + stars + Discord compound |

---

## Outside voice — independent marketing critique

Acting as an independent reviewer with no prior commitment to the inside plan:

### 1. Single biggest risk the inside review missed

**The competitive math against Better Auth is worse than the inside plan admits.** Better Auth absorbed the Auth.js / NextAuth.js maintainership in September 2025. NextAuth.js had >27K GitHub stars and the dominant install base in Next.js auth — that migration audience is now Better Auth's owned funnel. AuthForge is launching as the third OSS option in a market where the #1 alternative (Better Auth) is actively absorbing the #2 (NextAuth.js) community. The "third entrant in OSS auth" position is structurally harder than the inside plan treats it. Specific mitigation: AuthForge needs to identify a DIFFERENT migration funnel to own (Clerk-pricing-refugees? Supabase-self-host-frustrated? Auth0-enterprise-fleeing?). The plan should NAME the migration funnel explicitly.

### 2. Channel mentioned that's actually weaker than positioned

**"Founder's Twitter / X (3K)" is weaker than the plan treats it.** 3K dev-Twitter is small. Algorithm shifts in 2024-2026 have meaningfully suppressed organic reach for non-paying accounts; 3K followers typically see 500-1.5K impressions per tweet. That's not enough to drive launch lift on its own. The blog (20K monthly readers) is doing 13-40x more reach than Twitter — the plan should weight blog far higher than Twitter as a launch lever. Twitter is HIGH because dev-influencer DMs CAN drive lift if Theo/Lee Robinson amplify; without that amplification, organic Twitter is moderate at best.

### 3. Audience claim lacking evidence

**"20K monthly blog readers" is asserted from the design doc with no traffic-source / engagement evidence.** Are those 20K unique visitors? Sessions? Pageviews? Is the audience converting on anything (newsletter, social follow, repo clicks)? Without evidence of READER-TO-ACTION conversion, 20K monthly readers could be high-bounce SEO traffic that doesn't engage with the founder's voice. **Action:** founder should audit blog analytics this week — bounce rate, time-on-page, conversion to any CTA — before treating 20K as load-bearing.

### 4. Provocative reframe

**Should AuthForge be an OSS library at all? Or should the wedge be the migration tool from Auth0/Clerk to a customer's own self-managed instance?** The OSS auth library market is increasingly crowded (Better Auth, SuperTokens, Hanko, Stack Auth, FusionAuth, NextAuth.js). The MIGRATION market is empty. Founder is uniquely positioned (ex-Stripe = trust + migration tooling experience) to offer "AuthForge Migrate" — a tool that takes a Clerk/Auth0 customer's data + auth flows and ports them to a self-managed AuthForge instance, with optional hosted tier. This recasts the product as a **rescue / cost-control wedge** rather than a "third OSS auth library." The hosted tier becomes the easy-button after migration. Worth a founder conversation: is "yet another OSS auth" actually the right product, or is "the auth migration company" the bigger opportunity?

These four findings are surfaced for founder discussion. Items 1 and 4 are the most provocative and warrant explicit response before final plan lock.

---

## Handoff — top 3 actions for THIS week

The founder must commit to three specific actions before next session:

### 1. Install newsletter capture on the technical blog. (Highest leverage; estimated 2 hours.)

ConvertKit, Beehiiv, or Buttondown. Add a signup form to the blog header AND footer AND a soft inline CTA mid-article. Begin emailing the list weekly with technical content (NOT product launches yet). Goal: convert 20K monthly readers into a measurable, owned audience. Without this, every other downstream tactic is dampened.

### 2. Identify and personally contact 5 candidate alpha-team CTOs this week. (PMF gate prerequisite.)

Personal emails. Specific ask: "I'm building OSS auth. Want to be one of 5 design-partner teams who get free hosted tier for life in exchange for weekly feedback and a willingness to ship me what breaks?" Target: 3 confirmed by next week; 5 confirmed by week 3. These become the PMF-gate cohort AND the first paying customers post-launch AND the first public testimonials.

### 3. Audit blog traffic + write the first "design decisions" post. (Audience asset confirmation.)

This week, pull blog analytics: are the 20K monthly readers engaged? What posts get the most engagement? Who are they (referrer breakdown, geographic / role inference)? Use the data to inform the first AuthForge-adjacent post: "What I learned shipping auth at Stripe" (or equivalent — pre-launch warm-up post that primes the audience without selling the product). Goal: confirm the audience asset is real, then start activating it.

### Self-check

Re-run `/plan-cmo-review` in 30 days against actual numbers (newsletter signups, alpha-team count, blog engagement, Show HN draft copy, podcast pitch count). The gate for "is this plan working" is: by day 30, is the founder generating ≥3 leading-indicator wins (newsletter live + signups, ≥3 alpha teams committed, ≥1 podcast appearance booked, ≥2 dev-influencer DMs returned positively)? If <3, the audience-build sprint is failing and the launch sequence should be paused.

### Follow-up skill recommendations

- `/office-hours` — if Outside Voice Item 4 (migration-wedge reframe) lands, the positioning is shifting meaningfully and warrants a fresh problem-framing pass
- `/plan-ceo-review` — if the pricing restructure (Section 6 Option A: $0 / $29 / $199) is adopted, business model assumptions shift and warrant a CEO-level review
- `/plan-eng-review` — if the in-product growth loops (referral program, "Powered by AuthForge" footer, anonymous telemetry) are adopted, product spec needs adjustment

---

## Artifacts written

- `marketing_plan.md` (this file)
- `icp.md` — ICP specification with Maya persona, adjacent stack, objection patterns
- `launch_playbook.md` — sequenced launch schedule (Day -30 through Day +30)
- `audience_build_journal.md` — weekly tracking template
- `TODOS.md` — short-list of marketing implementation tasks

## Web searches performed (live, with citations)

1. https://gautamkhorana.com/blog/authentication-services-2026-clerk-auth0-supabase-workos/ — competitor landscape 2026
2. https://workos.com/blog/top-better-auth-alternatives-secure-authentication-2026 — Better Auth ecosystem
3. https://news.ycombinator.com/item?id=41923641 — HN discussion of auth alternatives
4. https://dev.to/thiago_alvarez_a7561753aa/clerk-vs-better-auth-2026-we-verified-every-price-so-you-dont-have-to-13pk — Clerk pricing
5. https://clerk.com/pricing — Clerk pricing tiers (incl. $99/mo Pro+SSO tier collision)
6. https://github.com/orgs/supabase/discussions/17876 — Supabase self-host limitations complaints
7. https://danfking.github.io/blog/2026/04/23/show-hn-by-the-numbers/ — Show HN base rates (188K post analysis)
8. https://druriley.com/stripe-marketing-playbook-7-strategies-33-examples/ — Stripe playbook
9. https://supertokens.com/about-us — SuperTokens 12K+ stars + transparent comparison strategy
10. https://github.com/nextauthjs/next-auth/discussions/13252 — Better Auth absorbing Auth.js maintainership Sept 2025
11. https://blog.logrocket.com/best-auth-library-nextjs-2026/ — 2026 Next.js auth library landscape
12. https://stormy.ai/blog/open-source-saas-launch-playbook — Postiz / Papermark open-core conversion data
13. https://www.getmonetizely.com/articles/whats-the-optimal-conversion-rate-from-free-to-paid-in-open-source-saas — OSS hosted conversion base rate (0.3-3%)
14. https://blog.pragmaticengineer.com/sponsor/ — Pragmatic Engineer no-sponsorship policy
15. https://newsletter.pragmaticengineer.com/about — Pragmatic Engineer reach (1.1M subs)
16. https://comparetiers.com/tools/clerk — Clerk tier comparison (confirmed $99/mo Pro+SSO)
17. https://www.getmonetizely.com/articles/clerk-vs-auth0-pricing-for-startups-how-to-choose-the-right-identity-tool — Auth pricing comparison

