# Regression test fixture — tldrof / plan-cmo-review

**Skill under test:** `plan-cmo-review`
**Input fixture:** `tldr-of-tldrs/design_document.md` at the revision frozen for this test (see "Input snapshot" below).
**Expected output:** marketing plan that surfaces ≥5 of 7 insights documented below.
**Reference output:** `tldr-of-tldrs/MARKETING.md` produced via a parallel `/deep-research` conversation, which surfaced all 7. This file is the rubric extracted from it.

## Why this fixture exists

`plan-cmo-review` v0.1 (initial release) was run against tldrof's design_document.md and produced `marketing/marketing_plan.md` + `marketing/launch_playbook.md`. A separate session using `/deep-research` produced `MARKETING.md` — measurably stronger output because it questioned premises that `plan-cmo-review` accepted as given.

This fixture exists so future versions of the skill can be regression-tested: given the same input, does the new version produce comparable insight coverage to the deep-research baseline?

Without this fixture, model upgrades, prompt edits, or section reorderings can silently weaken the skill — and nobody would notice until the next user produces a bad plan.

## Input snapshot

- File: `tldr-of-tldrs/design_document.md`
- Frozen at: state as of 2026-05-23 (after Founder Editorial Pass 5; before any Day 5+ corrective queue items shipped)
- File: `tldr-of-tldrs/IMPLEMENTATION.md` (companion context)
- Founder profile data: ex-Micron, building tldrof.com, LinkedIn 996 followers, Substack 11 subscribers, dogfood on technical newsletters

If the input snapshot drifts, the expected insights MAY drift too. Re-derive the rubric if the input changes meaningfully.

## Expected insights (7 items)

The skill output is judged against these 7 insights. Pass condition: **≥5 of 7 surfaced**. Below 5 = regression.

### Insight 1: HN as launch-platform CATEGORY ERROR

**What we expect:** The skill flags Hacker News as the wrong audience class for tldrof (a consumer-habit product), not just a risky single channel. Specifically: HN's technical/DIY-by-instinct audience produces both false-negative (DIY crowd shrugs at viable product) AND false-positive (builders upvote and churn) signals. HN should not be the pass/fail gate.

**Why this matters:** The original design doc treated Show HN as the entire launch plan AND as the validation gate (P6). Both treatments are wrong. plan-cmo-review v0.1 accepted HN as a launch channel and added other channels around it — useful but didn't catch the deeper "wrong audience class" framing.

**Acceptable variations:**
- Explicit "HN is wrong audience class for this product" language
- Implicit treatment: relegates HN to one channel among 3+, removes HN as the validation gate, and flags audience-platform-fit as a separate question from channel-viability

### Insight 2: Freebie-disqualifier (time-rich vs money-rich ICP selection bias)

**What we expect:** The skill surfaces that low-commitment trial mechanics (free trial, $1 reservations, "try it for a month") select for time-rich/money-poor users — the OPPOSITE of the time-poor/money-rich paying ICP. Implication: the validation cohort and the paying cohort are different humans; cheap-trial validation produces misleading signal.

**Why this matters:** This is the load-bearing frame that made the founder realize the entire acquisition strategy was selecting against the actual buyer. Without this insight, the marketing plan optimizes for wrong-segment acquisition.

**Acceptable variations:**
- Explicit "freebie-disqualifier" naming
- Implicit treatment via: recommending high-trust acquisition (referral, comparable-recommendation, concierge) for time-poor segments + explicit warning about trial-mechanic selection bias

### Insight 3: Canonical-success comparables (Superhuman / Readwise / Mailbrew / Artifact)

**What we expect:** The skill pulls in named comparables from outside the founder's stated comp set:
- **Superhuman** — $30/mo, won via concierge + WOM + scarcity ($825M acquisition Jul 2025)
- **Readwise** — ~$10/mo, ~$14M ARR, >90% retention, niche-indispensable + product-led + partnerships
- **Mailbrew / Artifact** — failed; the free-aggregator pattern doesn't sustain
- **Meco** — alive on free + partner-program ($4/referral); closest live analog

Each comparable should include a brief playbook note and a specific lesson for tldrof.

**Why this matters:** Real comparables anchor the analysis against precedent. plan-cmo-review v0.1 named direct competitors (Readless, Meco, Refind) but didn't pull in the canonical successes that prove the playbook works at this motion class.

**Acceptable variations:**
- All 4 comparables named with playbook notes — best
- 2-3 of 4 with playbook notes — pass
- Only direct-competitor named without playbook depth — fail

### Insight 4: Pricing reconsideration ($9 may be wrong band, not just wrong price)

**What we expect:** The skill questions the $9 pricing band itself, not just the specific number. Specifically: surfaces evidence that $5-9 is a documented LTV-penalty band; that time-poor/money-rich ICPs tolerate $9-15+; that Readwise (~$10, >90% retention) and Superhuman ($30) prove the higher band works for the motion class.

**Why this matters:** Pricing is the single biggest unit-economics lever and was treated as locked from CEO review forward. Without re-opening, every downstream marketing decision (CAC tolerance, channel choice, trial mechanic) inherits a suboptimal anchor.

**Acceptable variations:**
- Direct "$9 is the wrong band" claim with evidence
- "Consider raising to $9-15 / annual pricing" with evidence
- At minimum: explicitly flags pricing as worth re-opening with CEO review, not silently accepted

### Insight 5: Dogfood audience-class mismatch (technical → non-technical pivot)

**What we expect:** The skill flags that the technical-newsletter dogfood (TLDR, AlphaSignal, etc.) tunes the product to a technical audience, while the paying ICP is non-technical (Morning Brew / 1440 / Skimm readers — high newsletter volume, low DIY-threat, willing to pay). Surfaces that the audience mismatch ALSO matches feature value: technical newsletters are differentiated (low overlap → little dedup value); general news newsletters massively overlap (high dedup value where it matters).

**Why this matters:** The product is being calibrated to the wrong audience. Without this insight, the marketing plan targets the technical audience the product was tuned for instead of the non-technical audience the product would actually serve well.

**Acceptable variations:**
- Direct "pivot dogfood and target audience to non-technical news-rich" recommendation
- "Add non-technical newsletter fixtures to dedup tuning" + audience pivot in marketing
- At minimum: flags the dogfood/buyer mismatch as a strategic issue, not just a marketing tweak

### Insight 6: Anti-feature identification (BYO-Claude / MCP)

**What we expect:** The skill identifies at least one feature currently in scope that contradicts positioning. The canonical case for tldrof: any BYO-Claude / MCP integration that lets users connect their own LLM is an offramp for the exact technical segment that won't pay anyway — courts wrong-ICP, breaks push-model (MCP is pull/interactive), optimizes the wrong cost.

**Why this matters:** Anti-features are a category of strategic risk that tactical planning skills don't surface. Without anti-feature awareness, plans accept features that quietly undermine the wedge.

**Acceptable variations:**
- Specifically names BYO-Claude / MCP as the anti-feature
- Identifies a different in-scope feature that contradicts positioning with similar reasoning quality
- At minimum: introduces "anti-feature" as a concept and asks the founder to identify ≥1

### Insight 7: PMF-gated launch (Vohra "very disappointed" test or equivalent)

**What we expect:** The skill reframes the launch gate from calendar-driven (P6: 15 paying by day 14, P5: 25 paying by day 30) to PMF-signal-driven. Specifically: introduces or references a real PMF gate (Vohra "how would you feel if you could no longer use this — >40% very disappointed" or equivalent) AND recommends concierge-onboarding the first cohort (manually, with founder doing the onboarding) before widening rollout.

**Why this matters:** Calendar-driven launch gates fire whether or not the product is actually indispensable. PMF-gated launches force the product to be indispensable before scaling. The Superhuman comparable (Vohra personally onboarded the first 200 users) is direct precedent.

**Acceptable variations:**
- Explicit Vohra "very disappointed" reference
- Implicit treatment: concierge-onboard first cohort + measure dependence-signal before scaling + delay public launch until signal clears
- At minimum: surfaces that calendar gates are wrong for retention-driven products and recommends a real dependence metric

## Pass criteria

- **PASS:** ≥5 of 7 insights surfaced with reasonable depth (per acceptable variations)
- **WEAK PASS:** 5/7 surfaced but at minimum-acceptable variation level — acceptable but flag as "barely passing; insight depth declining"
- **FAIL:** ≤4 of 7 surfaced — regression caught; investigate which skill change degraded coverage
- **STRONG PASS:** 7/7 surfaced with depth — actively improved over reference

Pass condition is intentionally set at 5/7 not 7/7. Some insight variation is expected from model differences and prompt drift; the regression test catches genuine degradation, not minor variation.

## How to run this regression test

### Manual run (recommended for v0.x — fast, low ceremony)

1. Check out the input snapshot revision of `tldr-of-tldrs/design_document.md`
2. Run `/plan-cmo-review` against that input in a clean Claude Code session (no prior context that would leak from this rubric file)
3. Open the resulting `marketing/marketing_plan.md` and `marketing/launch_playbook.md`
4. For each of the 7 insights above, check the skill output and mark: **surfaced (depth: deep / moderate / minimum) / not surfaced**
5. Compute pass/fail per criteria above
6. Append result to `tests/regressions/results.jsonl` as one line:
   ```json
   {"date": "YYYY-MM-DD", "skill_version": "v0.x.x", "model": "claude-X-X-X", "score": "N/7", "verdict": "PASS/WEAK/FAIL/STRONG", "missed": ["insight N", "insight M"]}
   ```

### LLM-judged run (recommended for v0.5+ — automated)

1. Run the skill as above to produce the output
2. Pass the output + this rubric file to a Claude subagent with prompt:
   > You are scoring a marketing plan against a rubric of 7 expected insights. For each insight, the rubric specifies "acceptable variations." Read the plan, then for each insight return: { "surfaced": bool, "depth": "deep"|"moderate"|"minimum"|"absent", "evidence_excerpt": "the relevant quote from the plan", "notes": "your reasoning" }. Be strict on rubric matching but allow the variations explicitly listed.
3. Aggregate the 7 results into a single pass/fail per the criteria above
4. Append to `results.jsonl`

### CI integration (for v1.0+)

1. On every change to `plan-cmo-review/SKILL.md`, trigger a regression run
2. Compare against last-known-good baseline result
3. Block merge if regression caught (score drops below previous PASS level)
4. Allow manual override with documented reason (model improvements that change acceptable depth, etc.)

## Cadence

- Run on every skill version bump
- Run on every model upgrade in production (Claude version change)
- Run on every major prompt-template edit
- Re-derive the rubric from a fresh deep-research session every 6 months — comparables may shift (new comparable products, dead competitors, evolving playbooks)

## Why 5/7 not 7/7

Strict 7/7 pass condition creates pressure to over-fit the skill to this exact rubric, which itself is a snapshot of one good deep-research run. 5/7 leaves room for legitimate variation while catching real degradation. Adjust the threshold upward as the skill matures and the rubric stabilizes.

## Adding more fixtures

This is one fixture for one product. The skill needs MORE regression fixtures to be reliable across product types:

- B2B SaaS at higher price point (different motion: ABM-flavored)
- Marketplace (different motion: two-sided cold-start)
- Dev tool (different motion: developer-marketing-led)
- AI agent product (different motion: trust-led + capability-curve-aware)
- Hardware-adjacent SaaS (different motion: long sales cycle + integration partnerships)

Add fixtures as you collect them. Each fixture is a frozen input + an expected-insight rubric derived from a known-good output. The total set of fixtures defines what "the skill works" actually means.
