# AuthForge — Marketing Plan (CMO Review)

**Status:** COMPLETE — full run, Mode A with elevated Section 4.
**Run:** dev-tool-2026-06-01-v0.3-blindA
**Date:** 2026-06-01
**Mode:** **Mode A (Full Marketing Review)** — see Step 0B for tie-breaker reasoning.
**Founder posture:** Marketing-naive default applies (ex-Stripe engineer, no prior $10K+ MRR shipped product). HOWEVER, the founder's existing 3K dev-Twitter + 20K monthly dev-blog readership IS ICP-aligned (devs selling to devs). That is the rare overlap that flips one of the dev-tool channel rules (Section 3) but does NOT flip the marketing-naive default itself. Premise audit (Step 0.5) is load-bearing.

---

# PREMISE-LEVEL FINDINGS BLOCK

> **Triggered:** ≥2 of M0a–M0e failed challenge. See Step 0.5 for full reasoning. Read this BEFORE the tactical sections.

| # | Premise from design doc | Verdict | Cascade |
|---|---|---|---|
| M0a | "Show HN at launch" as primary distribution event | **PARTIALLY SURVIVES** (HN IS the right audience class for a dev-tool — but as the *primary* lever it's a lottery; must pair with docs/SEO + GitHub-as-marketing-surface + the founder's existing dev-blog/dev-Twitter) | Section 3 elevates docs/SEO + GitHub + founder-blog from "auxiliary" to **PRIMARY** channels. Section 5 refuses Show HN as the lone launch event. |
| M0b | "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)" — competitor anchoring | **FAILS** | Two issues: (1) Supabase Auth IS open-source (it's GoTrue fork, MIT) — the design doc has a factual error; (2) no canonical-success comparable was named. The category is crowded (Hanko, SuperTokens, BetterAuth, Keycloak, FusionAuth, ZITADEL, Ory). Section 1 must research canonical-success precedents — Stripe (docs-as-marketing), Supabase (HN+OSS+free-tier), BetterAuth (YC-launched, fastest-growing 13K stars in <2 yrs). |
| M0c | In-scope features assumed to all serve the paying ICP | **INCONCLUSIVE** (only the offered design doc surface is visible — but the $99/mo hosted tier + $0.001/MAU model contradicts the "simpler than Auth0" wedge if the SDK ships with the same enterprise breadth) | Section 2 ICP must split: OSS-DIY user (won't pay) vs. paying hosted-tier user (will pay). Refuse to plan as if they're one segment. |
| M0d | Hosted-tier first-10-customer plan = "GitHub stargazers who upgrade to hosted tier" | **FAILS** | Stars are vanity for purchase intent — only a small fraction of starrers are positioned to influence purchasing (Clarm 2025 data). The selection bias of a free OSS SDK attracts time-rich/money-poor self-hosters. The paying hosted-tier user is a different human: small-team CTO/lead engineer who values "don't want to run Postgres + Redis + JWT rotation" over saving $99/mo. M6 / Section 5 must add a HIGH-TRUST acquisition mechanic (concierge onboarding for first 10 hosted-tier prospects). |
| M0e | Founder dogfooded on themselves (ex-Stripe engineer building auth) — same audience as paying ICP? | **PARTIALLY SURVIVES** (dogfood audience = technical engineer = same class as both OSS and hosted-tier ICP). But sub-mismatch: founder is a *world-class* engineer; the paying hosted-tier ICP is a *median* small-team lead who specifically does NOT want to learn auth deeply. Section 2 calls this out as a sub-mismatch; dogfood expansion to "founder of a 5-person startup who has never read RFC 6749" recommended. |

**Net:** 2 hard fails (M0b, M0d), 2 partial-survives that still cascade (M0a, M0e). The PREMISE-LEVEL FINDINGS BLOCK is load-bearing. Tactical questions (Step 0A) and Section 3/5/6 inherit these findings.

**Single sharpest claim:** *The founder is planning a launch that conflates two ICPs (OSS-DIY users and paying hosted-tier customers) and is anchoring distribution on the segment that won't pay. The marketing plan must split the two ICPs, optimize the OSS surface for the DIY user (because it produces credibility and inbound), and bolt on a DIFFERENT acquisition motion (concierge / vertical-newsletter / podcast-guest) for the paying hosted-tier user.*

---

## Step 0 — Pre-review system audit

### What exists (read from design doc)

- **Product:** AuthForge — open-source auth SDK (MIT) + hosted tier ($99/mo + $0.001/MAU >10K)
- **Distribution plan in doc:** "Show HN + r/programming + integration tutorials"
- **First 10:** "GitHub stargazers who upgrade to hosted tier"
- **Validation gate:** 100 GitHub stars + 5 hosted-tier signups by day 60
- **Differentiation claim:** "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)"

### Marketing artifacts present

- Founder has a **technical blog (~20K monthly readers)** — load-bearing audience asset
- Founder has **~3K dev-Twitter followers** — small but ICP-aligned
- No prior shipped products → no GitHub stars accrued under founder identity (no carryover credibility)
- No landing page mentioned, no newsletter mentioned, no Discord/Slack mentioned

### Web-searched competitive landscape

Full detail in Section 1. Headline findings:

- **Direct competitors (managed):** Auth0 (incumbent, $0.07/MAU at scale), Clerk ($25/mo + $0.02/MAU, just expanded free tier to 50K MAU Feb 2026), WorkOS (enterprise SSO focus), Stytch (acquired by Twilio 2025), Kinde ($25/mo bundle), Descope, FusionAuth, PropelAuth
- **Direct competitors (OSS):** Supabase Auth (GoTrue fork, MIT — the design doc is wrong on this), **BetterAuth (THE hottest comp — 13K stars, YC-launched, "the recommended auth library by Next.js, Nuxt, Astro")**, Hanko (OSS, MIT, "alt to Auth0/Clerk/WorkOS/Stytch"), SuperTokens, Keycloak, Ory, ZITADEL
- **Canonical successes for OSS+hosted dev-tool motion:** Supabase (HN front page 2 days → 80→800 users overnight in spring 2020; integrate-OSS-others-built strategy), Stripe (docs-as-marketing, 7-lines-of-code framing, eng job ladder included docs)
- **The market is crowded.** BetterAuth alone is going to be the hardest competitor — they hit YC, hit 13K stars fast, and are the *recommended* library in the major TS frameworks. AuthForge needs a sharp wedge against BetterAuth specifically — "simpler than Auth0" is not a wedge against BetterAuth.

### Founder audience audit (numeric)

| Surface | Size | ICP-aligned? | Load-bearing? |
|---|---|---|---|
| Dev-Twitter | ~3,000 followers | Yes (engineers follow engineers) | Yes — small but real |
| Personal tech blog | ~20,000 monthly readers | Yes (if dev/backend content) | **YES — the largest asset** |
| Newsletter | Not mentioned (assume 0) | — | Should exist |
| GitHub stars (prior projects) | 0 (no prior shipped products) | — | Gap — no carryover repo credibility |
| Discord/Slack presence | Not mentioned | — | Gap |
| LinkedIn | Not mentioned | — | Probably not load-bearing for dev tool |
| Conference talks / podcast appearances | Not mentioned | — | Gap |

**Net:** ~23K ICP-aligned attention surface — small but real, and unusually high quality (the 20K blog readers, not the 3K Twitter, are the load-bearing asset). This is enough to flip several channel rankings (founder's blog becomes a primary channel) but NOT enough to flip the marketing-naive default — first-time-shipping risk remains.

### Mode selection input (resolved in Step 0B)

Founder has ICP-aligned audience >> 1K threshold AND product is mid-build with an implied 60-day launch gate. Per SKILL Mode A vs C tie-breaker: **Mode A with Section 4 elevated**. Not Mode C (audience-build sprint alone) because a launch playbook is still required.

---

## Step 0.5 — Premise audit

(Five questions, run BEFORE Step 0A. Each verdict cascades into tactical sections.)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis to test) |
|---|---|---|---|
| 1 | Launch platform = Show HN + r/programming | "Distribution Plan" | HN IS right audience class for dev tools (unlike consumer products) — but as the *primary* lever it's a lottery; must pair with compounding surfaces |
| 2 | Audience = "backend engineers building auth into their apps" | "Target users" | Two-ICP problem: OSS-DIY user ≠ paying hosted-tier user. Conflating them produces wrong messaging |
| 3 | Pricing band = $99/mo + $0.001/MAU above 10K | "Distribution model" | Anchored against Auth0 ($1750/mo @ 50K MAU) — but the *paying* ICP for hosted-tier may not be Auth0-displacement; could be Supabase-Auth-graduate or Clerk-graduate, where the band is different |
| 4 | Differentiator = "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)" | "Differentiation" | (a) Supabase Auth IS open-source — factual error. (b) BetterAuth, Hanko, SuperTokens, Keycloak, FusionAuth, Ory all exist. Wedge is weak. |
| 5 | First 10 customers = GitHub stargazers who upgrade | "First 10 customers" | Stars are vanity for purchase intent; star-to-paid conversion is poor without a separate enterprise-touch motion |
| 6 | Validation gate = 100 stars + 5 hosted signups by day 60 | "Validation gate" | Calendar-driven gate (day 60), not PMF-signal-driven. For a hosted tier that depends on retention, "5 signups" is the wrong threshold — should be "5 signups + retained 30 days + 1 expansion to >10K MAU" |

### M0a. Launch-platform audience-class fit

**Question:** Is Show HN + r/programming the right *audience class* for a dev-tool open-source auth SDK?

**Verdict: PARTIALLY SURVIVES.** HN IS the canonical right audience class for OSS dev tools — see Supabase's HN-driven 80→800 user moment, see BetterAuth's YC/HN-driven rise. r/programming is also valid. **BUT**:

- HN as a *primary* lever is a lottery — Hidden Signal base rate for Show HN posts is <5 upvotes. Even with the right audience class, traction is not guaranteed by audience-fit alone — it requires technically-specific copy + code-first link + already-warm trust signals (founder rep, repo stars).
- The plan misses three PRIMARY dev-tool channels per SKILL Section 3 dev-tool motion-class rules: (1) docs-as-marketing / SEO compounding ("Next.js auth with X" tutorials rank long-tail), (2) GitHub-as-marketing-surface (repo health, named adopters, ecosystem of integrations), (3) founder's existing dev-blog/dev-Twitter.

**Cascade:** Section 3 elevates the 3 missing primary channels. Section 5 launch playbook refuses Show HN as the sole event; sequences it AFTER docs/SEO seeding + blog/Twitter warm-up + named adopters in GitHub README.

### M0b. Canonical-success comparable

**Question:** Name the canonical successful product in the OSS-dev-tool-with-hosted-tier motion class. What did they do that AuthForge's plan does NOT?

**Verdict: FAILS.** The design doc names no canonical success — only direct competitors (Auth0, Supabase Auth). Canonical successes for this exact motion class:

1. **Stripe (docs-as-marketing).** Built $95B business with documentation as the primary sales channel. "Seven lines of code" framing. Engineering ladder included documentation contribution. Source: Product Marketing Alliance Stripe playbook. **Delta:** AuthForge plan has "write integration tutorials" — one line — vs Stripe's institutional commitment to docs as the conversion surface.
2. **Supabase (OSS-first → managed-tier).** Forks GoTrue (Netlify's OSS auth), wraps with Postgres-native managed tier. Spring 2020 HN front page 2 days running → 80→800 users overnight. Strategy: integrate proven OSS components, contribute upstream. **Delta:** AuthForge plans to build the SDK from scratch — no upstream-contribution credibility, no integrate-known-good-things story.
3. **BetterAuth (newest comp, fastest growth in category).** YC-backed, 13K GitHub stars, 100K weekly downloads, "recommended auth library" of Next.js / Nuxt / Astro. 5K Discord members. **Delta:** AuthForge plan has no Discord, no plugin ecosystem, no framework-author endorsements. BetterAuth is a year ahead and accelerating — AuthForge needs a wedge BetterAuth cannot easily copy.

**Pricing comparable for the hosted tier:** Clerk's Feb 2026 pricing shift — free tier expanded from 10K → 50K MAU, Pro at $25/mo. **AuthForge's $99/mo for managed instance is 4× Clerk's entry price.** Either there's a justifying feature (named) or the band is wrong.

**Cascade:** Section 1b mandates Stripe + Supabase + BetterAuth comparables. Section 3 names docs-as-marketing as a primary surface. Section 6 questions $99 price point against the Clerk/Kinde/BetterAuth comparables.

### M0c. Anti-feature surface

**Question:** Name 2+ features in scope that contradict positioning ("simpler than Auth0").

**Verdict: INCONCLUSIVE** — only partial feature visibility in the prompt. Speculative anti-feature candidates worth interrogating with the founder:

- **Open-core feature gating** — if hosted-tier-exclusive features (SSO, audit logs, RBAC) are heavy, this contradicts "open-source SDK" branding. Hanko / SuperTokens publish 100% OSS; AuthForge needs a clean line.
- **$0.001/MAU above 10K usage metering** — usage-metering requires phone-home telemetry from the OSS SDK, which contradicts the trust positioning of an OSS auth library. The community will reject this.
- **MCP / programmatic integrations** — for non-Stripe-level founders, this is a v2 distraction.

**Cascade:** Add to founder Q&A. Document any features ≥1 stakeholder can't justify against "simpler than Auth0."

### M0d. Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the planned acquisition tactic ("GitHub stargazers who upgrade to hosted tier") select for the wrong segment?

**Verdict: FAILS.** Two-segment problem:

- **OSS SDK adopters (free)** = time-rich/money-poor self-hosters. They will star the repo and run the SDK on their own infra. They will NOT upgrade to $99/mo hosted tier because they enjoy not paying for infra they can run themselves.
- **Hosted-tier paying customers** = time-poor/money-rich small-team CTO/lead. They specifically do NOT want to run Postgres + Redis + JWT-key-rotation for auth. They are NOT typically starring auth repos for fun — they evaluate, decide, and integrate. **They reach AuthForge from a Stripe-style docs hit + integration tutorial, NOT from a GitHub star.**

The validation gate ("100 stars + 5 hosted signups") conflates the two segments. Stars are the OSS-DIY signal; hosted signups are a different funnel entirely.

**Cascade:** Section 2 splits the two ICPs. Section 5 launch playbook adds a SEPARATE high-trust acquisition mechanic for the paying ICP — concierge onboarding for first 10 hosted prospects (Superhuman / Vohra precedent) PLUS Stripe-style docs + integration tutorial SEO seeding. Section 8 metrics treat star-count as a vanity metric for the paying funnel.

### M0e. Dogfood audience-class match

**Question:** Did the founder dogfood on the same audience that will buy hosted tier?

**Verdict: PARTIALLY SURVIVES with sub-mismatch.** Founder is ex-Stripe engineer building auth → dogfood audience class is "expert backend engineer." Both OSS-DIY ICP and paying hosted-tier ICP are also engineers, so the high-level class matches. **But:**

- Founder is a *world-class* engineer with deep auth knowledge. The paying hosted-tier ICP is a *median* small-team lead who explicitly does NOT want to learn auth deeply.
- This means the SDK API and docs may be calibrated for the wrong sub-segment. A median engineer wants "do the right thing by default" and "I should not have to read RFC 6749." A world-class engineer wants "expose all the knobs."
- Per SKILL M0e, the correct fix is BOTH PIVOTS: (a) re-target marketing to the median small-team lead, NOT the auth-fluent expert; (b) expand dogfood to include a paying-ICP-representative subject (e.g., paid concierge-onboard 2 small-startup CTOs in the next 2 weeks, watch them integrate, fix what trips them up). The wrong fix is to keep the expert-tuned API and defer the median-engineer audience.

**Cascade:** Section 2 ICP doc is calibrated to the median small-team lead. Section 4 audience-build adds 2 paying-ICP-representative concierge-dogfood sessions BEFORE launch.

### Step 0.5 verdict summary

| # | Verdict | Cascades into |
|---|---|---|
| M0a | Partial-survives | Section 3 (elevate docs/SEO + GitHub + founder-blog), Section 5 (refuse Show HN as sole event) |
| M0b | **FAILS** | Section 1b (Stripe + Supabase + BetterAuth comparables), Section 3, Section 6 (pricing band) |
| M0c | Inconclusive | Founder Q&A; document features that can't be justified |
| M0d | **FAILS** | Section 2 (split ICPs), Section 5 (concierge motion for paying ICP), Section 8 (don't conflate funnels) |
| M0e | Partial-survives with sub-mismatch | Section 2 (target median engineer), Section 4 (concierge-dogfood sessions) |

≥2 hard fails → PREMISE-LEVEL FINDINGS BLOCK promoted to top of doc (done).

---

## Step 0A — Forcing questions (M1–M7)

Asked one at a time. Founder answers simulated per "technically strong, marketing-naive" posture.

### M1. Audience reality

**Q:** Name a specific person who would actively seek out AuthForge. Where do they hang out RIGHT NOW?

**Founder's first answer (rejected):** "Backend engineers building auth into their apps."

→ Refused: demographic category, no specific person, no places.

**Founder's second answer (accepted):**

> *"Marcus, 32, CTO/co-founder of a 4-person YC W26 SaaS startup. TypeScript + Postgres stack on Vercel + Supabase. Currently using Supabase Auth but hitting limits (custom claims, B2B org switching). Reads: Pragmatic Engineer (subscribes), HackerNews daily, Theo.t3.gg YouTube, @leerob on Twitter. Hangs out: Vercel Discord, the YC Slack, r/nextjs, r/SaaS. Recently complained on Twitter about Auth0 enterprise pricing creep."*

5 attributes named, 3+ places named.  But: the **OSS-DIY ICP** is a DIFFERENT person — name them too:

> *"Priya, 28, senior backend engineer at a 50-person fintech. Self-hosts everything for compliance reasons. Reads: lobste.rs, HN, /r/golang, /r/rust. Will never pay for hosted auth — but will star the repo if it's clean and integrate it at work, becoming an internal champion."*

**Accepted.** Two ICPs documented. `icp.md` will codify both.

### M2. Discovery path

**Q:** Walk through specific path Marcus (paying ICP) takes to discover AuthForge. Min 3 steps. Step 1 is NOT "sees my Show HN."

**Founder's first answer (rejected):** "He sees my Show HN post."

→ Refused per skill.

**Founder's revised path (accepted):**

1. Marcus hits a custom-claims limit in Supabase Auth on a Tuesday afternoon. Googles `"supabase auth custom claims b2b organization"`.
2. Lands on an integration tutorial on the founder's existing tech blog: *"Migrating from Supabase Auth to AuthForge for B2B org claims"* (SEO-targeted; written 60 days before launch).
3. The tutorial links to the GitHub repo. Marcus sees 800+ stars, named adopters in README (because founder did the work to get them), and a 10-minute integration test.
4. Marcus tries the SDK locally Saturday morning. Posts a question in the AuthForge Discord. Founder responds personally in 2 hours.
5. By Wednesday, Marcus's team is evaluating the $99/mo hosted tier vs self-hosting. CTO judgment: "$99/mo is cheaper than the eng-hours to rotate JWT keys monthly."

Time-to-discovery: weeks, not "eventually." Specific channel (founder's blog SEO → GitHub → Discord). Specific intermediary (the integration tutorial). **Accepted.**

For Priya (OSS-DIY ICP), the path is shorter: lobste.rs/HN frontpage of an integration tutorial → repo → integration → no purchase, but she stars the repo and pitches it internally over the next 6 months.

### M3. Pre-launch audience

**Q:** Show numeric evidence of existing audience.

**Founder's answer:**
- 3,000 dev-Twitter followers
- 20,000 monthly readers on tech blog
- 0 newsletter subscribers (no list)
- 0 Discord members (no community)
- 0 GitHub stars on prior projects (no prior shipped product)

**Accepted with caveat:** the 20K blog audience is the largest asset and is ICP-aligned IF blog content is dev-backend-focused (verify before launch — if it's about Rust language internals, less ICP-aligned than if it's about distributed systems / payment infra). Founder confirms it's primarily backend / Stripe-era distributed systems content → ICP-aligned. The 3K Twitter is solid but small. **Gap:** no newsletter (means no owned distribution outside platform algorithms). **Gap:** no Discord (means no community surface for trust/eval).

### M4. Channel honesty

**Q:** Name ONE distribution channel where you have a credible advantage over a generic founder.

**Founder's answer:** "My tech blog. 20K monthly readers, consistent for 3 years, mostly senior backend engineers."

**Accepted** — this is real and verifiable. The blog is the load-bearing distribution asset. Most founders launching in this category have nothing close to this. Treat as primary channel.

### M5. Competitor traffic source

**Q:** Where do BetterAuth, Clerk, Supabase Auth get their users?

**Founder's first answer (rejected):** "I don't know."

→ Refused without commitment.

**Founder's revised answer (accepted):**

- **BetterAuth:** YC launch announcement, framework-author endorsements (Next.js, Nuxt, Astro recommending), Twitter virality (@imbhargav5 founder thread), GitHub trending, Discord-driven community advocacy. Will research SimilarWeb before next session.
- **Clerk:** Heavy paid search ("nextjs auth"), partner integrations (Vercel, Next.js docs), developer-focused video content (YouTube), strong React UI components as the wedge.
- **Supabase Auth:** Pulled along by Supabase platform (Postgres + Auth + Storage + Edge Functions). HN spike in 2020 (Y Combinator W20). Self-hosting+managed-tier symmetry. Distribution is bundled with the larger Supabase platform — not an apples-to-apples comp for a pure-auth SDK.

Accepted with assignment to verify SimilarWeb data before Section 1 finalization.

### M6. First 10 paying customers

**Q:** Name the specific path to first 10 paying hosted-tier customers. Not "viral on HN."

**Founder's first answer (rejected):** "GitHub stargazers who upgrade to hosted tier" (from design doc).

→ Refused — per M0d, stars-to-paid is the wrong funnel. Star-only signal is vanity for purchase intent.

**Founder's revised plan (accepted):**

1. **Personal network first (3-4 customers):** Email 25 people from the ex-Stripe network + YC personal connections + 5 specific Vercel Discord regulars Marcus knows by handle. Offer free 6-month hosted tier in exchange for being a named adopter in the README. Target: 3 acceptances.
2. **Concierge from blog conversion (3-4 customers):** Write 3 integration tutorials targeted at "Supabase Auth user hitting B2B limits" / "Auth0 user looking to cut costs" / "Clerk user evaluating self-host fallback." Each tutorial closes with "30-min concierge integration call — book here." Target: 3 calls → 3 hosted-tier converts.
3. **Vertical Discord targeted outreach (2-3 customers):** Be helpful (not spammy) in Vercel Discord, Bun Discord, Hono Discord for 30 days pre-launch. Answer auth questions. Get known. After launch, mention in context where helpful. Target: 2 hosted converts.

Total: 8-10. Names 25+ specific humans for step 1. Specific communities. Concrete sequence. **Accepted.**

### M7. Time allocation

**Q:** % time pre-launch on audience-building vs building?

**Founder's first answer (flagged):** "Maybe 10%. I have a lot of building to do."

→ Skill challenges: 10% is the wrong ratio.

**Founder's revised plan (accepted with risk flag):**

- 40% on building (down from 100%)
- 30% on **integration tutorials + blog SEO seeding** (this is BOTH audience-build AND content the paying ICP needs at discovery — dual-purpose)
- 15% on **named-adopter outreach** for README (specific email campaign, ~25 people)
- 10% on **community presence** (Vercel Discord, Bun Discord, lobste.rs, HN — show up, don't pitch)
- 5% on **first-10-customer concierge prep** (intake forms, calendly, onboarding script)

60% on non-building activity. Explicitly acknowledged as a major shift from "I'll start marketing after launch" plan. **Accepted with risk flag:** if founder reverts to >70% building, plan fails by day 30. Section 9 lists this as the single highest founder-side execution risk.

### M1–M7 completion summary

All 7 answered concretely. Gaps surfaced: no newsletter, no Discord, no GitHub repo carryover, no SimilarWeb verification yet (assigned). Proceed to mode selection.

---

## Step 0B — Mode selection

**Selected: Mode A (Full Marketing Review) with elevated Section 4 (audience-build sprint embedded).**

Reasoning:
- Founder has ≥1K ICP-aligned attention surface (20K blog readers + 3K Twitter) → meets Mode A threshold.
- Product is mid-build with an implied 60-day launch gate (validation: 100 stars + 5 signups by day 60) → tie-breaker per SKILL rule: prefer Mode A with elevated Section 4 over Mode C alone, because Mode C alone skips the launch playbook the founder still needs.
- Section 4 elevated because newsletter=0, Discord=0, GitHub-prior-stars=0 — three distribution surface gaps that need concrete 30/60/90 cadence even though the audience as a whole exceeds the Mode A threshold.

Runs all 9 sections. `marketing_plan.md` is canonical artifact; `icp.md`, `launch_playbook.md`, `audience_build_journal.md` as supporting.

---

# Section 1 — Competitive landscape

## 1a. Direct competitors

| Name | Founded | Pricing | Apparent traffic sources | User complaints | Their wedge | Winning? |
|---|---|---|---|---|---|---|
| **Auth0** (Okta) | 2013 | $0.07/MAU; ~$1,750/mo @ 50K MAU, $5,250/mo @ 100K MAU. B2C Essentials gates >20K MAU behind sales calls. | Enterprise sales, partner channel, paid search, Okta acquisition channel | "Pricing creep — 5-10× over 3 yrs"; "every checkbox costs more"; "MAU model penalizes growth" | Enterprise CIAM breadth | Stagnant — losing dev mindshare to Clerk/Supabase/BetterAuth |
| **Clerk** | 2020 | Pro $25/mo + $0.02/MAU; free 50K MAU (post-Feb-2026 update). $25 + 40K×$0.02 = $825/mo @ 50K MAU | Heavy paid search ("nextjs auth"), partner integrations (Vercel, Next.js docs), YouTube, founder Twitter | "Pricing was confusing pre-2026" (fixed); "React-only UI" (true) | React-first UI components, best DX | **Winning** — growing fast, best DX in category |
| **Supabase Auth** | 2020 | Bundled w/ Supabase; $0.00325/MAU on Pro; free 50K MAU | Pulled by Supabase platform, HN 2020 spike, OSS-fork of GoTrue, Postgres-native | "Tied to Postgres"; "no RBAC built-in"; "B2B org-switching is hard" | Postgres-native, cheapest at scale, full-platform | **Winning** in the Postgres lane; weak outside it |
| **WorkOS** | 2019 | $125/enterprise-connection/mo (SSO); free for first 1M MAU on AuthKit | Enterprise sales, content marketing (workos.com/blog), partner relationships | "Pricing flips at enterprise"; "less DIY-friendly" | "Make your app enterprise-ready" SSO/SCIM/audit | Winning the B2B enterprise-readiness lane |
| **Stytch** | 2020 | API-first, usage-based | API-first content, founder Twitter | Acquired by Twilio 2025 — uncertain direction | Programmatic control, fraud/bot tooling | Uncertain post-acquisition |
| **BetterAuth** | 2024 | OSS (MIT), self-host free | YC launch, framework-author endorsements (Next.js, Nuxt, Astro), Discord community (5K members), GitHub trending | "Fast-moving — breaking changes"; "still young" | "The recommended auth library" for TS frameworks | **Winning fastest — biggest direct threat to AuthForge** |
| **Hanko** | 2022 | OSS (MIT) + paid Cloud | GitHub, content, passkey-positioning | "Smaller community" | Passwordless / passkey-first, OSS | Growing in passwordless lane |
| **SuperTokens** | 2020 | OSS (Apache 2) + paid managed | Content, GitHub, dev forums | "Self-host complexity" | OSS-first, self-host with managed option | Steady; lost mindshare to BetterAuth |
| **Kinde** | 2023 | $25/mo bundle (orgs, RBAC, MFA, social, flags) | Australia founder network, content | Newer | "Cheaper than Clerk, more bundled" | Growing in early-stage SMB |
| **Keycloak** | 2014 | OSS (Apache 2), self-host only | Enterprise IT, JBoss-era inheritance | "Java-heavy, ops-heavy" | Enterprise OSS IdM | Stable in enterprise self-host |
| **FusionAuth** | 2016 | OSS Community + paid Enterprise | Content, conferences | "Less modern DX" | OSS + paid; self-host friendly | Stable niche |
| **Ory** / **ZITADEL** | — | OSS + Cloud | Cloud-native positioning | "Steep learning curve" | Cloud-native IdM | Niche but growing |

**Honest read:** the category is crowded. BetterAuth is the single biggest threat — they have YC distribution, framework-author endorsements, 13K stars and accelerating. Clerk is the dominant DX leader. Supabase Auth is the cheapest. **AuthForge cannot win on "open-source unlike Auth0/Supabase Auth" (Supabase Auth IS open source, and 6 other OSS options exist).** Wedge must be different.

## 1b. Canonical-success comparables

| Name | Founded | Price | Scale | Primary acquisition channel | Onboarding model | Launch gate | Delta vs AuthForge plan |
|---|---|---|---|---|---|---|---|
| **Stripe** | 2009 | Usage-based (2.9% + $0.30) | $95B valuation | **Docs-as-marketing**; "7 lines of code"; engineering ladder requires doc contribution; SEO compounding on every payment API query | Self-serve via docs; concierge for enterprise | Private beta to "Collison-brother personal network" before broad launch | AuthForge has "write integration tutorials" — one line. Stripe institutionalized docs as the conversion surface. AuthForge plan does NOT make docs the central conversion mechanism. |
| **Supabase** | 2020 | Free 50K MAU + $25/mo Pro | $2B valuation | HN front page Apr 2020 (2 days running, 80→800 users overnight); OSS-integration story (GoTrue+PostgREST+pgvector); Postgres-native wedge; YC W20 | Self-serve hosted + self-host OSS | YC W20 demo day + HN moment | AuthForge plan has "Show HN" — but no platform-integration story, no upstream-OSS-contribution credibility, no YC distribution. Needs replacement compounding loop. |
| **BetterAuth** | 2024 (YC) | OSS, MIT | 13K stars, 100K weekly downloads in ~18 months | YC launch announcement; framework-author endorsements (Next.js / Nuxt / Astro recommending); Twitter virality (founder thread); Discord community (5K); GitHub trending; plugin ecosystem | Self-serve docs; Discord support | Open-source first, hosted/paid TBD | AuthForge plan has no Discord, no plugin ecosystem, no framework endorsement strategy. BetterAuth is the direct precedent for "what to do" AND the direct competitor.  AuthForge must define what wedge BetterAuth cannot replicate. |
| **Vercel** (dev infra exemplar) | 2015 | Free hobby + $20/mo Pro | $3B+ valuation | Next.js author employed (Guillermo Rauch hired Tim Neutkens); framework-as-distribution; HN/Twitter via founder; conference content | Self-serve with concierge for enterprise | Continuous (no single launch event) | AuthForge has no framework-author leverage. Closest analog: become the default for a rising TS framework (Bun? Hono? Effect?) before the framework becomes mainstream. |

## 1c. Pattern surface

**What the canonical successes have in common that the AuthForge plan lacks:**

1. **Docs are the conversion surface, not a side artifact.** Stripe and Supabase both made documentation the central marketing investment. AuthForge plan mentions "integration tutorials" once. This is the single highest-leverage gap to close pre-launch.
2. **An integration ecosystem creates the network effect.** BetterAuth has plugin ecosystem; Stripe has framework SDKs in every language; Supabase integrates the OSS components devs already trust. AuthForge plan has no plugin / integration strategy.
3. **Community surface (Discord) is load-bearing for OSS dev tools.** BetterAuth's 5K Discord is the trust-evaluation surface. AuthForge plan has none.
4. **Named adopters in README are evaluative oxygen.** Supabase had Mozilla / GitHub references early; BetterAuth has Next.js endorsement. AuthForge plan has none yet (founder must do this work pre-launch).

**Where direct competitors diverge from canonical-success patterns:**

- Auth0 grew on enterprise sales motion, not OSS or dev-DX. Not a precedent AuthForge should copy.
- Clerk grew on paid search + best-in-class React UI. Could be copied IF AuthForge has the UI investment to match (probably not for a solo founder).

**Which pattern is the current plan implicitly following — and is it the right one?**

The plan implicitly follows the **single-channel HN-lottery pattern** that consistently fails for crowded OSS categories without compounding surfaces. The right pattern is the **Stripe-Supabase docs-and-integrations compounding pattern**, sequenced so the docs/SEO/integration corpus exists BEFORE the HN moment, so HN drives traffic into a converting surface rather than a landing page.

**Founder action:**
- Study Patrick Collison's interviews + Stripe blog history → extract the docs-as-marketing lessons.
- Study Paul Copplestone's Supabase founder narratives → extract the "integrate proven OSS, contribute upstream" playbook.
- Study Bekacru Solomon (BetterAuth founder) Twitter + YC launch interview → understand what they did in the first 90 days that AuthForge can adapt.

---

# Section 2 — ICP specification (→ `icp.md`)

**Two ICPs, not one. Conflating them is the M0d failure mode.**

## ICP-A: "Marcus" — paying hosted-tier user

- 32 yo CTO/co-founder of 4-12-person SaaS startup
- Stack: TypeScript + Next.js + Postgres on Vercel + Supabase (or similar)
- Currently using Supabase Auth, Clerk, or rolling-their-own; hit a B2B / multi-org / custom-claims wall
- Reads: Pragmatic Engineer, HackerNews, Theo.t3.gg, @leerob, @rauchg, @t3dotgg
- Hangs out: Vercel Discord, YC Slack, r/nextjs, r/SaaS, Bun Discord
- Pays for: Cursor ($20/mo), Linear ($8/seat), Vercel Pro ($20/mo), Supabase Pro ($25/mo), Resend ($20/mo), Clerk Pro ($25/mo if they're already on it)
- Complains about (in adjacent categories): Auth0 pricing creep; Clerk's React-only UI when they want Vue/Svelte; Supabase Auth B2B limits
- Objections to AuthForge: "Why would I switch from Clerk? It works.", "Why pay $99 when Clerk is $25?", "I don't want to migrate auth — it's the riskiest migration"
- Reasons to convert: framework-agnostic (vs Clerk React-only), open-source escape hatch (vs Clerk lock-in), B2B-first design (vs Supabase Auth), cheaper at scale (vs Auth0), simpler than running Keycloak

## ICP-B: "Priya" — OSS-DIY adopter (will NOT pay)

- 28 yo senior backend engineer at 50-person fintech or regulated-industry company
- Stack: Go or Rust, self-hosted everything, compliance-driven
- Reads: lobste.rs, HN, /r/golang, /r/rust, /r/selfhosted
- Hangs out: lobste.rs comments, GH issues threads
- Pays for: almost nothing personally; advocates for OSS internally
- Complains about (in adjacent categories): Auth0 "$15K bills for what should be free"; managed services going down; data-residency requirements
- Objections to AuthForge: "Is this just open-core with the good stuff locked behind paid?", "What's the license? Will it switch to BSL later?"
- Reasons to convert (to advocate, not pay): Clean SDK, clear MIT license, can self-host without phone-home telemetry, named upstream contributors

**Strategy:** ICP-B is the OSS-credibility and star-growth surface (drives evaluative trust signals that ICP-A reads when deciding). ICP-A is the revenue surface. The marketing plan must serve BOTH simultaneously without confusing the messaging:

- **OSS landing page + README:** speak to Priya (MIT, no phone-home, plugin ecosystem, self-host docs).
- **/pricing and /hosted landing page:** speak to Marcus (concierge onboarding, B2B-first, "your engineers don't want to rotate JWT keys").
- **Discord:** serves both — Priya answers questions for Marcus's team; founder builds reputation for both.

Output: `icp.md` codifies both personas in full.

---

# Section 3 — Distribution channels (dev-tool motion-class rules applied)

Per SKILL Section 3 dev-tool rules: docs/SEO + GitHub + founder's existing dev-audience are **PRIMARY**, not auxiliary. HN/Reddit are right audience class but not standalone. Marketing-speak tone is INVERSELY correlated with traction.

## Channel scoring table

(Score 1-5; reach × conversion × founder fit / cost / effort)

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Leverage | Status |
|---|---|---|---|---|---|---|---|
| **Founder's tech blog (existing 20K/mo)** | 5 | 1 | 4 (warm, ICP-aligned) | 5 | 2 (already cadenced) | **HIGHEST** | **PRIMARY — load-bearing** |
| **Docs-as-marketing / integration tutorials SEO** | 4 (long-tail compounding) | 1 | 4 (high-intent search) | 4 (founder can write) | 4 (must produce 8-12 quality tutorials) | **VERY HIGH** | **PRIMARY (Stripe precedent)** |
| **GitHub as marketing surface (repo health, named adopters, plugin ecosystem)** | 4 (developers research repos) | 1 | 3 (eval-stage trust signal) | 4 | 4 (community work) | **VERY HIGH** | **PRIMARY (per SKILL dev-tool rule)** |
| **Founder's dev-Twitter (3K)** | 2 (small) | 1 | 3 | 5 | 2 | High for trust | **PRIMARY (warm)** |
| **Show HN (launch event)** | 5 if hits, 0 if miss | 1 | 4 (right audience class) | 4 (technical founder) | 2 (one post, but rehearsed) | High EV-weighted but lottery | **SECONDARY** — sequenced AFTER warm surfaces |
| **r/programming + r/golang + r/rust + r/typescript + r/selfhosted** | 3 | 1 | 3 | 4 | 2 (compliant posts, no spam) | Medium-high | **SECONDARY** |
| **lobste.rs** | 2 | 1 | 4 (senior eng audience) | 4 | 2 | Medium | **SECONDARY** |
| **Pragmatic Engineer / vertical dev newsletters** | 4 | 4 (sponsorship) or 5 (guest post) | 4 | 3 (depends on relationship) | 5 | High if landed | **SECONDARY — high-leverage** |
| **Podcast guesting (Software Engineering Daily, Changelog, JS Party, Syntax)** | 3 | 1 | 4 (deep-context audience) | 4 | 4 (research, pitch, prep) | Medium-high | **SECONDARY** |
| **Vercel Discord / Bun Discord / Hono Discord (community presence)** | 2 (small, targeted) | 1 | 5 (warm, intent-revealing) | 5 | 3 (sustained presence) | High per-touch | **PRIMARY for ICP-A reach** |
| **YouTube (technical screencasts)** | 3 | 1 | 4 | 2 (no track record) | 5 (very high) | Low for THIS founder | **SKIP for v1; revisit post-launch** |
| **LinkedIn organic** | 2 (B2B dev is weak on LinkedIn) | 1 | 2 | 2 | 3 | Low | **SKIP** |
| **IndieHackers** | 2 | 1 | 2 (SMB SaaS, not infra) | 3 | 2 | Low for THIS product | **SKIP** |
| **Product Hunt** | 3 (different audience than HN) | 1 | 2 (designer/PM heavy) | 3 | 3 (need hunter) | Medium — separate event | **SECONDARY — sequenced 7 days post-HN** |
| **Paid ads (Google "nextjs auth")** | 4 | 5 ($8-15 CPC for auth keywords) | 3 | 2 | 4 | Low ROI without revenue | **SKIP for v1; revisit if hosted-tier signups validate** |
| **Cold email outreach (to YC W26 cohort, named-adopter ask)** | 3 (targeted) | 1 | 4 (warm via founder identity) | 4 | 3 | High for first-10 work | **PRIMARY for first-10 customer plan** |
| **Affiliate** | 1 | 1 | 1 | 1 | 2 | None | **SKIP — premature** |

## Top channel ranking for AuthForge (v1)

**PRIMARY (do these — non-negotiable):**

1. **Founder's tech blog as the integration-tutorial publishing surface** — 8-12 tutorials pre-launch targeting `[framework] + auth + [pain]` queries
2. **Docs as conversion surface** — make `docs.authforge.dev` the Stripe-quality landing for every framework
3. **GitHub repo as evaluative surface** — pre-launch named adopters, plugin ecosystem v0.1, contributor recognition
4. **Founder's dev-Twitter for warm distribution of every tutorial / GitHub update**
5. **Vercel / Bun / Hono Discord community presence** — 30 days pre-launch sustained, not pitchy
6. **Cold email to specific 25 ex-Stripe + YC W26 contacts for named-adopter list**

**SECONDARY (do these in sequence at launch):**

7. **Show HN** (sequenced — see Section 5)
8. **r/programming + r/golang + r/typescript** (compliant, founder-led)
9. **lobste.rs** (one-shot, follow community norms)
10. **Pragmatic Engineer / Lenny / SED podcast guest** (pitched at day 14 post-launch)

**SKIP for v1:** Paid ads, LinkedIn, IndieHackers, YouTube, Affiliate, Product Hunt-as-primary.

## Dev-tool tonal rule (LOAD-BEARING for Section 5)

Per SKILL — Show HN / r/programming / lobste.rs / dev-Twitter copy MUST NOT use:

- "revolutionary" / "best-in-class" / "enterprise-grade" / "world-class" / "game-changing" / "seamless" / "robust"
- Benefit-led hero copy without technical specifics
- Marketer-vocabulary phrasing

Copy MUST:

- Lead with technical specifics (e.g., "Framework-agnostic auth SDK in TypeScript, JWT + session hybrid, ~3K LOC core, plugin architecture for OAuth providers")
- Include honest negatives ("Worse than Clerk if you only need React + want pre-built UI. Worse than Supabase Auth if you're already on Supabase. Better than both if you're framework-pluralist or need self-host parity with managed.")
- Link to the GitHub repo BEFORE the marketing landing page on HN/Reddit/lobste.rs
- Read as "engineer wrote this for engineers"

**Anti-pattern flagged for the founder:** instinct as ex-Stripe-engineer will be to write Stripe-marketing-quality copy. For Show HN, that reads as adversarial. The right tone is closer to a thoughtful internal Slack message from a senior engineer than a Stripe landing page.

---

# Section 4 — Pre-launch audience-build (ELEVATED)

30/60/90 plan. Section is elevated per Mode A tie-breaker — gaps (no newsletter, no Discord, no GitHub-prior-stars) need closing.

## Day 1-30 (audience seeding)

**Weekly cadence:**

- **2× integration tutorial / week** on founder's existing blog (total 8 tutorials). Topics SEO-targeted:
  1. "Migrating from Supabase Auth to AuthForge for B2B org claims"
  2. "Next.js + AuthForge: 10-minute integration"
  3. "Bun + AuthForge: framework-agnostic auth without React"
  4. "Hono + AuthForge: edge-deployed auth"
  5. "Replacing Auth0 with AuthForge: cost & migration walkthrough"
  6. "Self-hosting AuthForge: Postgres + 1 binary, no Redis"
  7. "B2B multi-tenant patterns in AuthForge"
  8. "AuthForge vs Clerk vs BetterAuth: honest comparison" (the must-write piece — link to all comp repos, name where AuthForge is worse)
- **2× Twitter thread / week** — technical, not promotional. E.g., "5 things I learned shipping JWT rotation in production at Stripe"
- **Discord launch — week 1.** Empty Discord with 3 channels (#general, #show-and-tell, #help). Founder seeds initial messages.
- **Newsletter launch — week 1.** Founder's existing blog readers prompted to subscribe to "AuthForge & auth-engineering newsletter" — capture intent. Target: 500 subs by day 30.
- **Cold email to 25 named-adopter prospects** (ex-Stripe + YC W26 + Vercel Discord regulars). Offer 6mo free hosted tier in exchange for README placement. Sent in batches of 5/wk. Target: 5 acceptances by day 30.
- **Lurk in 3 Discords (Vercel, Bun, Hono).** Answer questions, do not pitch. Goal: be recognized name by day 30.

**Day 30 measurable gates:**
- 8 tutorials shipped
- 500 newsletter subs (founder converts ~2.5% of monthly blog readers — realistic)
- 100 Discord members
- 5 named adopters confirmed (committed to README)
- 200 GitHub stars (organic from blog traffic + tutorials linking to repo)

## Day 31-60 (cadence + warmup)

- **1× integration tutorial / week** (cadence cools as launch nears; depth increases)
- **3× Twitter thread / week** (cadence increases as launch nears)
- **1× substantive PR or contribution** to a framework's auth docs (Next.js, Hono, Bun) per week — get the framework author's recognition
- **Discord office hours** weekly — founder shows up Wednesday 4-5pm PT, answers anything
- **Newsletter:** weekly issue with build-in-public + tutorial of the week
- **Podcast pitches** — pitch 8 podcasts (Changelog, SED, JS Party, Syntax, Practical AI, ThePrimeagen stream, Theo.t3.gg, Lenny). Target: 2 booked recordings for ~3 weeks post-launch.
- **Named adopters: target 10 confirmed for README** by day 60.
- **Concierge dogfood: 2 paid concierge sessions** with small-startup CTOs from the YC W26 cohort (per M0e fix). Watch them integrate. Fix what trips them. This calibrates the SDK toward ICP-A (median engineer), not just the founder (world-class engineer).

**Day 60 measurable gates:**
- 1,200 newsletter subs
- 250 Discord members
- 10 named adopters (logos in README + landing page)
- 600 GitHub stars (sustained from tutorial SEO)
- 2 framework auth-docs contributions merged
- 2 podcast recordings scheduled

## Day 61-90 (launch integration)

Launch is sequenced within this window per Section 5. Audience-build narrows into launch comms:

- **3× launch-comms posts / week** across blog + Twitter
- **Discord goes from quiet → high-engagement** — founder live for first 72 hours post-launch
- **Daily metrics dashboard** posted publicly (build-in-public — Pieter Levels precedent)

Output: `audience_build_journal.md` template with weekly check-in fields.

---

# Section 5 — Launch playbook (→ `launch_playbook.md`)

## 5a. Question the launch gate BEFORE the playbook

**Required question per SKILL:** What gate fires the launch? Calendar (day 60) or PMF-signal?

**Design doc gate:** "100 GitHub stars + 5 hosted-tier signups by day 60." This is calendar + count gate. It is **PARTIALLY WRONG.**

- **GitHub stars as a gate** = vanity for hosted-tier purchase intent (per M0d). Stars are appropriate for OSS-credibility tracking but NOT as a launch trigger.
- **5 hosted-tier signups as a gate** = better, but should add retention dimension. "5 signups" can be a paid-trial spike that all churn at day 30.

**Recommended gate (replacement):**

| Signal | Threshold | Why |
|---|---|---|
| Concierge-onboard signal (M0d-aligned) | Founder personally onboarded 5 ICP-A prospects who report dependence after 14 days | This is the Vohra/Superhuman precedent. Retention-driven hosted tier; "very disappointed" test fits. |
| OSS credibility floor | ≥250 GitHub stars from organic discovery (blog traffic, not gamed) | Stars matter for evaluation trust — but as a floor, not a gate. Below this, Show HN reads as low-credibility. |
| Doc surface threshold | ≥8 integration tutorials live and ranking on at least 3 long-tail queries | Stripe precedent — docs must convert before the launch traffic spike, not after. |
| Named adopter floor | ≥5 logos in README (real adopters who shipped to prod) | Evaluation trust signal. |

If all four met → launch. If only calendar met but signals weak → DELAY launch and continue audience-build / concierge. This is a meaningful departure from the design doc's calendar gate and the founder should defend if pushing back.

**Specific founder pushback to anticipate:** "I have a finite runway / I need to ship by day 60." Acceptable IF the founder commits that "launching with weak signals will be a soft launch, not a moment-launch — no HN, no PR push, just OSS release + tutorial + Discord open." A soft launch buys time to hit signals without burning the HN moment.

## 5b. Sequenced launch playbook

Assumes signals met by day 60. If not, soft-launch instead.

| Day | Channel | Specific action | Risk if missed |
|---|---|---|---|
| -30 | Audience-build | Continue tutorial cadence (Section 4) | Low |
| -14 | Personal email | Founder emails 100-person personal list (ex-Stripe + YC peers + tech-blog newsletter VIPs): "Here's what I'm launching in 2 weeks. Want early access?" | Med — sets warm cohort |
| -7 | Twitter | Build-in-public thread previewing launch (no link yet — tease) | Low |
| -7 | Newsletter | "AuthForge launches in a week — here's why I built it" (links: tutorial corpus, GitHub repo for early access) | Low |
| -3 | Discord | Pin announcement; invite first 20 named adopters to share their stories | Low |
| -3 | GitHub | Tag v1.0.0 release; cut release notes that are technical + honest (lead with what's stable, name what's beta) | Med — release-note credibility is read by HN audience |
| 0 (Tuesday 6:30am PT) | Hacker News | Show HN: AuthForge — TS-first framework-agnostic auth SDK + optional hosted tier | **Highest single-event risk** |
| 0 + 30 min | Founder | Live in HN comments — engineer-tone, honest, link to GitHub before landing page | Critical for retention on front page |
| 0 + 2hr | Twitter | Thread linking HN discussion (NOT direct link to product) — pulls Twitter audience into HN | Med |
| 0 + 4hr | r/programming + r/typescript + r/golang | Compliant cross-post (follow each sub's rules; no duplicate-content sin) | Med — bans possible if rules ignored |
| 0 + 6hr | lobste.rs | One-shot post (follow lobste.rs norms — no marketing copy) | Med — lobste.rs audience is high-quality, hostile to marketing |
| 0 + 8hr | Discord | "We're live" announcement; founder camps in #general for next 24hr | Low |
| 0 + 24hr | Newsletter | Launch retrospective email — "what's working, what's broken, what's next" | Low |
| 0 + 48hr | IndieHackers | Cross-post (low priority — different audience) | Low |
| 0 + 7d | Product Hunt | Separate launch event (different audience, hunter relationship needed) | Med — recruit hunter pre-launch |
| 0 + 14d | Podcast outreach activation | First scheduled podcast records (booked at day 30-60) | Low |
| 0 + 30d | Substack / blog | "30 days post-launch" retrospective with traction numbers + lessons | Low |

**Show HN copy template (dev-tool tonal rules applied):**

> **Show HN: AuthForge — framework-agnostic TypeScript auth SDK with optional hosted tier**
>
> Hi HN. I'm [name], ex-Stripe (worked on [specific team]). Spent the last 4 months building AuthForge because every existing TS auth library forced a tradeoff I didn't want.
>
> What it is: ~3K LOC core, MIT, framework-agnostic (Next.js / Hono / Bun / Express adapters), JWT + session hybrid, plugin architecture for OAuth/SAML/passwordless. Self-host (one binary + Postgres, no Redis) or use the hosted tier ($99/mo + $0.001/MAU >10K).
>
> Where it's worse than the alternatives:
> - Worse than Clerk if you only need React and want pre-built UI components (Clerk's UI is genuinely better).
> - Worse than Supabase Auth if you're already on Supabase — no reason to migrate.
> - Worse than BetterAuth if you want the largest plugin ecosystem today (they have 18 months on me).
>
> Where it's better:
> - Framework-pluralist (Hono / Bun / Vue / Svelte / Solid all first-class)
> - Self-host = managed parity (same binary; managed is just hosted self-host)
> - B2B org-switching is built-in (Supabase Auth pain point)
>
> GitHub: [link to repo, FIRST]
> Docs: [link to docs]
> Hosted tier (optional): [link to landing]
>
> Honest open question for HN: what's the wedge I'm missing against BetterAuth? Genuinely asking.

**Risk callouts:**

- **HN miss risk:** if Show HN doesn't get traction, primary acquisition for the launch week is dead. Mitigation: pre-warm with named adopters + Twitter + newsletter so launch traffic exists even without HN.
- **lobste.rs ban risk:** lobste.rs is hostile to anything reading as marketing. Mitigation: technical-tone copy + follow norms + don't post unless invited (or get an existing user to post).
- **Reddit ban risk:** r/programming has aggressive self-promo bans. Mitigation: founder must have a comment history (not just a launch post); be useful 30 days pre-launch.
- **BetterAuth counter-launch risk:** BetterAuth could publish a "we already do that" comparison thread within 24hr. Mitigation: be honest about deltas in the launch copy (already drafted above).
- **Single-channel concentration risk:** if HN + Reddit + lobste.rs all miss, the launch falls back to founder's blog/newsletter/Discord (already warm — survivable, not catastrophic).

Output: `launch_playbook.md` with full hour-by-hour and day-by-day detail.

---

# Section 6 — Pricing & packaging

## 6a. Question the pricing BAND before the price point

**Required question per SKILL:** Did $99/mo + $0.001/MAU >10K inherit from competitor anchoring or from ICP willingness-to-pay evidence?

**Verdict:** anchored against Auth0 (much higher) and Supabase Auth (much lower). $99/mo is positioned as "premium-but-cheaper-than-Auth0." But the relevant **paying ICP comparable band** is:

- Clerk Pro: $25/mo + $0.02/MAU
- Kinde: $25/mo bundle
- WorkOS: $125/connection
- Supabase Pro (bundled): $25/mo

**The hosted-auth band at this audience tier is $25-50/mo, not $99/mo.** $99/mo is 4× Clerk's entry price. Two scenarios:

**Scenario A — band is wrong:** founder anchored on Auth0 because Auth0 is the symbol of expensive auth, but the actual paying ICP (Marcus, 4-12 person SaaS) compares against Clerk. At $99/mo, Marcus's first response is "why pay 4× Clerk?" and the answer has to be load-bearing (e.g., "concierge onboarding," "framework-agnostic," "all features unlocked"). If the answer is weak, pricing is wrong.

**Scenario B — band is right, justification needed:** $99/mo IF it includes managed instance + named-account support + all features unlocked + concierge onboarding. Then it positions against "DIY-Keycloak ops cost" (~$2-5K/mo in eng time) rather than against Clerk. This is a higher-trust segment but smaller TAM.

**Recommendation:** founder must choose explicitly which segment they're targeting. Options:

| Option | Price | Positioning | TAM | Founder fit |
|---|---|---|---|---|
| Match Clerk band | $19-29/mo + per-MAU | "OSS-alternative to Clerk, framework-agnostic" | Larger | Better fit for solo founder; SMB self-serve |
| Hold $99/mo with strong concierge | $99/mo + per-MAU + named-account support | "DIY-Keycloak ops escape hatch for 5-20 person teams" | Smaller (but higher LTV/cust) | Requires sustained founder time per customer; doesn't scale past ~50 customers without hiring |
| Two-tier: $29 self-serve + $199 concierge | Both | Capture both segments | Largest | Most complex; risks confusing both segments |

**Founder pushback:** likely says "I want $99 because it signals premium." Counter: per SKILL anti-pattern #7, cheapening for time-poor segment is wrong — but $99 vs $29 is not "cheapening to commodity"; it's matching the market band the paying ICP already evaluates within. If the founder wants $99, the justification must be observable in the product (concierge included, not aspirational).

**Single sharpest recommendation:** start at **$29/mo + $0.001/MAU >10K** with an optional **$199/mo concierge tier** (named-account, founder-led onboarding, monthly check-in). The $29 captures Clerk-graduates; the $199 captures DIY-Keycloak-escapees. Drop the $99/mo middle SKU entirely — it's the worst of both worlds.

## 6b. Standard pricing & packaging coverage

- **Tier structure:** Free OSS (unlimited self-host) / Hosted Starter $29 (50K MAU) / Hosted Pro $199 (concierge, named-account) / Enterprise custom (SSO/SOC2/audit).
- **Trial mechanics:** NO free trial on hosted — instead, 30-day money-back guarantee + free OSS self-host as the trial. Per M0d, free trials select wrong segment (Priya, not Marcus). OSS-as-trial selects the right segment.
- **Annual billing:** 2 months free on annual (≈16% discount). Documented retention boost — RevenueCat data shows annual billing dominates retention for SaaS.
- **Usage metering:** must NOT phone-home from OSS SDK (community-killing). Metering ONLY on hosted-tier API.
- **Per-MAU vs per-seat:** per-MAU is right for auth (Auth0 / Clerk precedent). Don't invent a new model — confuses evaluation.

---

# Section 7 — Post-launch growth loops

| Loop | Type | Compounds? | Notes |
|---|---|---|---|
| **Integration tutorial SEO** | Content | **YES — strongly** | Each tutorial ranks for long-tail queries; compounds over 6-18 months (Stripe precedent) |
| **GitHub stars / contributor recognition** | Social proof | **YES — moderately** | Each named adopter and each star reduces evaluation friction; compounds slowly |
| **Plugin ecosystem (community-built OAuth providers, framework adapters)** | Network effect | **YES — strongly if seeded** | Each plugin makes AuthForge more valuable for the next user — but requires plugin SDK + recognition program first (HashiCorp HUG model) |
| **Discord trust** | Community | **Modest** | Compounds with founder presence; collapses if founder stops showing up |
| **Concierge → testimonial → README adoption** | Word of mouth | Modest | Compounds if founder captures testimonials systematically |
| **Newsletter** | Owned audience | **YES — slowly** | Compounds independent of platform algorithms; resilient channel |
| **Paid ads** | Linear | NO | Every new user requires new spend |
| **Retention-as-acquisition** | WOM | YES if PMF | Marcus tells next-Marcus only if AuthForge is genuinely better than Clerk-for-his-stack |

**Acquisition treadmill risk:** if SEO + plugin ecosystem don't materialize, AuthForge defaults to acquisition treadmill (paid + founder hustle). Section 9 risk #1.

**Compounding loop priority:**
1. SEO / docs — the highest-leverage compounding loop; demands sustained writing cadence
2. Plugin ecosystem — second highest; demands community investment + plugin SDK
3. Newsletter — third; lower ceiling but resilient

---

# Section 8 — Metrics & instrumentation

## Measure (weekly dashboards)

**OSS funnel (ICP-B — Priya):**
- GitHub stars (with weekly delta, source-of-discovery breakdown via referrer where possible)
- GitHub clones (truer signal than stars for engaged users)
- Discord member count + 7-day active count
- npm weekly downloads (delta vs prior week)
- Doc-page views (with top-10 entry pages)
- "Time to first integration" for new users (instrument via opt-in telemetry only if community-acceptable; otherwise from concierge dogfood sample)

**Hosted-tier funnel (ICP-A — Marcus):**
- Hosted landing page views (by UTM-tagged source)
- Trial / signup count (by source)
- Concierge calls booked
- Activated accounts (definition: first auth flow shipped to prod within 14 days)
- 30-day retention
- Conversion rate from concierge-call → paying
- Expansion: hosted accounts crossing 10K MAU (revenue trigger)
- MRR + churn (monthly)
- LTV / CAC (after 3 months of data)

**Channel attribution:**
- UTM-tagged links from every blog tutorial, newsletter, Twitter post
- HN referrer source captured
- Discord-to-signup linkage tracked manually for first 50 accounts

## Don't measure (vanity)

- Total signup count without retention
- HN upvote count (correlation with revenue near-zero)
- Twitter follower growth (doesn't predict paid conversion)
- Stars without clone-to-star ratio (stars alone are vanity)

## Dashboards

- Weekly: `/dashboard/weekly.md` — auto-generated from analytics + GitHub API + Discord API + Stripe API
- Monthly: founder retrospective + adjust plan
- Daily during launch week (-3 to +7): every-hour instrumentation

---

# Section 9 — Risk analysis

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| **Founder reverts to 80%+ building, neglects marketing** | HIGH (this is the default behavior of technical founders) | Catastrophic | Calendar-blocked content time; weekly retro forcing function; accountability partner |
| **BetterAuth out-iterates AuthForge in next 6 months** | HIGH (they have 18-month head start + YC distribution) | High | Sharp wedge BetterAuth cannot replicate (framework-agnostic + B2B-first + 1-binary self-host); refuse to compete on plugin count |
| **Show HN misses (front page no)** | MED (base rate for new-founder dev tools is <30% front page) | Medium (recoverable if other channels warmed) | Pre-warm Twitter + newsletter + Discord; treat HN as ONE of 5 surfaces |
| **Pricing band wrong ($99 too high for paying ICP)** | MED | High (validates wrong segment, mis-tunes product) | Drop $99 SKU; start $29 + $199 concierge tier (Section 6 recommendation) |
| **OSS-tier free-rider dominates, no hosted conversion** | MED | High for business viability | Concierge motion bolted on (Section 5); focus on Marcus-segment signal, not Priya-segment signal |
| **lobste.rs / r/programming ban for self-promo** | LOW-MED | Low (mitigable, but burns the channel) | Founder establishes comment history pre-launch; follow norms |
| **Phone-home telemetry in OSS SDK rejected by community** | LOW | Catastrophic for OSS credibility | Decision now: NO phone-home in OSS. Metering only on hosted tier. |
| **Trust risk — first-time-shipping founder, no carryover GitHub stars** | MED | Medium | Named adopters in README pre-launch (5+ by launch); ex-Stripe credential foregrounded in bio |
| **Calendar gate fires before signals met** | HIGH (founder pressure) | Medium | Pre-commit to soft-launch fallback if signals not met (Section 5a) |
| **Macro: AuthForge category gets absorbed (e.g., Vercel ships Vercel Auth, Cloudflare ships Worker Auth)** | LOW-MED (24-month risk) | Catastrophic | Framework-agnostic positioning hedges platform-specific entrants; partnership posture |
| **Concentration risk: founder's blog as primary surface** | MED | High if Substack/blog platform changes | Own the domain (already does); always cross-post to owned newsletter |

---

# Outside-voice critique

(Run mentally as a Codex-style adversarial pass — what would an independent reviewer say?)

## 1. Single biggest marketing risk the inside review missed

**Sequencing risk inside the docs corpus.** The plan calls for 8 tutorials by day 30. In practice, founders ship 2-3 quality tutorials and then revert to building. The tutorials are also the LEADING INDICATOR of whether the docs-as-marketing motion will work post-launch — if the founder can't sustain 1 tutorial/week pre-launch, they will not sustain it post-launch, and the entire Stripe-precedent compounding loop fails. **Mitigation:** commit to 4 tutorials being LIVE AND RANKING by day 30 as a precondition for proceeding to launch sequence. Not as aspiration.

## 2. Channel mentioned that's weaker than positioned

**Dev-Twitter (3K followers) is positioned as a PRIMARY channel.** Realistically, 3K is small for dev-Twitter. Engagement-per-follower matters far more than count. If founder's recent tweets get <50 likes, the actual reach is <500 viewers per tweet. **Mitigation:** demand engagement data before counting Twitter as primary; if engagement is weak, downgrade Twitter to "supporting" and lean harder on the blog newsletter (which is the actual moat).

## 3. Audience claim that lacks evidence

**"20K monthly readers on tech blog ARE ICP-aligned."** Asserted but not verified. If blog is 60% Rust language internals and 40% Stripe-era distributed systems, only 40% are paying-ICP-relevant. **Mitigation:** founder does one-day audit of last 20 blog posts → categorize → re-rate the audience. If <50% ICP-aligned, the audience asset shrinks to ~8K, which materially changes the Section 4 cadence (more aggressive build needed).

## 4. Provocative reframe the founder might not have considered

**Don't launch a hosted tier in v1.** The OSS SDK + integration corpus alone could be the entire v1. Hosted tier launches in v2 once OSS adoption gives concrete signal about which features paying customers actually need. The hosted-tier-in-v1 plan splits founder attention across two completely different motions (OSS community + SaaS sales) with one founder. **Most successful precedents (Supabase, BetterAuth) shipped OSS-only for 12-24 months before monetizing.** Stripe was an exception (shipped paid first), but Stripe had two co-founders and $2M seed.

This reframe should be surfaced to the founder explicitly. The "right answer" may be: ship OSS v1.0 on day 60, hold hosted tier for day 180 once OSS has 2K+ stars and 50+ named adopters. Founder may push back with "I need revenue" — fair, but the deferred-monetization path has higher LTV/CAC if OSS adoption succeeds.

---

# 3 strongest action items for THIS week

1. **Write the AuthForge-vs-BetterAuth comparison tutorial RIGHT NOW.** This is the highest-leverage piece of content in the entire plan. It will rank for `"authforge vs better-auth"` queries (which Marcus will type), it forces the founder to articulate the wedge honestly, and it serves as the public "answer" for HN-comment objections at launch. Treat as a 2-day deliverable, not week-3.
2. **Drop the $99 SKU. Decide between $29 (Clerk band) or $199 (concierge band) — pick one — by Friday.** The $99 middle SKU is the worst-of-both-worlds. Founder reluctance to drop $99 = anchoring on aspirational positioning vs evidence about the paying ICP.
3. **Pre-commit to the soft-launch fallback in writing.** Founder writes a 1-page "what counts as ready-to-launch" doc, listing the 4-signal gate (5 concierge dependence + 250 stars + 8 ranking tutorials + 5 named adopters). If by day 60 the gate is not met, the launch is a soft OSS-only release with no HN moment. This pre-commitment is the only way to prevent the "calendar-driven HN burn" failure mode.

---

# Appendix — WebSearch URLs invoked

- [Best Supabase Alternatives in 2026 — Cerbos](https://www.cerbos.dev/blog/supabase-alternative-best-open-source-auth-options)
- [Comparing Auth from Supabase, Firebase, Auth.js, Ory, Clerk and others](https://blog.hyperknot.com/p/comparing-auth-providers)
- [Auth Pricing Wars: Cognito vs Auth0 vs Firebase vs Supabase vs Clerk — Zuplo](https://zuplo.com/learning-center/api-authentication-pricing)
- [Clerk vs Auth0 vs Supabase: Pricing & DX Compared](https://designrevision.com/blog/auth-providers-compared)
- [Hanko on GitHub — open source alternative to Auth0/Clerk/WorkOS/Stytch](https://github.com/teamhanko/hanko)
- [WorkOS vs. BetterAuth vs. Clerk — WorkOS blog](https://workos.com/blog/workos-vs-betterauth-vs-clerk)
- [Best Clerk Alternatives for B2B SaaS & AI Applications in 2026](https://www.scalekit.com/blog/clerk-alternatives-for-b2b-ai-apps-in-2026)
- [Better Auth — homepage](https://better-auth.com/)
- [Better Auth on GitHub](https://github.com/better-auth/better-auth)
- [Launch YC: Better Auth — The Authentication Framework for TypeScript](https://www.ycombinator.com/launches/NUm-better-auth-the-authentication-framework-for-typescript)
- [How to launch a dev tool on Hacker News — markepear.dev](https://www.markepear.dev/blog/dev-tool-hacker-news-launch)
- [Show HN: Torii — framework-agnostic authentication library for Rust](https://news.ycombinator.com/item?id=43213090)
- [Show HN: Comprehensive authentication library for TypeScript](https://news.ycombinator.com/item?id=41678652)
- [Hacker News Posting Guide — Syften](https://syften.com/blog/hacker-news-marketing/)
- [Supabase Auth on GitHub (GoTrue fork)](https://github.com/supabase/auth)
- [Why Supabase Became the Go-To Open-Source Alternative to Firebase](https://medium.com/@takafumi.endo/why-supabase-became-the-go-to-open-source-alternative-to-firebase-2d3cd59e7094)
- [Stripe Marketing Playbook — Dru Riley](https://druriley.com/stripe-marketing-playbook-7-strategies-33-examples/)
- [The marketing strategies that got Stripe to $95 billion — Product Marketing Alliance](https://www.productmarketingalliance.com/developer-marketing/the-marketing-strategies-that-got-stripe-to-95-billion/)
- [Stripe Documentation Case Study — Ninad Pathak](https://ninadpathak.com/marketing-research/stripe-documentation-case-study/)
- [Clerk Pricing (2026)](https://clerk.com/pricing)
- [Clerk pricing changelog — Feb 2026 update](https://clerk.com/changelog/2026-02-05-new-plans-more-value)
- [Convert GitHub Stars Into Revenue — Clarm 2025 guide](https://www.clarm.com/blog/articles/convert-github-stars-to-revenue)
- [Open Source Marketing: GitHub Repo to Growth Engine — rzlt.io](https://www.rzlt.io/blog/open-source-marketing-how-to-turn-a-github-repo-into-a-growth-engine)
