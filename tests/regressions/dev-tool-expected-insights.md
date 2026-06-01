# Regression test fixture — Dev tool / OSS+paid (synthetic) / plan-cmo-review

**Skill under test:** `plan-cmo-review`
**Fixture type:** synthetic (no real founder; constructed product scenario)
**Purpose:** exercise the skill against an open-source dev tool with a hosted/paid tier — different motion from consumer subscription (tldrof) and B2B SaaS (b2b-saas). Catches over-application of either pattern.

## Synthetic input scenario

A fictional founder is building **"AuthForge"** — an open-source authentication / identity SDK with a hosted tier. Their design doc says:

- **Product:** open-source SDK (MIT) + hosted tier at $99/mo for managed instance + $0.001/MAU above 10K
- **Target users:** backend engineers building auth into their apps
- **Distribution Plan:** "Show HN at launch + post on r/programming + write integration tutorials"
- **First 10 customers:** "GitHub stargazers who upgrade to hosted tier"
- **Validation gate:** 100 GitHub stars + 5 hosted-tier signups by day 60
- **Differentiation:** "Simpler than Auth0, more flexible than Supabase Auth, open-source (unlike both)"
- **Founder background:** ex-Stripe engineer, has 3K Twitter followers, popular technical blog with ~20K monthly readers
- **Existing audience:** strong dev-Twitter presence, no prior shipped products

## Why this fixture exists

Dev tools have a third distinct motion class with its own dynamics:

- **HN IS the right audience class** (corrects tldrof's HN-as-category-error pattern)
- **Open-source freemium economics** — most users never convert; the conversion mechanic matters
- **Time-to-Hello-World** is the magic moment (not 60-second backlog clearing)
- **GitHub stars are real social proof** (not vanity for this audience)
- **Docs and tutorials are marketing** — content has SEO compounding
- **Integration ecosystem** matters disproportionately
- **Developer skepticism of marketing** — overt sales-language hurts conversion

A skill that applies consumer-product patterns (audience-build via LinkedIn, freebie-disqualifier framing) or B2B patterns (case studies, ACV analysis, procurement gates) to a dev tool will produce a misaligned plan.

## Expected insights (7 items)

Pass condition: ≥5 of 7 surfaced.

### Insight 1: HN is correct audience class for this product

**What we expect:** The skill recognizes that HN's audience (backend engineers, infra-builders, developers) overlaps heavily with this product's ICP. Does NOT apply the tldrof "HN is wrong audience class" pattern. Treats HN as a high-leverage primary channel.

**Why this matters:** Catches over-generalization of the HN-category-error pattern. HN works for dev tools.

**Acceptable variations:**
- Explicit "HN reaches the right audience for this product class"
- High leverage score for HN
- At minimum: doesn't apply consumer-product HN-skepticism

### Insight 2: Time-to-Hello-World as the magic moment

**What we expect:** The skill identifies that for dev tools, the load-bearing magic moment is "developer can get the SDK working in their app in under N minutes." Not "see a digest in 60 seconds." Implication: the entire onboarding, docs, getting-started flow IS marketing. Slow setup = lost conversion regardless of channel quality.

**Why this matters:** Dev-tool specific magic moment. Skill must recognize the analog of consumer-product backlog-clearing exists in dev tools but is shaped differently.

**Acceptable variations:**
- Explicit time-to-first-success metric proposed
- "Quickstart" / "5-minute setup" framing in launch playbook
- At minimum: docs / onboarding quality flagged as core marketing surface, not separate concern

### Insight 3: Open-source / hosted-tier conversion mechanic

**What we expect:** The skill surfaces the freemium-to-paid mechanic explicitly: most OSS users never convert; what triggers conversion? Production deploys at scale, multi-region requirements, SLA needs, team-account features, support. Implication: the hosted tier needs specific features OSS lacks AND the SDK needs to make this distinction obvious.

**Why this matters:** Consumer freemium and B2B free-trial dynamics don't apply directly. OSS+paid has its own conversion mechanics.

**Acceptable variations:**
- Direct analysis of "what makes someone upgrade from OSS to hosted"
- Specific paid-tier features that justify $99/mo over self-hosted
- At minimum: flags that OSS adoption ≠ paid conversion, requires separate strategy

### Insight 4: Content / docs as marketing channel

**What we expect:** The skill identifies that for dev tools, docs + integration tutorials + technical blog posts are the dominant marketing surface. SEO compounds. "How to add auth to a Next.js app with AuthForge" tutorials become long-tail discovery. This is different from launch-day-Show-HN marketing.

**Why this matters:** Dev tools win on content compounding. Skill should center this in the channel strategy.

**Acceptable variations:**
- Content / docs SEO surfaced as primary long-term channel
- Specific tutorial / integration patterns proposed
- At minimum: doesn't treat docs as separate from marketing

### Insight 5: GitHub as social-proof and discovery surface

**What we expect:** The skill surfaces that GitHub stars, repo activity (commits, issues, PRs), and ecosystem (who uses this in production?) are real signal for developer adoption. Stars >5K materially affects conversion. Implication: ecosystem-building (getting visible adopters, integrations, community PRs) is its own marketing motion.

**Why this matters:** GitHub matters in dev-tool marketing in ways it doesn't matter in consumer or B2B SaaS. Skill should know.

**Acceptable variations:**
- GitHub stars / repo activity surfaced as KPIs
- Ecosystem-building strategy proposed (named integrations, community PRs encouraged)
- At minimum: GitHub recognized as more than just a code host — as a marketing surface

### Insight 6: Anti-marketing — developer skepticism of overt sales

**What we expect:** The skill flags that overt marketing language ("revolutionary," "best-in-class," "enterprise-grade") hurts dev-tool conversion. Developers prefer technical specifics, benchmarks, honest comparisons. Implication: launch messaging needs to feel like "engineer wrote it for engineers," not "marketer wrote it." Tonal shift from B2B and consumer.

**Why this matters:** Dev-tool-specific failure mode. Skill should recognize the tonal constraint.

**Acceptable variations:**
- Explicit "avoid marketing-speak, lean technical" tonal recommendation
- Benchmark / comparison data proposed as marketing artifacts
- At minimum: flags that dev-tool launch posts should be technically specific, not sales-shaped

### Insight 7: Founder's existing dev-Twitter audience as the actual primary channel

**What we expect:** Given the founder has 3K Twitter followers + 20K-monthly-readers blog, the skill identifies this as a STRONG existing audience that's well-matched to the ICP. Launch should leverage this directly — not as background context but as a primary channel. Different from tldrof's case where the founder had effectively zero relevant reach.

**Why this matters:** The skill should adapt to the founder's actual situation. Strong existing audience changes the strategy.

**Acceptable variations:**
- Founder's audience flagged as primary launch channel
- Pre-launch content cadence to existing audience prioritized
- At minimum: doesn't treat founder as audience-less when they aren't

## Pass criteria

- **PASS:** ≥5 of 7 surfaced
- **STRONG PASS:** 7/7 with strong dev-tool-specific depth
- **FAIL:** ≤4 of 7 — investigate which skill change degraded dev-tool coverage

## Failure modes this fixture catches

- Skill applies tldrof's consumer-subscription HN-skepticism to dev tools
- Skill applies B2B's procurement / case study framing to dev tools
- Skill misses content / docs / SEO as marketing surfaces
- Skill ignores GitHub social-proof dynamics
- Skill recommends marketing-speak language inappropriate for developer audience
- Skill ignores the founder's actual existing relevant audience

## Notes for adding more dev-tool variants

This fixture covers OSS+hosted-tier dev tool. Consider variants for:

- **Pure-OSS dev tool** (no paid tier; alternative revenue / monetization questions)
- **Closed-source paid dev tool** (no OSS; different developer skepticism)
- **Infrastructure / API product** (not SDK — different integration dynamics)
- **Dev tool for non-engineers** (e.g., data analyst tools — different audience class)

Each has its own expected-insights rubric.
