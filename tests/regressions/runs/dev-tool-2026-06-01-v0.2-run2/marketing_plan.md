# AuthForge — Marketing Plan (CMO Review v0.2 — Run 2)

**Product:** AuthForge — open-source authentication / identity SDK (MIT) + hosted tier ($99/mo for managed instance + $0.001/MAU above 10K)
**Founder:** ex-Stripe engineer, ~3K Twitter followers, popular technical blog with ~20K monthly readers, no prior shipped products
**Differentiation claim:** "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)"
**Founder's stated validation gate:** 100 GitHub stars + 5 hosted-tier signups by day 60
**Founder's stated distribution plan:** "Show HN at launch + post on r/programming + write integration tutorials"
**Founder's stated first 10 customers:** "GitHub stargazers who upgrade to hosted tier"
**Review date:** 2026-06-01
**Mode:** Mode A — Full Marketing Review (founder qualifies: ICP-aligned audience exists; both distribution surface AND competitive context are within reach)
**Default posture note:** Marketing-naive default is PARTIALLY overridden. Founder has a genuinely ICP-aligned audience (blog readers = backend engineers = exact AuthForge ICP; dev-Twitter = same). Audience-existence assumption survives. Tactical marketing claims (pricing, channels, launch sequencing, validation gate, "GitHub stargazers convert" assumption) STILL get challenged per default.

---

## PREMISE-LEVEL FINDINGS BLOCK

**3 of 5 premise checks failed. 2 survive.** Read this before the tactical sections.

- **M0a — launch platform audience-class fit: PASS.** HN is the right audience class for an OSS auth SDK targeting backend engineers. This is the canonical use-case for Show HN (dev tools, dev infra). Founder gets credit here. BUT: HN base rates have collapsed — 28K Show HN posts in 2025, median post = 2 points. "Show HN" as a CHANNEL is correct; "Show HN" as the ENTIRE launch is still a lottery ticket. The premise survives at the audience-class level and fails at the sufficiency level.
- **M0b — canonical-success comparable: FAIL.** Founder's plan has no anchor against canonical OSS-to-paid successes (PostHog, Supabase, HashiCorp, Sentry, Cal.com). All five of these had multi-quarter audience-building BEFORE OSS launch, hosted-tier at materially higher price points than $99/mo flat, and used the OSS repo itself as the top-of-funnel — NOT as the conversion event. Founder is implicitly following an idealized "Show HN → stars → conversions" funnel that PostHog explicitly says doesn't work that way (they hit 100K customers via OSS + content + 9 products, not via launch-event conversion).
- **M0c — anti-feature surface: FAIL.** The MIT-licensed full OSS SDK that is self-hostable WITH the differentiation claim of "open-source (unlike both)" creates a structural anti-feature: the highest-skill backend engineers (the dogfood ICP) will self-host and never pay. The hosted tier serves the SEGMENT that won't self-host — which is a different ICP than the one HN/r/programming/blog audience represents. The founder is dogfooding for and marketing to Segment A while pricing for Segment B. See M0e for the resulting tuning mismatch.
- **M0d — freebie-disqualifier / acquisition mechanic: FAIL.** "GitHub stargazers who upgrade to hosted tier" is the explicit first-10-customers path. GitHub stars are the canonical low-commitment signal: a star takes 0.5 seconds, costs $0, and selects for time-rich/curiosity-driven engineers who star repos as a "read it later" mechanism. Industry data: stars are documented as showing curiosity, NOT purchase intent. Most OSS tools begin monetization at 500–2,000 stars; conversion rates from stars to paid are not even commonly published because they're so low. The path "stars → hosted-tier upgrade" is an acquisition-mechanic mismatch.
- **M0e — dogfood vs paying ICP mismatch: FAIL.** Founder (ex-Stripe engineer) is dogfooding for sophisticated backend engineers. That cohort is precisely the cohort that will self-host MIT-licensed auth and never pay $99/mo for a managed instance. The PAYING ICP for the hosted tier is the engineer who values their time more than $99/mo — typically: small-team CTOs at funded startups, solo founders shipping fast, agencies who bill by the project. The hosted-tier ICP is not the OSS-dogfood ICP, and the marketing surface (HN, r/programming, technical blog) over-indexes on the dogfood ICP.

**Cascading implication:** the entire validation gate ("100 GitHub stars + 5 hosted-tier signups") is internally inconsistent. Hitting 100 stars is plausible from this founder's audience; hitting 5 hosted-tier signups from THAT pool is not, because the people who star are NOT the people who would pay $99/mo. The founder needs either (a) a different paying-ICP-aligned distribution surface, or (b) a different monetization model that captures value from the cohort who actually shows up (e.g., enterprise tier sold via outbound, or pure consumption pricing with no flat $99 floor).

---

## Step 0 — Pre-review system audit

### Existing artifacts read

The "design doc" for this review is the prompt-embedded product brief. No separate design_document.md, no /office-hours output, no /plan-ceo-review output exists. The founder's stated marketing artifacts are: ~3K Twitter followers, ~20K monthly blog readers, no prior shipped products.

### Competitive landscape (web-searched)

Top direct competitors in dev-facing auth SDK space (2026):
- **Clerk** — $0.02/MAU after 10K free; drop-in React/Next.js components; the "DX-led" winner for small/mid apps. Closed-source.
- **Auth0** (Okta) — $0.07/MAU after 7.5K free; enterprise-heavy; configuration surface enormous. Closed-source.
- **Supabase Auth** — $0.00325/MAU after 50K free (bundled into Supabase platform); RLS-integrated; open-source backend.
- **Stytch** — $0.01/MAU consumer, $0.05/MAU B2B Growth; acquired by Twilio Nov 2025.
- **WorkOS / AuthKit** — free up to 1M MAU; $2,500/mo per additional 1M; B2B-focused; SSO/SCIM the wedge.
- **FusionAuth** — self-hostable, open-core; established OSS-friendly competitor.
- **Better Auth** — newer OSS challenger gaining traction.
- **SuperTokens** — open-source auth, hosted tier.

**Critical finding:** AuthForge's claim "open-source (unlike both Auth0 and Supabase Auth)" is partially wrong. Supabase Auth is open-source. FusionAuth, SuperTokens, and Better Auth are already established OSS-with-paid-tier competitors. The "open-source moat" is not a moat; it's table stakes in this category and crowded.

### Canonical-success comparables (for OSS dev tool → paid hosted tier motion)

- **PostHog** — open-source product analytics; YC; hit Show HN with MVP at 4 weeks; 300 deployments in days from HN trending; ~$39M raised; >100K customers paying-or-free; "enduringly low prices"; cloud-hosted tier is the conversion engine.
- **Supabase** — Firebase alternative; OSS Postgres platform; bottom-up dev adoption; hosted tier the primary revenue; community-led marketing.
- **HashiCorp** — Terraform/Vault; OSS for individuals, paid for orgs (RBAC, governance, audit); explicitly targets central IT/platform teams for paid conversion. NOT individual dev conversion.
- **Sentry** — error tracking; OSS-licensed core then BSL; hosted tier is the revenue; massive community investment ($750K back to OSS).
- **Cal.com** — OSS Calendly alternative; bottom-up adoption; hosted tier.
- **Plausible** — OSS analytics; small team; hosted tier; explicit Google Analytics positioning.

**Pattern (highly load-bearing):** every canonical OSS-to-paid success monetizes orgs/teams, not stargazers. Individual stars are top-of-funnel awareness; paying customers come from (a) teams who don't want ops burden, (b) enterprise features only available in paid, or (c) consumption-pricing at scale.

### Founder audience audit

- Twitter/X: 3,000 followers (small but ICP-aligned — dev-Twitter, technical)
- Blog: ~20,000 monthly readers (large for an individual technical blog; this is the strongest single asset)
- Newsletter: none stated
- LinkedIn: none stated
- GitHub: prior projects? not stated — must verify before launch
- Community presence: none specifically named
- Prior shipped products: zero

**Audience-existence verdict:** Founder qualifies for Mode A. Blog readership of 20K/month is a real distribution surface for an OSS dev tool. The marketing-naive default is partially overridden on the audience-existence question. It is NOT overridden on monetization tactics — the founder has no prior shipped paid product, so all assumptions about conversion and pricing remain suspect.

### Activation rule applied

Founder has substantial prior audience + (now) competitive analysis → **Mode A — Full Marketing Review.**

---

## Step 0.5 — Premise audit (M0a–M0e, with web evidence)

### Premise extraction

| # | Accepted premise | Source | Likely-wrong hypothesis |
|---|---|---|---|
| 1 | Show HN is the right launch | "Distribution Plan" | Sufficiency, not audience-class — base rate collapsed |
| 2 | "Backend engineers building auth into apps" is the paying ICP | "Target users" | Conflates OSS-user ICP with hosted-tier-paying ICP |
| 3 | $99/mo flat + $0.001/MAU after 10K is the right pricing structure | "Distribution model" | Band may be wrong; competitor anchoring; no WTP evidence |
| 4 | GitHub stargazers will upgrade to hosted tier | "First 10 customers" | Acquisition-mechanic mismatch — stars do not predict pay |
| 5 | 100 stars + 5 paid signups by day 60 = validation | "Validation gate" | Internally inconsistent given premise 4 failure |
| 6 | OSS+hosted-tier is a moat ("unlike both") | "Differentiation" | Factually wrong — Supabase Auth, FusionAuth, SuperTokens, Better Auth already OSS |
| 7 | "Simpler than Auth0, more flexible than Supabase Auth" is unique positioning | "Differentiation" | Clerk already owns "simpler than Auth0" via DX |

### M0a — Launch-platform audience-class fit

**Verdict: PASS (audience-class), FAIL (sufficiency).**

HN is the canonical audience class for OSS dev tools and dev infrastructure. Backend engineers are HN's modal reader. Show HN is the correct platform-class choice — this is NOT the tldrof "HN is wrong audience" pattern.

However, sufficiency fails. Per 2026 data: 28,302 Show HN posts in 2025 (3x pre-COVID), 200+ per day in 2026. Median Show HN post = 2 points. r=0.29 correlation between HN score and GitHub stars. Top 6% = 50+ points; top 1% = 250+. Even at correct audience class, the base rate makes "Show HN" alone a lottery ticket. The founder's plan treats HN as the LAUNCH; it should be one channel in a sequence that LEVERAGES the existing 20K blog readers + 3K Twitter followers BEFORE HN posting.

**Cascading implication for M2/M5:** the launch sequence MUST front-load owned-audience activation (blog post, email list, Twitter thread) at least 7-14 days BEFORE the Show HN, so HN engagement comes from a primed crowd rather than cold.

### M0b — Canonical-success comparable

**Verdict: FAIL.**

The founder has not anchored against PostHog / Supabase / HashiCorp / Sentry / Cal.com / Plausible. Every one of these is the relevant playbook. The founder's plan (Show HN + r/programming + tutorials) is from-first-principles where well-documented playbooks exist.

Specific deltas:
- **PostHog** front-loaded a YC launch, a documented founding-story content series, and hit Show HN with a deliberate setup — not "ship and post."
- **Supabase** spent months building dev-Twitter and Discord presence BEFORE the public hosted-tier push.
- **HashiCorp** explicitly sells to ORGS, not individuals — the AuthForge plan implicitly tries to convert individuals at $99/mo flat, which is a category error.
- **Sentry / Cal.com / Plausible** all use consistent content cadence (not one-time launch) as the compounding channel.

**Delta with current plan:** AuthForge plan treats the launch as the marketing moment. Canonical playbooks treat the launch as week 1 of a 52-week content+community grind. The plan is missing the grind.

### M0c — Anti-feature surface

**Verdict: FAIL.** At least 2 anti-features identified.

- **Anti-feature 1: Full MIT-licensed self-hostable SDK.** The differentiation claim is "open-source (unlike both)," but a fully self-hostable MIT-licensed auth SDK actively cannibalizes the hosted tier. The HN/r/programming/blog-reader audience is precisely the population most likely to self-host competently. Look at HashiCorp's model: free for individuals, paid for orgs with GOVERNANCE features individuals don't need. AuthForge has no such split. Fix: kill the "fully open-source" framing in favor of "open-core" with hosted-tier exclusives (multi-tenant management UI, audit logs, SSO/SCIM, support SLAs, compliance attestations) that map to org needs not individual needs.
- **Anti-feature 2: "Simpler than Auth0" positioning + open-source.** "Simpler" implies opinionated, low-config, drop-in. Open-source self-host implies configurable, customizable, ops-aware. These are in tension. Clerk wins "simpler" because they made the call to be closed-source and run all the ops themselves. AuthForge cannot be Clerk-simple AND self-hostable; the two product surfaces diverge.
- **(Optional anti-feature 3): BYO-instance + per-MAU pricing.** $99/mo flat + $0.001/MAU above 10K is a usage tier; combined with "managed instance" (single-tenant?), pricing is too low for a single-tenant managed deployment and too high for the casual stargazer. The pricing serves no one cleanly.

### M0d — Freebie-disqualifier / acquisition-mechanic selection bias

**Verdict: FAIL.**

"GitHub stargazers who upgrade to hosted tier" is the explicit acquisition path. GitHub stars are the lowest-commitment signal in the dev ecosystem:
- Star cost: 0.5 seconds, $0
- Most stars = "read it later" / "track this lib" / "show support"
- Industry evidence: monetization typically begins at 500–2,000 stars; conversion from stars to paid is so low it's rarely published as a benchmark
- Specific failure mode: the stargazer cohort is "dev who wanted to evaluate an auth SDK." The paying cohort is "dev who values their time more than $99/mo of ops burden." These are different humans.

PostHog's path: they DID launch on HN and trended on GitHub — but the 100K customers (paying or free) came from years of OSS distribution + content + product expansion to 9 products, not from launch-week star conversion.

**Acceptable acquisition mechanics for paying ICP of a hosted auth tier:**
- Referral from a team that already pays (trust-led)
- Free trial of hosted tier with manual concierge onboarding (founder personally helps team integrate)
- Outbound to small-team CTOs / agencies / solo founders shipping production apps
- Content-led: high-quality integration guides that rank on SEO for "auth for [framework]" queries, which attract devs WITH a paying need today
- Partner channel: integration listings in framework ecosystems (Next.js, Remix, SvelteKit)

### M0e — Dogfood vs paying ICP

**Verdict: FAIL.**

Founder is ex-Stripe engineer. Dogfood audience = sophisticated backend engineers. Blog audience = same. Twitter audience = same. Dogfood = HN audience = OSS-user ICP.

Paying-tier ICP for a $99/mo hosted auth = team that does NOT want to run their own auth ops. Sophisticated backend engineers WILL run their own auth ops — that's the whole point of MIT-licensing it for them.

The paying ICP is one of:
- **Solo founder / small startup CTO** who is shipping a SaaS in 4 weeks and just wants auth done — they will pay for managed but they're price-sensitive and Clerk's drop-in components beat AuthForge's "SDK"
- **Agency** building 5+ client projects per year — they want a partner program, not stars
- **Mid-size company** that wants enterprise features (SSO, SCIM, compliance) — they want WorkOS, not a $99/mo flat tier

NONE of these three are the natural blog reader / HN browser / r/programming poster. The dogfood-vs-buyer mismatch is structural.

### Step 0.5 completion summary

- M0a: PASS (audience-class) / FAIL (sufficiency)
- M0b: FAIL
- M0c: FAIL
- M0d: FAIL
- M0e: FAIL

4 of 5 fail (with M0a half-pass). Premise-level findings block at top is load-bearing for the rest of the plan.

---

## Step 0A — Forcing questions (simulated naive founder answers + skill challenges)

### M1 — Audience reality

**Founder (naive):** "Backend engineers building auth into their apps."

**Skill challenge:** That's a job-title category, not a person. Refuse.

**Founder (second attempt):** "OK — devs like me. Indie devs, maybe early-stage startup engineers. They read HN, they're on dev Twitter, they follow people like @swyx, @t3dotgg, @leerob."

**Skill challenge:** Closer, but the question is WHICH person actually CONVERTS to paid. The OSS user persona and the hosted-tier-payer persona are different humans. Define the PAYER specifically.

**Accepted answer (extracted/composite):**
*"Persona: Maya, technical co-founder of a 4-person seed-stage Y Combinator startup building a vertical SaaS in fintech compliance. Stripe alum (knows the founder by reputation from blog). Ships in Next.js. Currently using Clerk because it took 8 minutes to integrate. Pays $25/mo to Clerk. Pain points: Clerk gets expensive past ~5K MAU; she wants more control over the auth UI; she's vaguely uncomfortable with closed-source for an auth layer. Spends time on: HN (daily), dev Twitter (heavy), Lenny's Newsletter, swyx blog, Vercel blog, t3dotgg YouTube, /r/nextjs occasionally. Would convert from Clerk if AuthForge had drop-in Next.js components AND price/MAU lower than Clerk AND she trusted the maintainer (the blog credibility is load-bearing here)."*

This persona is the only one realistically convertible from the founder's existing audience surface.

### M2 — Discovery path

**Founder (naive):** "She sees my Show HN post."

**Skill challenge:** REFUSE. Step 1 is not Show HN, especially given M0a sufficiency failure.

**Accepted answer:**
1. **Step 1:** Maya reads founder's existing technical blog post titled something like "What I learned shipping auth at Stripe" (founder's existing 20K-monthly-readers surface). Builds trust.
2. **Step 2:** Maya follows founder on Twitter after the blog post. Sees a build-in-public thread series leading up to AuthForge.
3. **Step 3:** Maya sees Show HN post AFTER it has been primed by the 20K blog audience + 3K Twitter followers + email list (which founder should be building NOW). HN front-page risk drops materially because primed audience supplies initial upvotes within first hour.
4. **Step 4:** Maya tries the OSS SDK, integrates in <10 min (TTHW industry benchmark = 5 min, must beat). Reads the hosted-tier docs.
5. **Step 5:** Maya stays on OSS for prototype phase. Converts to hosted tier when she crosses 10K MAU OR when team grows to 4+ engineers and ops burden gets real OR when SOC2 audit forces compliance question.

**Realistic time-to-paying:** 6-12 months from first blog touch. Not launch week.

### M3 — Pre-launch audience

**Founder (naive):** "I have 3K Twitter, 20K monthly blog readers. That's pretty good right?"

**Skill challenge:** It's the most ICP-aligned audience asset of any founder I'd advise. But: zero email subscribers, zero Discord, zero GitHub waitlist, zero newsletter. Twitter algorithm + blog SEO are RENTED audiences. You don't own them. The work item before launch is to convert blog readers + Twitter followers into an owned audience (email list).

**Accepted answer:** Substantial ICP-aligned RENTED audience. ZERO owned audience. Pre-launch work item: install email capture on blog (target: 1,000 email subs from existing readership in 30 days), launch a sparse-cadence dev-Twitter-adjacent newsletter (monthly is fine; weekly is overkill while building), and create a GitHub waitlist repo for AuthForge.

### M4 — Channel honesty

**Founder (naive):** "I'm good at Twitter and writing."

**Skill challenge:** Twitter following of 3K is small (Clerk's founder Colin Sidoti has >20K, Theo has >300K, swyx >100K). Calling Twitter your channel advantage is overclaiming. Blog is the actual asset.

**Accepted answer:** The blog (20K monthly readers, technical depth, ex-Stripe credibility) is the credible, demonstrable channel advantage. No other founder in the auth-SDK category has equivalent owned long-form distribution. Twitter is supporting, not lead. HN is a launch event, not a channel. Real channel: **owned blog + email list converted from it.**

### M5 — Competitor traffic source

**Founder (naive):** "I don't really know."

**Skill challenge:** Then you're flying blind. Commitment to find out before next session.

**Accepted answer (skill provides starting points):**
- **Clerk:** dev-Twitter heavy (Colin Sidoti + team are HEAVY on Twitter), Next.js ecosystem integration (Vercel partnership), drop-in component virality (devs share screenshots), YC network. SimilarWeb shows strong direct + referral from Vercel / Next.js docs.
- **Supabase Auth:** organic from Supabase platform usage (bundle effect), heavy YouTube content (founders + DevRel), Discord community (large), Google search for "Firebase alternative."
- **Auth0:** SEO-dominant for "authentication" terms; enterprise sales motion; conference presence; declining mindshare among new builds.
- **Stytch:** developer-focused content marketing; YouTube; SDKs.io presence; now Twilio's distribution post-acquisition.
- **WorkOS:** content marketing (workos.com/blog is exceptional), SEO for "SSO" and "SCIM" terms; outbound to mid-market.

**Founder action item:** founder must spend 2 hours studying Clerk's Twitter cadence and Supabase's DevRel rhythm before week 1 of pre-launch.

### M6 — First 10 paying customers

**Founder (naive):** "GitHub stargazers who upgrade."

**Skill challenge:** REFUSE per M0d. Stars are not paying intent. Name 10 humans.

**Accepted answer (constructed):**
1. 5 named ex-Stripe colleagues now at YC startups (warm outreach; trust pre-built)
2. 3 named YC W26 / S26 batch CTOs the founder can reach via Stripe alumni network
3. 2 indie hackers from the founder's blog comments / Twitter DMs who've publicly complained about Clerk pricing

**Action:** founder must produce this list (real names) BEFORE the launch sequence runs. The first 10 are not discovered; they are recruited.

### M7 — Time allocation

**Founder (naive):** "I'm spending 90% on building. I'll do marketing after launch."

**Skill challenge:** REFUSE. The 20K blog audience is decaying every week the founder is not posting. Twitter is decaying. The email list that should exist doesn't.

**Accepted answer:** Founder commits to ≥40% audience-building from today until launch:
- 2 blog posts/month minimum (one per fortnight) tied to AuthForge-relevant topics (auth at Stripe, OSS-vs-closed, etc.)
- 3-5 Twitter threads/week
- Daily Twitter engagement (not just posting — replying in dev-Twitter)
- Email list build (capture form live on blog within 7 days)
- Build-in-public weekly thread

If this feels like too much, the founder is admitting they prioritize building over distribution — which is the bug this skill exists to catch.

---

## Step 0B — Mode selection

**Mode A — Full Marketing Review.** Founder has substantial ICP-aligned audience surface (20K blog readers + 3K dev-Twitter) AND a category with rich web-searchable competitive landscape. Full review applies. All 9 sections below.

(Notably, Mode C — Audience-Build Sprint — would apply if the founder had ZERO audience. They don't. But the OWNED audience layer (email list) is at zero, so a Sprint-style sub-plan is rolled into Section 4.)

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | Founded | Pricing | Acquisition channel | Position |
|---|---|---|---|---|
| **Clerk** | 2019 | $0.02/MAU after 10K free | Dev-Twitter, Vercel/Next.js partnership, drop-in components viral on dev Twitter | "DX-led winner" for React/Next.js indie + small SaaS. **Winning the modal AuthForge ICP.** |
| **Auth0** (Okta) | 2013 | $0.07/MAU after 7.5K free | SEO dominance, enterprise sales | Enterprise-default; losing developer mindshare; expensive at scale |
| **Supabase Auth** | 2020 | $0.00325/MAU after 50K free (bundled) | Supabase platform pull-through, YouTube, Discord, "Firebase alternative" SEO | Default if already on Supabase; bundle effect is its moat |
| **Stytch** (Twilio) | 2020 | $0.01/MAU consumer, $0.05 B2B Growth | Dev content, SDKs.io, now Twilio distribution | Solid passwordless; Twilio acquisition raises vendor-risk for some buyers |
| **WorkOS** | 2019 | AuthKit free to 1M MAU, then $2,500/mo per 1M | Content marketing (workos.com/blog), SEO for "SSO"/"SCIM" | B2B enterprise; SSO/SCIM the wedge; rapidly expanding |
| **FusionAuth** | 2018 | Free self-host; paid tiers for support/cloud | Established OSS community; SEO | Direct OSS competitor; AuthForge "open-source unlike both" claim is wrong because of this |
| **Better Auth** | 2024-25 | OSS; emerging hosted tier | Dev-Twitter, GitHub momentum | Newer OSS challenger; growing fast among Next.js devs |
| **SuperTokens** | 2019 | OSS self-host; paid managed | Dev content, Reddit, HN | Direct OSS+managed competitor |

**Honest assessment:** Clerk is winning the segment AuthForge most plausibly serves. FusionAuth/SuperTokens/Better Auth already occupy the OSS+hosted niche. Supabase Auth wins anyone on Supabase. Auth0 owns enterprise. WorkOS owns B2B SSO. **There is no obvious oxygen in this market for a generic OSS+hosted auth SDK.** The wedge must be more specific than "simpler than Auth0, more flexible than Supabase Auth."

### 1b. Canonical-success comparables (OSS dev tool → paid hosted tier motion)

| Company | Price | Founded | Scale | Primary acquisition | Onboarding | Launch gate |
|---|---|---|---|---|---|---|
| **PostHog** | "enduringly low" + usage | 2020 | $39M raised; 100K+ customers | Show HN as MVP; OSS-on-GitHub trending; content; YC network | Self-serve OSS; hosted cloud is conversion | Calendar (4-week MVP to HN); PMF emerged via OSS adoption signal |
| **Supabase** | $25/mo Pro + usage | 2020 | $100M+ Series C | OSS-on-GitHub; "Firebase alternative" SEO; massive YouTube + DevRel; Discord | Self-serve + heavy DevRel | OSS proof-of-traction before hosted-tier push |
| **HashiCorp** | Free OSS for individuals; enterprise tiers $$$ | 2012 | IPO 2021 | OSS adoption → enterprise upsell; HashiCorp conferences; ecosystem partnerships | Self-serve OSS; enterprise sales | Sold to ORGS for governance — not to individuals |
| **Sentry** | $26/mo team; $80/mo business | 2008 | Hundreds of millions ARR | OSS first; SDK ubiquity; content; community ($750K back to OSS) | Self-serve SDK; hosted is primary revenue | OSS-to-paid via team-size triggers |
| **Cal.com** | $15/mo Pro, enterprise tier | 2021 | $32M raised | OSS-on-GitHub trending; build-in-public Twitter (Peer Richelsen); content; "Calendly alternative" SEO | Self-serve + hosted | OSS traction before scale |
| **Plausible** | $9-19/mo | 2018 | Bootstrapped to $1M+ ARR | "Google Analytics alternative" SEO; privacy positioning; content | Hosted-only (OSS available but not pushed) | Bootstrapped — conservative gates |

### 1c. Pattern surface

**Common to every canonical success:**
- Multi-quarter pre-launch OR multi-quarter post-launch content/community grind (not "ship and Show HN")
- Hosted tier price aligns with target buyer's WTP — PostHog and Cal.com hit individuals/teams cheaply; HashiCorp hits enterprise at high price; **AuthForge's $99/mo flat fits NEITHER segment cleanly**
- The OSS repo is top-of-funnel awareness; the paying customer is recruited through a different motion (content, DevRel, enterprise sales, team-size triggers)
- Build-in-public + founder-as-character is a recurring pattern (Peer at Cal.com, Tim/James at PostHog, Paul at Supabase, Marcelo at Sentry)
- A specific "alternative-to-X" positioning that maps to a Google search query (Cal.com → Calendly; Plausible → Google Analytics; Supabase → Firebase). AuthForge has no such position because "alternative to Auth0/Supabase Auth/Clerk" is already crowded.

**AuthForge plan implicitly follows:** the "launch-week conversion" pattern, which is not the canonical OSS-to-paid playbook. Closest false analog is PostHog's HN launch — but PostHog's launch was THE START of a multi-year grind, not the validation event.

**Founder action:** read PostHog's "How we got here" handbook (posthog.com/handbook/story) and Peer Richelsen's build-in-public Twitter cadence for Cal.com. Both publicly documented.

---

## Section 2 — ICP specification

**Persona: Maya — Technical Co-founder / CTO, seed-stage YC-style SaaS startup**

- **Stage:** seed-stage, 4-12 person team, post-pre-seed pre-Series-A
- **Stack:** Next.js / TypeScript / Postgres / Vercel; React Native for mobile if applicable
- **Current auth:** Clerk ($25-200/mo bracket), or rolling-own-with-Lucia/NextAuth and regretting it
- **Pays for:** Vercel ($20-100/mo), Linear ($8/seat), Posthog (free or paid), GitHub Copilot, Cursor ($20/mo), Resend ($20/mo)
- **Where attention lives:**
  1. Hacker News (daily skim, top 30)
  2. Dev Twitter: @t3dotgg, @leerob, @swyx, @rauchg, @adamwathan, founder's own account
  3. Lenny's Newsletter, Pragmatic Engineer
  4. Vercel/Next.js blog
  5. /r/nextjs occasionally
  6. YouTube: Theo, Web Dev Simplified, Fireship
  7. swyx's various
  8. Discord: Next.js, Vercel, Cursor
- **Adjacent-category pay patterns:** $20-50/mo per SaaS tool happily; $200+/mo only for tools that save engineering hours
- **Adjacent complaints about Clerk:** "expensive past 10K MAU," "UI customization limits," "closed-source for our auth layer makes me nervous"
- **Objection patterns to AuthForge:**
  - "Why would I switch from Clerk? Migration is risky."
  - "Is this maintained? Solo founder, no team behind it."
  - "Is $99/mo flat actually cheaper than Clerk for me?"
  - "Self-host vs hosted — what's the actual value of hosted?"
- **Reasons she would convert:**
  - Trust the founder (blog + ex-Stripe credibility)
  - Drop-in Next.js components match or beat Clerk DX
  - Pricing is materially better than Clerk past 10K MAU
  - Owns her auth data (escape from vendor lock-in)

Saved as `icp.md` (separate file).

---

## Section 3 — Distribution channel-by-channel

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Verdict |
|---|---|---|---|---|---|---|
| **Founder's blog (OWNED)** | 20K/mo readers, ICP-aligned | $0 marginal | High (warm, primed) | EXCEPTIONAL | Already paying time cost | **Lead channel.** Highest-leverage asset. |
| **Email list (to be built)** | 0 today; target 1K-2K in 90d | $20/mo (Buttondown/Ghost) | Highest of any | Strong fit | Medium | **Critical work item, week 1.** |
| **Dev-Twitter (OWNED-ish)** | 3K followers, ICP-aligned | $0 | Medium (algorithmic) | Strong | Daily | **Supporting channel.** |
| **Show HN** | Lottery (median = 2 pts) | $0 | High IF hit | Audience match good | Low (one post) | **Launch event, not channel.** Use once, with primed audience. |
| **/r/programming** | Mod-strict; bans common | $0 | Low (broad audience, not paying ICP) | Weak | Low | **Skip or be very careful.** Cross-post day +2 only after HN traction. |
| **/r/nextjs, /r/SaaS, /r/webdev** | Narrower, more ICP-aligned | $0 | Higher than /r/programming | OK | Low-Med | **Better than /r/programming.** Compliant cross-post day +2. |
| **Product Hunt** | One-shot event | $0 | Medium | OK if has hunter relationship | Low | **Day +7-14, separate from HN.** |
| **IndieHackers** | Narrow but tight | $0 | Medium | Good | Low | **Day +1-3.** |
| **Integration tutorials (SEO)** | Slow compound, large eventually | High time | High (intent-matched) | Strong (founder is strong writer) | High over months | **Major channel post-launch.** Target queries like "Next.js auth with [framework]." |
| **DevRel / partner integrations** | Large via Vercel / Next.js / Remix ecosystems | $0 | High (bundled credibility) | Founder needs to build relationships | High | **Major mid-term channel.** Aim for Vercel integration listing within 3 mo. |
| **YouTube** | Large; long compound | Time-heavy | Medium | Unknown — founder hasn't shipped video | High | **Defer unless founder enjoys it.** |
| **Podcast guesting** | Moderate; high-trust | $0 | High per listener | Strong (ex-Stripe + blog credibility opens doors) | Low per appearance | **High-leverage: book 5 podcasts in first 90d.** Targets: Lenny's, syntax.fm, Changelog, ShopTalk Show, Pragmatic Engineer. |
| **Discord presence** | Medium; relationship-built | Time | Medium-high | Good | High | **Build presence in 2-3 Discords (Next.js, Vercel, /r/nextjs Discord) — defer to month 2+.** |
| **Cold outreach to first 10** | Tiny but converts | Time | Highest | Good (Stripe network) | Low | **Mandatory, week of launch.** |
| **Paid ads** | Large | High ($5-15 CPC dev category) | Low for new brand | Weak | High | **Skip until $10K+ MRR.** |
| **Affiliate** | Small | Free | Low | Weak | Low | **Defer.** |

**Surviving prioritized channels (ranked by leverage):**
1. Founder's blog (lead)
2. Email list converted from blog (compounding)
3. Cold outreach to first 10 (immediate)
4. Dev-Twitter (supporting)
5. Podcast guesting (high-leverage per hour)
6. Show HN (single-shot launch event)
7. Integration tutorials / SEO (compound months 3-12)
8. DevRel partnerships (Vercel integration listing) (months 2-6)

Everything else: defer or skip.

---

## Section 4 — Pre-launch audience-building plan (30/60/90)

The founder has rented audience (blog SEO, Twitter algorithm) but no owned audience. The single most important pre-launch work item is converting rented → owned.

### Days 1-30 — Owned audience installation + signal generation

- **Email capture on blog (week 1):** install email signup CTA on every blog post and as a popup on the blog homepage. Target: 1,000 email subs from existing readership in 30 days (~5% capture from 20K monthly).
- **Newsletter launch (week 1):** monthly newsletter, first issue = "Why I'm leaving Big Tech to build OSS auth." Frames the product narrative.
- **Build-in-public Twitter cadence (daily):** 1 quote-tweet + 2 substantive replies + 1 build update per day. Goal: get to 5K followers by day 30.
- **2 long-form blog posts (one per fortnight):**
  - Post 1: "What I learned about auth at Stripe" (credibility-building, no AuthForge mention)
  - Post 2: "Why Clerk is great and where it falls short" (positioning piece, soft AuthForge tease at end)
- **GitHub waitlist repo:** create AuthForge repo, README-as-pitch, "star to follow" CTA. Target: 200 stars from pre-existing audience pre-launch.
- **Recruit first 10 paying customers from network NOW (not at launch):** founder produces actual list of 10 named humans. Begins individual conversations.

### Days 31-60 — Cadence scaling + concierge cohort

- **Email list goal:** 1,500 subs
- **Twitter goal:** 7K followers
- **GitHub stars goal:** 500 stars on the waitlist repo
- **2 more long-form blog posts:**
  - "I tried 8 auth SDKs. Here's what's wrong with all of them." (positioning)
  - "Behind the scenes of AuthForge: design tradeoffs" (build-in-public deep-dive)
- **Concierge cohort onboard:** Founder personally onboards 5 named people from the first-10 list onto a private alpha. Measures: do they integrate in <10 min? Do they use it 5+ times per week? Do they say "very disappointed" if it disappeared (Vohra test)?
- **Podcast outreach:** book 3 podcast appearances for day-60-to-day-120 window.

### Days 61-90 — PMF-signal gate + launch sequence integration

- **PMF signal check:** ≥40% of alpha cohort says "very disappointed" if AuthForge disappeared (Vohra test). If not, DELAY launch by 30 days and iterate.
- **Email list goal:** 2,000+ subs
- **GitHub stars goal:** 1,000+ stars
- **Launch primer post on blog:** "AuthForge launches Friday — here's what it is and why I built it" (3 days before HN post)
- **Email to list:** "Launching Friday, here's early access" (same day as primer)
- **Twitter sequence:** day-by-day countdown thread starting 5 days out
- **Launch day:** see Section 5

**Refused:** "I'll start audience-building after launch." This was the founder's first instinct (M7) and is the build-it-and-they-will-come anti-pattern.

---

## Section 5 — Launch playbook (multi-channel, sequenced)

### 5a. Launch gate question

**Stated gate:** "100 GitHub stars + 5 hosted-tier signups by day 60." This is calendar-driven with two KPIs.

**Skill challenge:** the 5 hosted-tier signups KPI is internally inconsistent with the "stars convert to paid" mechanic (M0d failure). The gate measures the wrong thing for the wrong cohort at the wrong time.

**Proposed alternative gate (PMF-signal-driven):**
- ≥40% of alpha concierge cohort answers "very disappointed" if AuthForge disappeared (Vohra)
- ≥3 of the 10 hand-recruited prospects integrate AuthForge into a production app
- ≥1 unprompted referral from the alpha cohort

If hit by day 60: launch. If not: extend pre-launch by 30 days, iterate, repeat.

**If founder defends calendar gate:** acceptable ONLY if the marketing moment is genuinely time-bound (a vertical conference, a YC Demo Day, a coordinated Vercel partner launch). Otherwise default to PMF gate.

### 5b. Launch sequence

| Day | Channel | Action |
|---|---|---|
| -30 | Blog | Post "What I learned about auth at Stripe" (no AuthForge mention; credibility prime) |
| -21 | Blog + Twitter | Build-in-public weekly thread series begins |
| -14 | Blog | Post "Why Clerk is great and where it falls short" (positioning) |
| -7 | Email list | Soft pre-announce to 1K-2K email subs + 10 hand-recruited prospects |
| -5 | Twitter | Countdown thread day 1 |
| -3 | Blog | Launch primer: "AuthForge launches Friday — here's why I built it" |
| -1 | Twitter | Final hype thread; tag respected dev-Twitter accounts respectfully |
| 0 / 9am PT Tue-Thu | Hacker News | Show HN post; founder ready to reply in comments for 6 hours |
| 0 / 9:15am | Email + Twitter | Email "we're live"; Twitter announcement thread linking HN |
| 0 / +2hr | Twitter | Engagement reply burst as HN starts moving |
| 0 / +4hr | LinkedIn | Long-form launch post (different audience overlap) |
| 0 / +24hr | IndieHackers + /r/nextjs | Compliant cross-posts |
| 0 / +48hr | /r/SideProject, /r/webdev | Cross-posts following community rules |
| 0 / +5d | Outreach | Founder personally emails 10 hand-recruited prospects ("we're live, here's your migration help") |
| 0 / +7d | Product Hunt | Separate launch event |
| 0 / +14d | Podcast guesting | First booked appearance airs |
| 0 / +30d | Blog + Twitter | "30 days post-launch: real numbers, lessons" retrospective |
| 0 / +60d | Blog | Second retro + the first integration tutorial drops (SEO seed) |
| 0 / +90d | Continuous | Integration tutorial cadence (1/week) for SEO compound; podcast cadence (1/month) |

### 5c. Risk callouts

- **HN miss:** plan survives because of primed email list + Twitter + cold outreach + cross-posts. Show HN is not load-bearing alone.
- **/r/programming mod ban:** likely if first post; cross-post to narrower subs instead.
- **Solo-founder trust ceiling:** "is this maintained?" objection is real. Founder must publicly commit to maintenance horizon AND consider adding a co-maintainer / advisory board visibly.
- **Competitor counter-launch:** Clerk could ship "OSS Lite" or Better Auth could position as the dev-Twitter darling. Mitigation: speed + trust capital from blog.

Saved as `launch_playbook.md` (separate file).

---

## Section 6 — Pricing & packaging

### 6a. Pricing band question

**Stated:** $99/mo flat for managed instance + $0.001/MAU above 10K.

**Skill challenge:** Was this competitor-anchored or ICP-WTP-evidenced? Evidence says competitor-anchored.

**Comparable competitor pricing (per-MAU after free tier):**
- Clerk: $0.02/MAU
- Auth0: $0.07/MAU
- Stytch: $0.01-$0.05/MAU
- Supabase Auth: $0.00325/MAU (bundled)
- AuthForge proposed: $0.001/MAU after 10K free

**Problems with the proposed pricing:**

1. **$99/mo flat for a managed instance is too low for actual single-tenant compute.** A real managed instance per customer at $99/mo barely covers AWS infra at any usage. If it's actually multi-tenant ("managed instance" is misleading), then the flat $99 floor is too HIGH for low-usage users (Clerk and Supabase Auth give them free) and prices out the long tail that builds awareness.
2. **$0.001/MAU is suspiciously cheap.** That's 20x cheaper than Clerk, 70x cheaper than Auth0. It signals "commodity" precisely to the segment that buys auth on trust. Per M0d, time-poor/money-rich buyers trust-shop the top of the band, not price-shop the bottom. Pricing AuthForge as the cheapest in the band signals "indie hobby project" to the buyer who would actually pay.
3. **The flat-+-per-MAU structure is incoherent against the OSS option.** Why would I pay $99/mo flat when I can self-host MIT-licensed for free? The $99 has to be paying for something specific: hosted ops, SLA, multi-tenant management, compliance — and none of those are in the offer description.

### 6b. Pricing recommendations

- **Kill the $0.001/MAU price; it signals commodity.** Move to $0.01-$0.02/MAU range (parity to Clerk/Stytch) AFTER the 10K free tier. Defend at parity, not at discount.
- **Reframe the $99/mo flat:** make it a "Pro" tier with named hosted-tier exclusives — multi-tenant management UI, audit logs, SSO/SCIM, support SLA, compliance attestation roadmap (SOC2). Not "managed instance."
- **Add a Team tier at $299/mo and an Enterprise tier with custom pricing** to capture the actual high-WTP segments.
- **Annual billing at 20% discount** to lift retention (industry standard; LTV impact documented).
- **Trial mechanic:** drop the "self-host OSS as trial" assumption (it selects against the paying ICP per M0d). Offer 30-day hosted-tier trial with concierge onboarding for the first 10 paying customers. Trial = founder-led integration call.

### 6c. Revisit M0d freebie-disqualifier

The OSS+paid model itself is a freebie filter. To not let the OSS cannibalize the paid:
- Hosted tier exclusives must be features ORGS need, not features INDIVIDUALS need (HashiCorp model).
- Specifically: SSO, SCIM, audit logs, compliance attestations, multi-tenancy, support SLA. NONE of these are differentiators for the indie dev who would self-host.

---

## Section 7 — Post-launch growth loops

What compounds vs what's linear?

| Loop | Compound or linear? | Strength for AuthForge |
|---|---|---|
| Referral mechanics (in-product) | Compound IF in-product invite | Weak — auth SDK doesn't naturally have viral invite mechanics |
| Content compounding (SEO) | Compound | STRONG — founder is a writer; integration tutorials for "Next.js + auth" / "Remix + auth" / "SvelteKit + auth" / "auth in [framework]" rank well |
| Network effects | Compound | Weak — auth is single-tenant for the user |
| Brand compounding | Compound | STRONG IF consistent — blog + Twitter cadence sustained |
| Retention-as-acquisition (WOM) | Compound | Moderate — devs talk about tools they love but auth is a "boring infra" purchase, less WOM than dev-tools-of-joy like Linear or Cursor |
| Integration partnerships | Compound | STRONG — Vercel listing, Next.js docs, Remix listing |

**Net:** AuthForge's compounding loops are content (SEO + brand) and integration partnerships. NO product-led-growth loop. Acquisition will be content-treadmill, not viral-coefficient. **This is a strategic risk to surface to the founder** — every new customer needs to be earned through new content or new outbound, vs Calendly-style "every customer drives new customers."

Mitigation possibilities:
- Build an in-product "powered by AuthForge" badge that links to the marketing site (mild brand virality)
- Open-source community contributions as a top-of-funnel mechanism (each contributor becomes a brand ambassador)
- Reference customer logo program

---

## Section 8 — Metrics & instrumentation

### Measure weekly

- **Owned audience size:** email subscribers, weekly
- **GitHub repo:** stars, watchers, forks, issues, PRs
- **Blog traffic:** unique visitors, top posts, conversion to email
- **Twitter:** followers, engagement rate, top-performing threads
- **Acquisition by channel (UTMs):** every external link to product gets a UTM
- **OSS-to-hosted conversion:** % of OSS users who try hosted tier, % who convert to paid (probably <0.5% based on industry benchmarks)
- **Trial-to-paid conversion:** % of hosted trial signups who convert; cohort by source
- **Day-7 / day-30 retention** for hosted-tier signups
- **TTHW (Time to Hello World) for OSS SDK:** target <5 min (industry benchmark); ideally <2 min

### Do NOT measure (vanity)

- Total GitHub stars (curiosity metric)
- HN upvotes (near-zero revenue correlation)
- Twitter follower count in isolation
- Tutorial post views without conversion data

### Specific dashboards to ship in week 1

- Posthog cloud for product analytics on hosted tier
- Plausible or Fathom for blog analytics
- Email tool (Buttondown / Ghost / ConvertKit) for owned audience
- Weekly Sunday review ritual: founder updates a simple spreadsheet with 8-10 KPIs

---

## Section 9 — Risk analysis

| Risk | Severity | Mitigation |
|---|---|---|
| **Channel concentration on HN single launch** | High | Multi-channel launch sequence (Section 5); HN is one of 8 channels, not THE channel |
| **OSS cannibalizes hosted tier (M0c)** | High | Reframe hosted-tier exclusives as org-needs-only (HashiCorp model) |
| **Stars don't convert to paid (M0d)** | High | Replace gate metric; recruit first 10 by hand, not from star pool |
| **Dogfood-vs-paying-ICP mismatch (M0e)** | High | Add paying-ICP-aligned alpha cohort (5 named seed-stage CTOs) BEFORE launch; tune product to them |
| **Solo-founder trust ceiling** | Medium | Publicly commit to maintenance horizon; add named co-maintainer / advisors |
| **Clerk competitor velocity (DX leader)** | Medium | AuthForge wedge must be more specific than "simpler/more flexible" — needs to be a narrow framework-or-vertical win |
| **OSS competitor saturation (FusionAuth, SuperTokens, Better Auth)** | Medium | "Open-source unlike both" framing is wrong; differentiate on DX + ex-Stripe credibility + Next.js-first positioning |
| **Pricing band signals commodity (Section 6)** | Medium | Move to Clerk-parity pricing; defend value not discount |
| **Calendar gate fires before PMF (Section 5a)** | High | Use Vohra "very disappointed" signal; delay if not hit |
| **Acquisition-treadmill business model (Section 7)** | Medium | Accept that content + integrations are the compounding loop; staff/time accordingly |
| **Twilio's Stytch acquisition / Okta's Auth0 dynamics** | Low (opportunity) | Vendor-risk-averse buyers leaving for OSS — AuthForge benefits IF positioning is sharp |
| **Founder time allocation (M7) — 90% build, 10% market** | High | Force ≥40% audience-building from today; tracked weekly |

---

## Outside voice (simulated)

Mandatory step. Simulating an independent critique to surface the biggest risk the inside review missed.

**Biggest missed risk:** The whole AuthForge thesis is "OSS auth is a gap" — but the gap is NOT empty. FusionAuth, SuperTokens, Authentik, Keycloak, Better Auth, ORY Kratos all exist. The founder's "open-source (unlike both)" framing means they haven't actually surveyed the OSS landscape. Before launch, the founder needs a defensible answer to "why AuthForge over FusionAuth or Better Auth?" — and that answer probably needs to be Next.js-first DX + ex-Stripe credibility, not just "OSS exists."

**Channel reality check:** Twitter at 3K followers is small. The blog at 20K monthly readers is the actual asset. Inside review correctly weighted blog as lead channel.

**Audience claim that lacks evidence:** "GitHub stargazers who upgrade to hosted tier" — flagged in M0d.

**Provocative reframe:** AuthForge might be a worse positioning as a generic auth SDK than as **"auth-as-an-OSS-library specifically for Next.js founders who think Clerk is too expensive and Auth0 is overkill."** Narrow the wedge to Next.js / Remix / SvelteKit ecosystem. Specifically anti-position against Clerk's pricing curve past 10K MAU. This is a sub-segment where Clerk is genuinely vulnerable (price compression past 10K MAU is a real Clerk complaint surfaced in reviews). A vertical positioning has a chance; a horizontal "OSS auth" positioning is dead in the water.

---

## Action items this week (3 strongest)

1. **Install email capture on blog by end of week; target 200 subs in 14 days** from existing 20K monthly readership. This converts rented audience to owned. (Highest-leverage single action.)
2. **Produce the named list of 10 first paying prospects by end of week** — actual names, actual emails. Begin warm DMs/emails by next week. Not stargazers — humans.
3. **Sharpen positioning to a Next.js-first / framework-first wedge** by end of week. Draft new tagline and product description that anti-positions against Clerk's pricing curve past 10K MAU. Run by 3 trusted dev-Twitter friends for feedback before public.

---

## Re-run check

Re-run this skill in 30 days to evaluate:
- Email subs hit 1,000+?
- First-10 list produced and 3+ in conversations?
- Positioning sharpened?
- Alpha cohort onboarded?
- PMF signal trending toward Vohra threshold?

If yes to 4 of 5 → on track. If no → mode shifts; consider Mode C audience-build sprint or scope reduction.

## Follow-up skills to consider

- **/office-hours** if positioning shift is meaningful (probable)
- **/plan-ceo-review** for the pricing-model rethink and OSS-vs-hosted tier split (probable)
- **/plan-eng-review** for the multi-tenancy / hosted-tier architecture (probable)
