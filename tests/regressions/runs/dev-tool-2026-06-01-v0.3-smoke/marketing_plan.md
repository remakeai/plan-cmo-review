# Marketing Plan — AuthForge

**Skill:** plan-cmo-review v0.3.0 (smoke test)
**Fixture:** dev-tool synthetic — AuthForge open-source authentication / identity SDK with hosted tier
**Date:** 2026-06-01
**Mode:** **Mode A — Full Marketing Review** (with Section 4 elevated)

---

## Operating-default note

Default founder posture: technically strong, marketing-naive. Evidence override check (per skill):
- Prior shipped products with >$10K MRR: **NO** ("no prior shipped products")
- Documented marketing track record: **PARTIAL** — popular technical blog ~20K monthly readers, 3K dev-Twitter followers
- Existing audience surface large AND ICP-aligned: **YES** — 20K monthly dev blog readers IS the ICP class (backend engineers) for AuthForge
- Documented prior failed launches with retro: **NO**

**Verdict:** founder is partially audience-credentialed for THIS specific product (dev-tool, dev audience). The 20K blog readership in the right category flips two of four override criteria. Premise-challenge is still load-bearing on the *plan*, but the founder is not naive on the *audience* axis. This is exactly the Mode A profile, NOT Mode C. Treating this founder as "no audience" would be misreading the input.

---

## PREMISE-LEVEL FINDINGS BLOCK

(Surfaced at top per skill rule when ≥2 of M0a–M0e fail.)

**Three premises failed challenge:**

1. **M0d — "GitHub stargazers will upgrade to hosted tier" is acquisition selection-bias.** Stargazers select for "this looks interesting, saving for later" and almost never overlap with "I will pay $99/mo for managed instance" in the same person. Sentry data: 90% of users stay on the free self-hosted plan indefinitely; conversion to cloud happens at the *organization-scaling* moment, not the *star* moment. The current plan confuses repo popularity with revenue intent.
2. **M0e — Dogfood-vs-paying-ICP mismatch.** The product is being built by an ex-Stripe engineer (will dogfood on solo/indie use cases — auth for one app, one team). The $99/mo + $0.001/MAU pricing structure targets companies past 10K MAU — small/mid teams running production traffic, not solo builders. Without buyer-aligned dogfood, AuthForge will ship feature-tuned for the wrong end of the market.
3. **M0b — "Simpler than Auth0, more flexible than Supabase Auth, OSS unlike both" is positioning by negation against the wrong frame.** Supabase Auth IS effectively open-source (MIT-licensed within the Supabase repo). The differentiation collapses on inspection. The canonical-success comparables (Sentry, Supabase, PostHog, SuperTokens) all have richer positioning than "alternative to X, Y."

**One premise survived strongly:**

- **M0a — HN IS the right audience class.** Dev-tool launches on HN are not the category-error pattern that catches consumer products. The dev-tool motion-class block applies; Show HN should be a primary surface (not the entire plan).

**One premise survived with caveats:**

- **M0c — Anti-feature scan** found one candidate (hosted tier is a managed-instance model that pulls in DevOps overhead and conflicts with the "drop-in SDK" simplicity story). Worth flagging; not a kill.

These three failed premises cascade into the Section 1 / Section 3 / Section 6 work below.

---

## Step 0 — Pre-review system audit

### Read what exists
Design doc (the founder's brief, frozen synthetic input). No prior planning artifacts. No landing page yet. No README beyond a placeholder.

### Competitive landscape web search
Five competitor / canonical-success searches run live (URLs in run summary). Key findings:
- Clerk: free 50K MRU (raised from 10K in Feb 2026), $0.02/MAU thereafter, Pro $25/mo. Pre-built UI is the moat.
- Auth0 (Okta-owned): $0.07/MAU, Essentials $35/mo, "enterprise mature" positioning, free 25K MAU.
- Supabase Auth: free 50K MAU, $0.00325/MAU after — cheapest at scale by ~10x. Default for Supabase-stack teams.
- WorkOS: 1M MAU free on AuthKit; B2B-SSO-first positioning.
- Stytch: 10K MAU free; passwordless-led.
- Open-source self-hosted incumbents: Keycloak (Apache 2.0, most feature-complete), SuperTokens (Apache 2.0, lightweight, closest to AuthForge's stated position), Authentik, Ory, ZITADEL, Hanko, Stack Auth, FusionAuth Community.

**The OSS+hosted lane AuthForge wants to occupy is already crowded.** SuperTokens in particular is the direct positional twin: open source, self-hosted or cloud, designed as a Supabase-alternative for teams that don't want Postgres lock-in. AuthForge's positioning statement does not name SuperTokens. That's a blind spot.

### Founder audience audit
- Twitter/X: 3K followers, dev-aligned. **Modest but real.**
- Technical blog: ~20K monthly readers. **Substantial and ICP-aligned (backend eng audience).**
- Prior OSS reputation: none specified.
- Prior shipped products: none.
- Ex-Stripe engineer affiliation: signal of credibility within the dev-tool community (Stripe is the canonical DX brand per /Section 3 dev-tool block).

**Total ICP-aligned attention surface: ~23K monthly + Stripe-alum credibility.** This is genuinely strong for a dev-tool launch. It is the load-bearing distribution asset for this plan and Section 3 will rank it #1.

### Mode determination
- Founder has ≥1K ICP-aligned attention surface ✓
- Competitive context exists ✓
- Product is mid-build, launch contemplated

→ **Mode A — Full Marketing Review.** Not Mode C: the 20K blog disqualifies "zero audience" framing.

---

## Step 0.5 — Premise audit

### Premise extraction

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| 1 | Launch = Show HN + r/programming + integration tutorials | "Distribution Plan" | Single-burst plan with no compounding surface; tutorials are PRIMARY not auxiliary for dev tools |
| 2 | Audience = "backend engineers building auth into their apps" | "Target users" | Too broad — solo vs team vs platform-engineer have different buying behavior |
| 3 | Pricing = $99/mo + $0.001/MAU above 10K | "Distribution model" | Anchored on Clerk ($25/mo + $0.02/MAU). $0.001/MAU is 20x cheaper — signals commodity to enterprise buyers; $99/mo is high for solo devs but low for teams |
| 4 | First 10 customers = GitHub stargazers → hosted tier | "First 10 customers" | Stargazers ≠ buyers (Sentry: 90% stay self-hosted indefinitely) |
| 5 | Validation = 100 stars + 5 hosted signups by day 60 | "Validation gate" | Stars is vanity; 5 signups is too thin to validate either feature direction or pricing |
| 6 | Differentiation = simpler than Auth0, more flexible than Supabase, OSS unlike both | "Differentiation" | Supabase Auth IS effectively open-source; SuperTokens unnamed but occupies this exact position already |

### M0a — Launch-platform audience-class fit
**Premise:** Show HN is the launch platform.
**Web search check:** Show HN launches for auth/identity SDKs — successful dev-tool HN launches exist (Stytch, Clerk both used dev-comm channels). Multiple "How to launch a dev tool on HN" posts confirm HN is the right audience class for backend infra.
**Verdict:** **PREMISE SURVIVES (PASS).** HN is correct audience class for dev-tool/OSS launches. The dev-tool motion-class block (Section 3) applies. Do NOT downgrade HN here — that was the consumer-product pattern. The problem with the plan is not that HN is wrong; it's that HN is the *only* compounding surface named.
**Cascading implication:** Section 5 keeps HN as primary launch; Section 3 ranks HN alongside docs/SEO + GitHub + founder blog (NOT instead of them).

### M0b — Canonical-success comparable
**Premise:** "Simpler than Auth0, more flexible than Supabase, OSS unlike both" — implies the precedent set is competitive negation.
**Web search check:** Canonical OSS+hosted successes in dev infra:
- **Sentry** — open-source error tracking, FSL license, 90% of users self-host free; cloud conversion happens at organizational-scaling moments, not signup. Sentry's marketing playbook: docs-as-marketing, framework integrations as long-tail SEO, dev-conference presence.
- **Supabase** — explicit "open-source Firebase alternative," uses PostHog for product analytics, partnered with AI builder tools as soon as that traffic source appeared.
- **PostHog** — usage-based with generous free tier (1M events, 5K replays, 100K errors), open-source, content-engine driven.
- **HashiCorp** — contributor recognition (HUG program), enterprise upsell, multi-product ecosystem.
- **SuperTokens** — direct positional twin; needs to be named honestly.
**Specific delta** vs current plan:
- Sentry/Supabase/PostHog all treat **docs as marketing** with framework-by-framework integration tutorials. Current plan treats tutorials as a side channel.
- All have first-party SDK adapters across frameworks. Current plan does not specify SDK fan-out.
- All have a content engine (blog, newsletter) running continuously. Current plan has launch-burst posture only.
- All publish honest comparison content ("PostHog vs Sentry", "Supabase vs Firebase"). Current plan defines itself by negation only.
**Verdict:** **PREMISE FAILS.** Direct-competitor negation is not a strategy. Anchor on Sentry's playbook (the closest fit for OSS+hosted in dev infra).
**Cascading implication:** Section 1 will produce both tables; Section 3 will pull docs/SEO and GitHub-as-marketing to PRIMARY rank; Section 5 will include framework-tutorial cadence as a permanent surface, not a launch task.

### M0c — Anti-feature surface
**Premise:** All in-scope features serve the paying ICP.
**Line-by-line check:**
- Open-source MIT SDK — serves both free and paid; OK.
- Hosted tier at $99/mo — serves paying ICP; OK.
- $0.001/MAU above 10K — serves usage-scaling teams; OK BUT see M0b on pricing band signaling.
- "Managed instance" framing — this is a single-tenant DevOps-flavored deliverable. Conflicts with the "simpler than Auth0" simplicity story. Most dev-tool buyers at $99/mo expect multi-tenant SaaS, not "your own instance to manage" (even if managed).
**Verdict:** **PREMISE FAILS (mildly).** One candidate anti-feature: the "managed instance" framing should be revisited. Either become true multi-tenant SaaS at this price point, or rebrand the hosted tier as a higher-touch self-hosted-with-support offering.
**Cascading implication:** Section 6 must address what "hosted tier" actually means; Section 2 ICP doc must specify whether the buyer wants managed-single-tenant or simple-SaaS.

### M0d — Freebie-disqualifier (acquisition selection bias)
**Premise:** "First 10 customers = GitHub stargazers who upgrade to hosted tier."
**Mechanic mapping:**
- GitHub star → low-commitment, "save for later" gesture. Selects for "interested developer, no buying intent yet."
- OSS SDK install → moderate commitment. Selects for "actively using." Still mostly free-tier-forever.
- Hosted tier signup at $99/mo → trust-led, often org-driven, requires either a) self-host pain that crosses an annoying threshold, or b) a team/company decision to outsource the operational burden.
**Web search evidence:** Sentry — 90% of users self-host on free plan indefinitely. Conversion to paid cloud happens at *scaling* moments (infra complexity exceeds tolerance), NOT at *star* moments. GitHub stars correlate with awareness, not revenue.
**Verdict:** **PREMISE FAILS.** Stargazer-to-hosted-tier is not a real acquisition mechanism — it's a category confusion. Stars are top-of-funnel awareness; hosted-tier buyers come from operational pain at scale.
**Cascading implication:** M6 (first 10 paying customers) needs a real mechanism. Likely: (a) direct outreach to teams already on Auth0/Clerk who hit pricing pain at scale, (b) founder's own dev-blog readers who run production-scale apps, (c) concierge onboarding of first 10 with founder personally migrating their auth.

### M0e — Dogfood audience-class match (founder vs paying ICP)
**Premise:** Founder dogfoods → product is calibrated for paying ICP.
**Check:** Ex-Stripe engineer building auth SDK. Likely dogfood targets:
- Founder's own side projects (solo developer, small scale).
- Maybe a friend's startup or two (small team, pre-product-market-fit).
Paying ICP for $99/mo + per-MAU pricing:
- Teams running production apps past 10K MAU.
- Companies feeling Auth0's $0.07/MAU pricing pain at scale.
- Engineering teams making a build-vs-buy auth decision with budget authority.
**Mismatch is real.** Dogfooding on solo side projects tunes the SDK for "easy to integrate in 10 minutes" — which is great — but says nothing about the operational requirements of teams running auth in production (SSO, SCIM, audit logs, multi-tenant org models, compliance hooks). The product will ship missing the things its paying ICP needs to buy.
**v0.3 prescription check:** The wrong fix is "defer the paying ICP and target solo devs first." That preserves the mismatch and ships AuthForge as a free toy for individuals — the exact failure mode that kills OSS+hosted businesses. The correct fix is BOTH pivots:
1. **Pivot target audience** in marketing copy, ICP doc, and launch sequencing toward small/mid teams running production auth (not solo devs saving stars).
2. **Expand dogfood subjects** before launch — recruit 2-3 small-team paying-ICP-representative testers (could be alumni of Stripe, Y Combinator founder network, or existing blog-reader cohort) and run buyer-aligned dogfood for 1-2 weeks minimum.
**Verdict:** **PREMISE FAILS — but with explicit prescription that BOTH pivots happen.** Do NOT take the "defer paying ICP" off-ramp.
**Cascading implication:** Section 2 ICP doc names a small-team ICP, not solo-dev; Section 4 audience-build commits time to recruiting buyer-aligned dogfooders; Section 5 sequencing front-loads outreach to teams not stars.

---

## Step 0A — Forcing questions (M1–M7)

### M1 — Audience reality
**Naive founder answer:** "Backend engineers who don't want to use Auth0."
**Skill challenge:** Not specific enough. Name a real persona.
**Sharpened answer:** *Maya Chen, staff engineer at a 25-person seed-stage YC SaaS, currently on Auth0 paying ~$400/mo, about to hit the next tier and looking at $1500/mo+. Reads The Pragmatic Engineer, Lenny's Newsletter (occasionally), follows the Supabase team on Twitter, hangs out in r/ExperiencedDevs and the Cerbos/Authentik Slack. Has read the founder's Stripe-era blog posts. Has 30 minutes a week to evaluate alternatives.*
**Concrete attention surfaces:** Pragmatic Engineer newsletter, dev-Twitter (Supabase / Vercel / planetscale orbits), HN front page, r/ExperiencedDevs, Cerbos & SuperTokens GitHub issue trackers.

### M2 — Discovery path
**Naive answer:** "Show HN post."
**Skill challenge:** Show HN cannot be step 1 — it's at best a discoverability moment, not a discovery path. The skill specifically refuses "Show HN" as step 1.
**Sharpened 3-step path:**
1. Maya hits Auth0's next pricing tier and types "Auth0 alternatives 2026" into Google → lands on a *framework-specific integration tutorial* from AuthForge ranking for "Next.js auth alternative to Auth0" (long-tail SEO).
2. She clicks through to the GitHub repo (NOT the landing page first — engineer instinct), scans the README, checks star count, contributor count, and the last 30 days of commits.
3. She tries the SDK in 10 minutes in a sandbox, then either (a) Slacks her team about it, or (b) DMs the founder (who is known from blog).

**Time-to-discovery:** weeks, not "eventually." Realistic given framework-tutorial SEO ranking + founder's existing dev-blog reach.

### M3 — Pre-launch audience (specific numbers)
- Twitter/X: 3,000 followers (dev-aligned)
- Technical blog: ~20,000 monthly readers (backend engineering audience, exactly ICP-class)
- Newsletter: not mentioned — **assume zero**, flag as gap.
- Stripe alum network: ~unquantified but real (Slack groups, founder network)
- GitHub: no prior reputation specified — starting from zero stars on the AuthForge repo.

**Total ICP-aligned attention: ~23K + Stripe-network credibility.** Substantial. This is a Mode A profile, not Mode C.

### M4 — Channel honesty (one credible advantage)
**Named channel:** the founder's existing technical blog (20K monthly readers in the right ICP class). This is the demonstrable advantage over a generic founder. NOT Twitter (3K is modest); NOT GitHub (zero history yet). The blog is the one channel where the founder has a real edge.
**Secondary advantage:** Stripe alum brand-borrowing (credibility transfer, not distribution per se).

### M5 — Competitor traffic source
**Naive answer:** "I don't know."
**Skill: assignment + research:**
- Clerk: heavy investment in docs (clerk.com/docs), framework-specific integration content, dev-Twitter presence, conference sponsorships. Some paid (Google ads on "auth0 alternative"). Strong contributor recognition.
- Auth0: SEO dominance on "[framework] authentication" + Okta enterprise sales funnel + broad partner ecosystem.
- Supabase Auth: rides Supabase parent brand; PostHog-tracked AI-builder-tool referrals are a meaningful new channel.
- SuperTokens: docs-as-marketing, framework-integration SEO, active GitHub presence, dev-conference talks, content blog.
- Stytch: developer-marketing-heavy, content engine on passwordless/passkey trends.
**Pattern:** docs/SEO + GitHub + content engine dominates this category. Paid social barely exists in this space.

### M6 — First 10 paying customers (named path)
**Naive answer:** "GitHub stargazers."
**Skill challenge:** M0d killed this premise. Need real names + real outreach.
**Sharpened plan:**
1. Email 5 of the founder's blog readers known to run production-scale apps. Offer concierge migration from their current auth provider.
2. DM 5 named YC W25/S25 founder-network contacts whose stacks include Auth0 or Clerk.
3. Post in the Y Combinator alumni Slack (#dev-tools channel) with an honest "I'm working on X, want 5 design partners" message.
4. Reach out to 3 Stripe alumni now at small startups likely paying for auth.

**Total identified outreach surface: 15-20 named potential conversations.** Not all will convert. Aim for 5 paying design partners by day 60 (NOT 5 stargazer self-signups — different mechanism).

### M7 — Time allocation
**Naive answer:** "Most of my time on building."
**Skill challenge:** ≥30% should be audience-building pre-launch.
**Realistic target:** 70% build / 30% audience for the next 4-6 weeks. The 30% means: ship 1 technical blog post per week, ship 1 integration tutorial per week, do 1 podcast or community appearance every 2 weeks, and run weekly outreach to potential design partners. Numbered weekly cadence in Section 4.

---

## Step 0B — Mode selection

**Locked: Mode A — Full Marketing Review with Section 4 elevated.**

Rationale:
- Founder has ≥1K ICP-aligned attention surface (23K) ✓
- Competitive context now established ✓
- Mid-build with implied launch window (validation gate at day 60) ✓
- NOT Mode C — the 20K blog disqualifies "zero audience" framing per v0.3 activation tightening.

Section 4 elevated because:
- GitHub repo is at zero stars/contributors today; needs pre-launch warm-up cadence
- No newsletter exists; opportunity to build one before launch
- Recruiting buyer-aligned dogfooders (per M0e) is itself an audience-build activity

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Name | Pricing | Acquisition channels (verified) | User complaints | Position vs AuthForge | Winning? |
|---|---|---|---|---|---|
| Clerk | $25/mo + $0.02/MAU; free 50K MRU | Docs-as-marketing, framework SEO, dev-Twitter, conference sponsorships | Pricing surprises at scale, vendor lock-in | Premium DX + UI components; AuthForge can't compete on UI polish v1 | Yes — strong growth |
| Auth0 (Okta) | $0.07/MAU; Essentials $35/mo; free 25K | SEO dominance, enterprise sales, partner ecosystem | Expensive at scale, "enterprise tax" pain | The Goliath AuthForge is hunting; pricing pain is real | Yes (in revenue), losing on dev sentiment |
| Supabase Auth | Free 50K MAU; $0.00325/MAU after | Rides Supabase brand; AI-builder-tool partnerships (PostHog data) | Tied to Postgres; not standalone | Effectively OSS already — refutes AuthForge's "OSS unlike both" claim | Yes — default for Supabase-stack teams |
| SuperTokens | Free OSS self-host; managed cloud paid | Docs/SEO, GitHub, dev-content blog, conference talks | Self-host complexity for newcomers | **Direct positional twin to AuthForge.** OSS, Apache 2.0, lightweight alternative to Auth0/Supabase Auth | Yes — small but real traction |
| WorkOS | 1M MAU free on AuthKit; B2B-SSO-priced upmarket | B2B sales-led + dev-content | Aimed enterprise, less indie-friendly | Different lane — B2B-SSO-first | Yes, in B2B SSO |
| Stytch | 10K MAU free; passwordless-tier | Dev-marketing on passkeys, content engine | Passwordless-narrow positioning | Tangent — auth-method rather than auth-platform | Mid traction |

**Honest read:** SuperTokens is the closest match in positioning AND it's already shipped, has GitHub stars, and is in the conversation. AuthForge's "OSS unlike both [Auth0, Supabase]" line is incorrect AND ignores its true twin. This must be fixed in positioning.

### 1b. Canonical-success comparables (the part most plans skip)

| Name | Price | Founded | Scale | Primary channel (verified) | Onboarding | Launch gate | Delta vs AuthForge plan |
|---|---|---|---|---|---|---|---|
| Sentry | $26-$80/mo+ usage | 2008 | $100M+ ARR | Docs-as-marketing, framework SDK fan-out, 90% self-host conversion to cloud at scale moment | Self-serve SDK install | Continuous; no calendar gate | AuthForge plan has NO SDK fan-out cadence, NO "scale moment" conversion thesis |
| Supabase | Free + $25/mo Pro + usage | 2020 | $1B+ valuation | "Open-source Firebase alternative" positioning; AI-builder partnerships (Bolt, v0, Cursor); content engine | Self-serve | Continuous; community-driven | AuthForge has NO equivalent partnership thesis, NO content engine |
| PostHog | Usage-based; generous free | 2020 | Profitable, $10M+ ARR | Content engine (~1 post/day), honest comparison content ("PostHog vs Sentry"), customer case studies | Self-serve | Continuous | AuthForge has NO content-cadence, NO honest-comparison content |
| HashiCorp | OSS+Enterprise | 2012 | $5B+ (Vault/Terraform) | HashiCorp User Groups (HUG), contributor recognition, conference (HashiConf), docs | Self-serve OSS, sales-led enterprise | Continuous | AuthForge has no contributor program, no community-event surface |

**Specific delta from canonical successes:**
- **All four treat docs as primary marketing, not auxiliary documentation.** AuthForge plan lists "integration tutorials" as a launch-day tactic, not a continuous compounding surface.
- **All four publish honest comparison content** including where they lose. AuthForge plan defines itself by negation only.
- **All four have a continuous content cadence** (Sentry: framework SDK posts; PostHog: ~daily blog; Supabase: weekly product+ecosystem; HashiCorp: conference + docs). AuthForge plan has launch-burst only.
- **All four have either contributor recognition (HashiCorp HUG-style) or named-adopter visibility (Sentry's customer list, Supabase's ecosystem partner badges).** AuthForge has none planned.
- **All four converted to paid at scaling moments**, not at signup moments. AuthForge's "stargazers → hosted tier" thesis contradicts this.

### 1c. Pattern surface

Canonical successes in OSS+hosted dev-infra share four habits AuthForge lacks: docs-as-primary-marketing, honest comparison content, continuous content cadence, and ecosystem/contributor visibility. Direct competitors (Clerk, Auth0) win on different terrain — Clerk on UI polish + DX, Auth0 on enterprise sales — neither of which AuthForge can match in v1. The right anchor is the Sentry/Supabase/PostHog playbook (docs + framework fan-out + scaling-moment conversion), NOT the Clerk/Auth0 playbook.

**Implicit pattern AuthForge plan is following:** classic "Show HN single-shot launch + hope stars convert" playbook — the documented OSS-monetization failure mode. Reanchor to Sentry's playbook.

**Founder action:** read three pieces:
1. Sentry blog "How Sentry thrives as an open source software company"
2. PostHog "Supabase customer case study" (acquisition source data)
3. SuperTokens GitHub README + most-recent 5 framework-integration tutorials (the direct positional twin's actual current marketing surface)

---

## Section 2 — ICP specification

**See `icp.md`** (separate artifact).

Headline: small/mid team (5-50 engineers) running production-scale auth, currently on Auth0/Clerk feeling pricing pain or Supabase Auth feeling Postgres-coupling pain. NOT solo developers. NOT stargazers.

---

## Section 3 — Distribution channel-by-channel (with dev-tool motion-class block APPLIED)

### Generic channel scoring (filtered for dev-tool fit)

| Channel | Reach (1-5) | Cost (1-5, low=cheap) | Conv (1-5) | Founder fit | Effort | Verdict for AuthForge |
|---|---|---|---|---|---|---|
| Show HN | 4 (if hit) | 1 | 3 | 4 (Stripe alum credibility) | 2 (one-day burst) | KEEP — single-shot, plan accordingly |
| Twitter/X organic | 3 | 1 | 2 | 3 (3K followers modest) | 4 (continuous) | KEEP but secondary |
| r/programming, r/ExperiencedDevs, r/devops | 3 | 1 | 3 | 3 | 2 | KEEP — single-shot per sub, mind rules |
| lobste.rs | 2 | 1 | 4 (high-signal audience) | 2 (need invite) | 1 | KEEP — request invite or guest post |
| IndieHackers | 2 | 1 | 2 | 2 (wrong end of audience) | 2 | SKIP — solo-dev audience, not paying ICP |
| Substack/newsletter | 4 (compounds) | 1 | 4 | 5 (blog already established) | 4 | KEEP — start newsletter from existing blog list |
| LinkedIn organic | 2 (for dev tools) | 1 | 2 | 2 | 3 | DEPRIORITIZE |
| Paid ads | 2 | 5 | 2 | 1 | 3 | SKIP — dev tools rarely convert on paid social |
| Cold outreach (M6 named list) | 3 | 1 | 5 | 4 | 4 | KEEP — load-bearing for first 10 paying |
| Podcast guesting | 3 | 1 | 4 | 4 (Stripe alum + blog story) | 3 | KEEP — quarterly cadence |

### **DEV-TOOL MOTION-CLASS BLOCK (v0.3 LOAD-BEARING)**

Per v0.3 Section 3 dev-tool rules, three surfaces are **PRIMARY** (not auxiliary) for AuthForge. Ranking these correctly is the difference between a real plan and a Show-HN-lottery plan.

#### PRIMARY Channel #1 — Founder's existing technical blog + newsletter
- **Why PRIMARY:** 20K monthly readers in exactly the ICP class. Trust transfers within developer community in ways it does not in consumer or B2B-non-dev (v0.3 rule). This is the founder's single biggest distribution lever.
- **Action:** convert blog into the AuthForge home for technical narrative. Start a newsletter (Substack or Beehiiv) and migrate blog readers — target 5K subs by day 90. Publish AuthForge build-in-public + architecture-decision posts as the cadence.
- **Why ranked #1:** the founder's existing audience is the asset competitors can't replicate. Sentry, Supabase, PostHog, Clerk all started with founder-built audiences in dev media.

#### PRIMARY Channel #2 — Docs / SEO compounding (framework-by-framework)
- **Why PRIMARY:** Stripe is the canonical playbook (per v0.3 rule). Sentry, Supabase, PostHog, SuperTokens, Clerk ALL win on "[Framework] auth tutorial" long-tail SEO. This compounds over months; first-mover advantage on a framework integration ranks for years.
- **Action:** ship one framework integration tutorial per week starting 4 weeks before launch. Prioritized framework list (highest dev-search-volume + likely paying-team usage):
  1. Next.js (huge volume, paying-team adoption)
  2. Remix
  3. SvelteKit
  4. Fastify (Node backend)
  5. Hono
  6. Rails (long-tail, less competition)
  7. Django (long-tail, less competition)
  8. Phoenix/Elixir (niche but loyal)
- **Each tutorial:** working code repo, deploy-able example, "AuthForge vs [alternative]" honest comparison table at the bottom. Treat as marketing assets with permalink + ongoing SEO maintenance.
- **Why ranked #2:** ramps slowly but compounds infinitely. Behind the blog because the blog already exists; tutorials need 4-6 weeks of work to start landing.

#### PRIMARY Channel #3 — GitHub as marketing surface
- **Why PRIMARY:** per v0.3 rule, GitHub repo health (stars, watchers, contributors, issues hygiene, named adopters in dependency graphs) IS social proof for evaluators. Stars >5K materially affects evaluator conversion. Ecosystem-of-integrations is its own marketing motion.
- **Specific actions:**
  - **Contributor recognition program (HashiCorp HUG-style):** named "AuthForge Adopters" + "AuthForge Contributors" page in the README. Public credit by name. Email outreach to first 10 contributors thanking them publicly. This is verbatim from HashiCorp's playbook.
  - **First-party SDK adapters** as separate sub-repos under the org (next-authforge, remix-authforge, etc.). Each is its own GitHub asset with its own star count and discoverability.
  - **Issues hygiene:** every issue gets a response within 24h pre-launch; reply within 4h on launch day. This is visible to evaluators reading the repo.
  - **Named visible adopters:** as design-partner companies onboard, get permission to list them as adopters (logo wall in README). Even 3-5 named adopters change evaluator perception.
- **Why ranked #3:** zero today, needs build-up; but compounds powerfully once seeded.

#### Named integration partners proposed (per v0.3 rule)
- **Framework adapters:** Next.js team (Vercel-adjacent), Remix team (Shopify), SvelteKit (Vercel), Fastify, Hono, Rails (37signals adjacent), Django (DSF).
- **Ecosystem partners worth approaching:** Vercel (integration in their marketplace), Railway, Render, Fly.io (one-click deploy templates), Cerbos (authZ pairing, complementary not competing), trigger.dev, Inngest (job-running integrations needing auth).
- **AI builder tools (Supabase precedent):** Bolt, v0, Cursor, Lovable — get AuthForge into their default auth-pick lists for generated apps. Supabase's AI-builder partnership was its biggest acquisition surprise per PostHog case study; AuthForge can chase the same surface.

### Anti-marketing tonal rule for this section
Per v0.3 dev-tool tonal rule: AuthForge marketing materials in all three primary channels must REFUSE superlatives ("revolutionary", "best-in-class", "enterprise-grade", "seamless", "robust", "game-changing", "world-class") and REQUIRE technical specifics, honest comparisons including where AuthForge loses. See Section 5 for the launch-copy application.

### Surviving channel ranking (post-filter)

1. **Founder blog + newsletter (PRIMARY)** — highest leverage given existing audience
2. **Docs/SEO framework tutorials (PRIMARY)** — highest long-term compounding
3. **GitHub repo health + contributor program (PRIMARY)** — second-highest compounding
4. **Cold outreach to named M6 list** — load-bearing for first 10 paying
5. **Show HN launch event** — single-shot, plan for amplification not validation
6. **Podcast guesting** — quarterly, leveraging Stripe-alum + blog story
7. **r/programming, r/ExperiencedDevs, lobste.rs** — single-shot per community, follow rules
8. **Twitter/X build-in-public thread cadence** — augments blog, doesn't replace

**SKIPPED:** paid ads, LinkedIn, IndieHackers (wrong audience), Product Hunt (auxiliary at best for dev tools — keep light).

---

## Section 4 — Pre-launch audience-build plan (ELEVATED)

### Day 1-30 cadence
- **Weekly:** 1 long-form technical blog post on the existing blog (architecture decisions, OSS economics commentary, auth-system pitfalls). Audience: 20K existing readers.
- **Weekly:** 1 framework integration tutorial draft (first 4: Next.js, Remix, SvelteKit, Fastify). Publish to docs as it ships.
- **Weekly:** 1 Twitter/X thread linking to the blog post or tutorial (≥3K followers, slowly grow via discoverability).
- **Bi-weekly:** 1 podcast pitch + 1 dev-community guest appearance (Pragmatic Engineer podcast circle, Software Engineering Daily, Changelog).
- **Continuous:** newsletter setup migrated from blog list — aim 1K subs week 1, 3K by week 4.
- **Continuous:** recruit 3-5 buyer-aligned dogfood design partners per M0e (NOT solo devs; small teams running auth in production). Direct outreach via Stripe network + blog reader email replies.

### Day 31-60 cadence
- Scale tutorials to 2/week (5 more frameworks)
- Add weekly GitHub repo activity report (visible commit + issue cadence — repo health signal)
- Begin teasing AuthForge specifically in blog posts (build-in-public). Target newsletter to 5K.
- Run private alpha with design partners. Run Vohra "very disappointed" survey on alpha cohort.

### Day 61-90 cadence
- Public beta announcement on blog + newsletter (NOT public launch yet)
- Begin podcast appearances as confirmed (target 2 in this window)
- Set up the launch sequence per Section 5
- Verify launch gate: PMF signal (per Section 5a) — only proceed if ≥40% of alpha cohort says "very disappointed without"

---

## Section 5 — Launch playbook

### 5a. Launch gate question

**Question:** Calendar (day N) or PMF signal?

**For AuthForge specifically:** dev-tool launches CAN benefit from calendar-driven launch moments (Show HN is a time-bounded marketing event; Product Hunt similar) — this is the carve-out the skill explicitly notes for dev tools. BUT the validation gate should still be PMF-signal-driven, because retention is what drives OSS-to-paid conversion (Sentry's "scaling moment" thesis).

**Recommended gate:**
- **Validation:** PMF-signal — ≥40% of alpha-cohort design partners say "very disappointed" to losing AuthForge. Vohra test.
- **Public launch:** calendar within 2 weeks of validation gate passing, to capture HN/PH momentum. Do NOT calendar-launch without validation.
- **Refuses the founder's original validation gate ("100 stars + 5 signups by day 60")** — stars are vanity, 5 signups is too thin for either signal. Replace with: 3 paying design partners + Vohra survey + 5K newsletter subs by day 60.

### 5b. Sequenced launch (post-validation)

| Day | Channel | Specific action |
|---|---|---|
| -30 | Audience-build | Section 4 cadence in flight |
| -14 | Newsletter | Build-in-public deep-dive on AuthForge architecture (preview to existing readers) |
| -7 | Personal network email | Pre-announce to ~50 named contacts (Stripe alumni + design partners + named YC founders) |
| -3 | Twitter | Build-in-public thread previewing technical decisions, linking GitHub repo (NOT landing page) |
| -1 | Blog post | Detailed "Why we built AuthForge" post on existing blog — honest comparison including where we lose to Clerk and Auth0 |
| 0 morning | Hacker News | Show HN. Title: "Show HN: AuthForge – open-source auth SDK with optional managed instance" (NO superlatives). Body: technical specifics, links to GitHub FIRST, then docs, then landing page. Comments: founder responds technically to every comment within 1h. |
| 0 + 2h | Twitter | Thread amplifying HN, with technical excerpts (not "we launched!" copy) |
| 0 + 4h | r/programming | Honest "I shipped this" post linking to GitHub. NOT "introducing the revolutionary new..." copy. |
| 0 + 6h | lobste.rs | Submit (if invite); technical framing |
| 0 + 24h | r/ExperiencedDevs | Post about engineering trade-offs in building AuthForge — discussion-first, not promotion-first |
| 0 + 48h | LinkedIn (founder's network) | Brief professional note + link |
| 0 + 7d | Product Hunt | Separate event, but auxiliary; don't sweat the rank |
| 0 + 14d | Podcast outreach | Pitch 5 dev-podcasts with the build-in-public story |
| 0 + 30d | Newsletter retro | Honest traction report — what worked, what didn't, what's next |

### 5c. Launch-copy tonal rule (v0.3 LOAD-BEARING)

**REFUSE these phrasings in launch copy** (per Section 3 dev-tool tonal rule + anti-pattern #13):
- "Revolutionary auth platform"
- "Best-in-class developer experience"
- "Enterprise-grade security"
- "Game-changing approach to identity"
- "Seamless integration"
- "Robust authentication system"
- "World-class auth"
- "Reimagined identity for the AI era" (also avoid trend-piggybacking superlatives)

**REQUIRE these patterns:**
- **Lead with technical specifics:** "AuthForge — JWT + session-based hybrid, MIT-licensed SDK, ~50KB bundle, with an optional managed-instance tier"
- **Honest comparison table including AuthForge losses:**

  | | AuthForge | Clerk | Auth0 | Supabase Auth | SuperTokens |
  |---|---|---|---|---|---|
  | Pricing at 100K MAU | $99 + $90 | $1,800+ | $7,000+ | $325 | self-host: $0 + ops |
  | Pre-built UI components | Limited v1 | **Best** | Good | OK | OK |
  | Enterprise SSO/SAML | Roadmap, not v1 | Yes | **Best** | Limited | Yes |
  | Standalone (not tied to DB) | Yes | Yes | Yes | Coupled to Supabase | Yes |
  | Maturity | New | Mature | **Most mature** | Mature | Mature |

  Saying "Clerk has the best UI" and "Auth0 is more mature" in our own launch copy is what makes the developer audience trust the wins we DO claim.

- **Code-first links:** GitHub repo before landing page in HN/Reddit. Show, don't tell.
- **"Engineer wrote this for engineers" register:** the post should read like the founder's blog, not like marketing material.

**Anti-pattern #13 explicitly invoked here.** The instinct under launch pressure is to write copy that "sells." The dev audience reads selling as adversarial. This rule is the single highest-value protection v0.3 added for this fixture.

### 5d. Risk callouts
- **HN miss:** if HN doesn't catch fire, the Reddit + blog + newsletter sequence still produces real downloads. Not a single point of failure (unlike the original plan).
- **Comment-section ambush:** prepare for "this is just SuperTokens with extra steps" comments. Have an honest answer ready (and probably acknowledge the comparison rather than fight it).
- **Solo-dev audience capture:** if launch drives a flood of solo-dev signups (which it might), do NOT optimize for them — that re-triggers the M0e mismatch. Stay focused on small-team paying-ICP outreach.

**See `launch_playbook.md` for full hour-by-hour detail.**

---

## Section 6 — Pricing & packaging

### 6a. Price BAND question

**Did the price band ($99/mo + $0.001/MAU) inherit from competitor anchoring or ICP WTP evidence?**

Almost certainly competitor anchoring — and miscalibrated:
- Clerk: $25/mo + $0.02/MAU
- AuthForge: $99/mo + $0.001/MAU

The $0.001/MAU figure is 20x cheaper than Clerk. That is a "commodity" signal to the exact buyer segment AuthForge targets (small/mid teams currently paying Auth0/Clerk at scale).

**The cheap-MAU pricing fails M0d-adjacent logic:** the segment that hits MAU pain at scale is willing to pay real money to NOT hit it again. Pricing 20x below the alternative reads as "untrusted, may not last, may not scale, why is it so cheap." Stripe/Twilio/Sentry don't undercut by 20x on usage pricing — they undercut by 1.5-3x on enterprise tax, and charge full freight on the usage component because usage IS the value.

**Recommended pricing redesign:**
- **Free tier:** OSS SDK + self-host with no MAU limit (matches Sentry/SuperTokens). 100% MIT.
- **Starter:** $49/mo managed instance (rebranded from $99 because $99 is mid-priced for solo dev / undersized for teams) up to 10K MAU. Includes basic SSO.
- **Pro:** $299/mo, includes SAML SSO, audit logs, multi-tenant org models, 100K MAU. Real team-tier price.
- **Scale:** custom enterprise pricing past 100K MAU + compliance package.
- **Usage component:** $0.01/MAU above included tier (NOT $0.001 — that's 10x corrected; still 2x cheaper than Clerk, signals "we know our value").

**Specific failure mode flagged from anti-pattern #7:** matching/undercutting the cheapest competitor signals "commodity." AuthForge's actual buyer at $99-$299 is team-tier, time-poor, trust-buying. Price near the band ceiling for trust signaling, not the floor.

### 6b. Standard packaging coverage
- **Trial mechanic:** managed-instance free trial 14 days, credit card required (not no-CC). The no-CC trial would re-trigger M0d freebie-disqualifier (selects for tire-kickers).
- **Annual discount:** 20% off annual billing. Annual billing dramatically improves retention (RevenueCat data well established).
- **Pricing model:** per-org + per-MAU hybrid (not per-seat — auth doesn't price per-seat naturally).

---

## Section 7 — Post-launch growth loops

What compounds:
- **Docs/SEO:** ✓ framework tutorials compound for years (Stripe playbook)
- **GitHub stars + contributor visibility:** ✓ each star/adopter logo is a forever marketing asset
- **Newsletter:** ✓ recurring audience, compounds with each issue
- **Brand:** ✓ if launch tonal rule is followed, dev-community trust compounds

What's linear:
- **Cold outreach** — labor-intensive, doesn't scale
- **Podcast guesting** — quality but linear in founder time

What's missing entirely:
- **Product virality:** auth has no natural product-virality loop (unlike, say, Loom or Figma where the product CREATES outbound exposure). AuthForge will NOT grow through product-led virality. This is OK but needs explicit acknowledgment — it means audience-led growth is the only mechanism.

**Strategic risk:** absent product virality, content + docs + GitHub + newsletter are the entire compounding surface. If any one fails, growth slows materially.

---

## Section 8 — Metrics & instrumentation

### Real metrics to track
- **Newsletter subs (weekly delta)** — leading indicator of audience reach
- **Framework tutorial SEO ranking** — track positions for ~20 long-tail queries
- **GitHub stars + watcher + contributor delta (weekly)** — repo health signal
- **Design-partner cohort engagement** — weekly active per cohort
- **Hosted-tier trial-to-paid conversion** — track from trial start
- **Hosted-tier MAU growth per paying customer** — leading indicator of LTV
- **Self-host install metrics (if telemetry enabled with opt-in)** — total install base
- **Sentry-style "scaling moment" tracking** — when does a self-host user start asking about hosted tier? Instrument outreach.

### Vanity metrics to explicitly NOT chase
- Twitter follower count (weakly correlated with paying conversions for this product)
- Total GitHub stars in isolation (M0d: stars ≠ buyers; track stars+contributors+adopters)
- HN upvote count (correlation with revenue is near-zero — well documented)
- Total OSS installs without engagement breakdown

---

## Section 9 — Risk analysis

| Risk | Likelihood | Severity | Mitigation |
|---|---|---|---|
| SuperTokens response — they accelerate or copy AuthForge positioning | High | Medium | Lean on Stripe-alum brand + founder-blog distinct narrative. Don't fight on features; fight on developer story. |
| HN launch flops | Medium | Medium | Section 5 plan is multi-channel; HN is not single point of failure |
| Auth0/Clerk drop pricing in response | Medium | High | Hard to mitigate. Counter-positioning: emphasize OSS + escape-hatch (their pricing can change; AuthForge can't be taken away) |
| Solo-dev signup flood crowds out paying-team focus | High | Medium | Stay disciplined on M6 named-outreach plan. Free-tier is OK; don't tune product for free-tier. |
| Founder content cadence slips due to build pressure | High | High | The 30% time-on-audience rule is load-bearing. If it slips for 4+ weeks, re-prioritize. |
| Compliance buyers ask for SOC2/HIPAA/etc before paying | Medium | High | Acknowledge enterprise readiness is roadmap; route compliance-buyers to "we're not there yet, here's our path" — DO NOT pretend |
| GitHub-as-marketing fails (low stars, looks dead) | Medium | High | Contributor recognition program + framework SDK fan-out are designed to populate the repo with activity. Required pre-launch. |
| Pricing gets re-anchored cheaper by community pressure ("$49 is too expensive for a side project") | High | Low | Side projects aren't ICP. Free tier serves side projects. Hold price for paying ICP. |

---

## Outside voice

(For real run, would invoke Claude subagent or Codex CLI. For smoke-test, surfaced internally below.)

**Single biggest risk inside review may have missed:** AuthForge has chosen one of the most crowded categories in dev tooling. Even with perfect execution on the v0.3 plan, the question "why does the world need a 12th open-source auth provider" is unanswered. The founder's existing 20K dev-blog readership and Stripe-alum brand may NOT be enough differentiation for the auth category specifically, where buyers are extra-conservative (it's security-critical infrastructure). Outside voice would push: is there a wedge — a specific framework or scaling-pain niche — where AuthForge can be THE answer rather than another answer?

**Possible reframe:** instead of "another auth provider," frame as "the auth migration tool" — a product designed specifically for the moment a team is leaving Auth0/Clerk/Supabase Auth because of pricing or coupling. The plan should then optimize for that specific moment, not for general "build auth into your app" demand.

---

## Three strongest action items for THIS week

1. **Start the newsletter NOW.** Convert blog list to Substack/Beehiiv. Ship first issue this week. (Without this, the 20K blog readership is unowned — a Google algorithm change could vaporize it.)
2. **Ship the first 2 framework integration tutorials** (Next.js + Remix) as drafts. Publish even before AuthForge is launched. This starts the SEO compounding clock.
3. **Reach out to 10 named potential design partners** from M6 list. Goal: 3 confirmed alpha users by end of week. Direct email, no funnel.

---

## Handoff
- Artifacts: `marketing_plan.md` (this doc), `icp.md`, `launch_playbook.md`
- Re-run this skill in 30 days to evaluate progress (newsletter signups, tutorial publish count, design-partner count)
- Recommend follow-up: `/plan-eng-review` to lock framework-SDK adapter architecture; possibly `/plan-ceo-review` if the "auth migration tool" reframe (above) is taken seriously.
