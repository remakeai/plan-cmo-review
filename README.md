# plan-cmo-review

A Claude Code skill for **pre-launch marketing and distribution review** — CMO-shaped, paralleling GStack's executive-role naming (CEO / Eng / Design / CMO). Fits alongside [GStack](https://github.com/garrytan/gstack)'s planning pipeline (`/office-hours` → `/plan-ceo-review` → `/plan-eng-review` → `/plan-design-review` → `/plan-cmo-review`).

Catches the build-it-and-they-will-come trap before it kills 3-6 months of work.

## Why this exists

I'm a solo founder building [tldrof.com](https://github.com/remakeai/tldr-of-tldrs) using GStack. Three full review cycles (CEO, eng, design) caught real bugs and architectural gaps. None of them flagged this:

> "Distribution Plan: Show HN."

That was my entire marketing strategy. A single post. To Hacker News. With no prior audience. From a domain registered six days before launch.

GStack is strong on product judgment, architecture, security, design — and silent on distribution. This skill fills that gap.

## Default founder assumption

This skill assumes the typical user is **technically strong but marketing-naive** — they ship product reliably but have never sold one. Under this default:

- The **product description** is accepted on faith (with room for tweaks).
- Every **marketing premise** — pricing, ICP, channels, launch platform, dogfood mix, in-scope features — is treated as SUSPECT and gets premise-audited before tactical optimization.

The default flips only when the founder provides evidence to the contrary (prior shipped product with paying traction, demonstrated marketing track record, large + ICP-aligned existing audience, documented prior launch retrospectives). Without that evidence, the skill challenges marketing premises by default.

## What it does

Interactive marketing-and-distribution review modeled on GStack's office-hours pattern, **with a premise-audit pass added in v0.2 after v0.1 failed its own regression test**:

- **Step 0.5 Premise Audit (5 questions, NEW in v0.2)** — runs BEFORE tactical questions; attacks the marketing premises the design doc accepts as given:
  - **M0a Launch-platform audience-class fit** — catches "Show HN" for products whose buyers aren't on HN
  - **M0b Canonical-success comparable** — forces research into the proven playbook at this motion class (Superhuman / Readwise / Linear / Stripe / etc.), not just direct competitors
  - **M0c Anti-feature surface** — catches features in scope that contradict positioning
  - **M0d Freebie-disqualifier** — catches acquisition mechanics that select for the WRONG segment (time-rich / money-poor users when the paying ICP is time-poor / money-rich)
  - **M0e Dogfood vs paying-ICP audience-class match** — catches products tuned on the founder's audience when the buyer is a different audience
- **7 tactical forcing questions** (Step 0A) — hard to dodge, refuse evasions. Surface audience reality, channel honesty, first-10-customer specifics. Inherit findings from Step 0.5.
- **Real competitive web search** — not vibes; actual research into where competitors get users PLUS canonical-success comparables at this motion class.
- **Channel-by-channel evaluation** — refuse "we'll do all of them"; force 2-3 channel prioritization.
- **Pre-launch audience-build plan** — 30/60/90-day cadence starting now, not at launch.
- **Launch playbook with gate-question (NEW in v0.2)** — questions whether the launch gate should be calendar-driven or PMF-signal-driven (Vohra "very disappointed" / Superhuman concierge-first) BEFORE producing the sequence.
- **Pricing review with band-question (NEW in v0.2)** — questions the pricing BAND before optimizing the price point. Catches the "match cheapest competitor" technical-founder reflex.
- **Outside-voice critique** — independent cold-read of the marketing plan.
- **Artifacts:** `marketing_plan.md`, `icp.md`, `launch_playbook.md`, `audience_build_journal.md` (or `audience_build_sprint.md` in Mode C).

Three modes: Full Review (90-120 min), Focused Review (40-60 min), Audience-Build Sprint (60 min — for founders with zero existing audience).

## What it refuses to accept

The failure patterns most marketing plans fall into:

- "Build it and they will come"
- "Show HN as the entire distribution strategy"
- "I'll start marketing after launch"
- "My competitors don't really compete with me"
- "I don't need a marketing plan because the product is so good"
- "Indie hackers" as a target audience (without specificity)
- "I'll do all the channels" (without prioritization)
- **NEW in v0.2:** "Match the cheapest competitor's price" — common technical-founder reflex; almost always wrong for time-poor/money-rich ICPs
- **NEW in v0.2:** "Calendar-driven launch is fine" — for retention-driven products, the launch gate should be PMF-signal-driven
- **NEW in v0.2:** "Cheap-trial mechanics validate willingness-to-pay" — they validate willingness to try for free; different segment
- **NEW in v0.2:** "All our in-scope features serve the paying ICP" — almost always wrong; look line-by-line
- **NEW in v0.2:** "Direct competitors are the only comparables that matter" — canonical-success comparables (Superhuman, Readwise, etc.) are the precedents; direct competitors are just the alternatives
- **NEW in v0.3:** "Marketing-speak language in dev-tool launches" — for dev-tool products, superlatives ("revolutionary", "best-in-class", "enterprise-grade") inversely correlate with launch traction. Lead with technical specifics, honest comparisons including where you lose, and code-first links.
- **NEW in v0.3:** "Defer the paying ICP and keep the dogfood-aligned audience" — when M0e flags a dogfood/buyer mismatch, the wrong fix is to defer the paying ICP "to v1.0.5" while keeping the dogfood-aligned audience. Both pivots are required: target audience AND dogfood subjects.

If you lean into these, the skill surfaces it and requires a concrete alternative before continuing.

**Default refusal posture under marketing-naive default:** when in doubt between accepting and challenging a founder's marketing claim, CHALLENGE. A wrongly-accepted premise produces a polished plan that ships to silence; a wrongly-challenged premise costs 10 minutes to re-defend. Cost asymmetry favors challenge.

## Installation

### Option 1: Drop into Claude Code globally

```bash
mkdir -p ~/.claude/skills/plan-cmo-review
cp SKILL.md ~/.claude/skills/plan-cmo-review/
```

Then invoke from Claude Code with `/plan-cmo-review`.

### Option 2: Per-project

```bash
mkdir -p ./.claude/skills/plan-cmo-review
cp SKILL.md ./.claude/skills/plan-cmo-review/
```

### Option 3: Integration with GStack

If you have GStack installed at `~/.claude/skills/gstack/`, place this skill alongside as a sibling:

```bash
mkdir -p ~/.claude/skills/plan-cmo-review
cp SKILL.md ~/.claude/skills/plan-cmo-review/
```

The skills compose naturally — invoke this one after `/plan-ceo-review` and before `/ship`.

## Quick start

```
You: I'm about to start marketing my SaaS. Help me think it through.
Claude: [invokes /plan-cmo-review]
```

Or explicitly:

```
You: /plan-cmo-review
```

The skill will:

1. Audit existing artifacts (design doc, repo, etc.)
2. Run a competitive web search
3. Audit your existing audience surface area
4. Ask 7 forcing questions (one at a time, ~15-25 min)
5. Recommend a mode (Full / Focused / Audience-Build Sprint)
6. Walk through the chosen mode's sections
7. Run outside-voice critique
8. Write output artifacts to your repo

Total time: 40-120 min depending on mode.

## When NOT to use this skill

- Post-launch growth optimization (different inputs; different skill)
- B2B enterprise account-based sales (long-cycle ABM; different motion)
- Acquisition / M&A strategy (out of scope)

For those, use other tools or skills.

## What it doesn't do (limitations)

- It doesn't run paid ads for you or execute outreach
- It doesn't guarantee distribution success (no tool can)
- It doesn't replace founder judgment on positioning or voice
- Same gameability caveat as any AI evaluator — a founder who iterates with Claude to game the forcing questions can produce a polished plan that masks weak fundamentals. Use the outputs as a draft to react to, not as truth.

## Regression tests

**This skill ships with regression tests.** Unusual for AI skills; necessary because AI evaluators don't crash when they degrade — they confidently produce subtly weaker output. Without fixture-based regressions, model upgrades and prompt edits can silently weaken what the skill catches; nobody notices until the next user gets a bad plan.

Test fixtures live in [`tests/regressions/`](tests/regressions/). Each fixture is:

- **A frozen input scenario** (real or synthetic product description)
- **An expected-insights rubric** — 7 specific insights the skill SHOULD surface against that input
- **Pass criteria** — typically ≥5 of 7 insights at acceptable depth

### Current fixtures

| Fixture | Motion class | Why it exists |
|---|---|---|
| [`tldrof-expected-insights.md`](tests/regressions/tldrof-expected-insights.md) | Consumer subscription ($9/mo) | Real founder case (tldrof.com). Baseline derived from a parallel `/deep-research` session that produced a meaningfully better plan than the skill's first version. |
| [`b2b-saas-expected-insights.md`](tests/regressions/b2b-saas-expected-insights.md) | B2B SaaS ($40/seat/mo, mid-market) | Synthetic fixture catches over-application of consumer-product patterns (HN-as-category-error, freebie-disqualifier) to B2B contexts where they don't apply. |
| [`dev-tool-expected-insights.md`](tests/regressions/dev-tool-expected-insights.md) | OSS + hosted-tier dev tool ($99/mo) | Synthetic fixture catches over-application of consumer OR B2B patterns to dev tools. HN IS right audience for dev tools; docs/SEO compounding matters; OSS-to-paid mechanics are distinct. |

### How to run the regression tests

**Manual run** (recommended for v0.x — fast, low ceremony):

1. Open the fixture file (e.g., `tests/regressions/tldrof-expected-insights.md`) and read the input scenario + expected insights
2. Run `/plan-cmo-review` in a clean Claude Code session against the input scenario
   - For the tldrof fixture: check out `tldr-of-tldrs/design_document.md` at the snapshot revision noted in the fixture, then run the skill against it
   - For synthetic fixtures: paste the "Synthetic input scenario" section as the design-doc context and run the skill
3. Read the resulting `marketing_plan.md` (and `launch_playbook.md` if produced)
4. For each of the 7 expected insights, mark **surfaced (deep / moderate / minimum) / not surfaced** per the fixture's "Acceptable variations" guidance
5. Compute pass/fail per the fixture's pass criteria
6. Append the result to `tests/regressions/results.jsonl`:
   ```json
   {"date": "YYYY-MM-DD", "fixture": "tldrof", "skill_version": "v0.x.x", "model": "claude-X-X-X", "score": "N/7", "verdict": "PASS|WEAK|FAIL|STRONG", "missed": ["insight 3", "insight 6"]}
   ```

**LLM-judged run** (recommended for v0.5+ — automatable):

1. Run the skill against the fixture's input scenario as in step 2 above
2. Pass the resulting marketing plan output + the fixture file (rubric) to a Claude subagent with prompt:
   > You are scoring a marketing plan against a rubric of 7 expected insights. For each insight, the rubric specifies "acceptable variations." Read the plan, then for each insight return `{ "surfaced": bool, "depth": "deep"|"moderate"|"minimum"|"absent", "evidence_excerpt": "the relevant quote from the plan", "notes": "your reasoning" }`. Be strict on rubric matching but allow the variations explicitly listed.
3. Aggregate the 7 results into a pass/fail per the fixture's pass criteria
4. Append to `results.jsonl` as above

**CI integration** (for v1.0+): trigger regression run on every `SKILL.md` change; compare against last-known-good baseline; block merge if a fixture drops below previous pass level.

#### Methodology notes

**Real web search is required, not optional.** The skill's competitive analysis depends on current (post-training-cutoff) data — competitor pricing changes, dead products, new entrants. Runner subagents that simulate web searches from training-data knowledge instead of invoking the WebSearch tool live should be flagged in the `notes` field of the `results.jsonl` entry as a methodology gap. A run that self-reports simulated web search does not count as a clean pass; re-run with mandatory live WebSearch invocation before treating the score as authoritative.

**Reliability requires multiple runs per fixture.** A single passing run doesn't distinguish skill quality from a lucky draw. For meaningful reliability claims (model upgrades, major prompt edits, before-vs-after comparisons), run each fixture ≥3 times with blind runners + independent judges. Look at the variance, not just the headline pass rate — same input + same skill should produce consistent insight coverage, mode selection, and prescription direction across runs. Cross-run variance (different mode selection, directionally inverted prescriptions, consistently shallow depth on the same insights) is a skill gap, not noise.

### When to run regressions

- **Every skill version bump** (`SKILL.md` edits)
- **Every model upgrade in production** (Claude version change in your Claude Code setup)
- **Every major prompt-template edit**
- **Quarterly** as a baseline drift check, even without intentional changes

### Adding more fixtures

PRs welcome for fixtures covering motion classes not yet represented:

- Marketplace (two-sided cold-start dynamics)
- Enterprise SaaS (>1000 seats, RFP-driven, security-questionnaire-heavy)
- Vertical SaaS (industry-specific channel/community landscape)
- AI agent product (trust-led, capability-curve-aware)
- Hardware-adjacent SaaS (long sales cycles, integration partnerships)
- Pure-OSS dev tool (no paid tier; alternative monetization)
- Mobile consumer app (App Store dynamics, ASO)

Each motion class has distinct failure modes that a one-fixture-fits-all skill will miss. Each new fixture catches a class of skill regression the existing fixtures don't.

To add a fixture:

1. Copy the structure of an existing fixture (`tldrof-expected-insights.md` is the reference)
2. Define a frozen input scenario (real OR synthetic — both are valid)
3. Derive 7 expected insights from EITHER a known-good parallel session OR domain expertise about the motion class
4. Specify acceptable variations per insight (must be strict enough to catch regressions, lenient enough to allow legitimate variation)
5. Set pass criteria (default ≥5/7)
6. Open a PR

### Why this matters beyond plan-cmo-review

If you're building any AI evaluator skill — code reviewer, document grader, plan critic, founder-idea scorer — **ship regression tests with it**. Same principle as code. Skills that confidently produce subtly-degrading output are more dangerous than software that crashes, because users have no clear signal that something has degraded.

This applies to GStack and to most AI planning tools currently in circulation. The convention should be widespread; it isn't yet.

## Contributing

Issues, PRs, and forks welcome. Marketing skill design has weak feedback loops — honest reports from founders who used it (and especially those who shipped after using it) are the most valuable input.

If you use this skill and find a question that should have been asked but wasn't — open an issue. If you find a category of marketing failure the skill doesn't catch — open an issue or PR. If you have a frozen input + expected-insights rubric for a motion class not yet covered, contribute a regression fixture.

## License

Apache 2.0. Use freely. Attribution appreciated but not required.

## Acknowledgments

Built to fill the marketing gap I found in [GStack](https://github.com/garrytan/gstack) (Garry Tan's open-source startup planning skill package). GStack is excellent at what it does; this skill is meant to complement, not replace.

## Author

Dr. Ilia Ovsiannikov — find me on [LinkedIn](https://www.linkedin.com/in/iliao/). Subscribe to startup founder notes [iliaov.substack.com](https://iliaov.substack.com).
