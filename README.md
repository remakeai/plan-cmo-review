# plan-cmo-review

A Claude Code skill for **pre-launch marketing and distribution review** — CMO-shaped, paralleling GStack's executive-role naming (CEO / Eng / Design / CMO). Fits alongside [GStack](https://github.com/garrytan/gstack)'s planning pipeline (`/office-hours` → `/plan-ceo-review` → `/plan-eng-review` → `/plan-design-review` → `/plan-cmo-review`).

Catches the build-it-and-they-will-come trap before it kills 3-6 months of work.

## Why this exists

I'm a solo founder building [tldrof.com](https://github.com/remakeai/tldr-of-tldrs) using GStack. Three full review cycles (CEO, eng, design) caught real bugs and architectural gaps. None of them flagged this:

> "Distribution Plan: Show HN."

That was my entire marketing strategy. A single post. To Hacker News. With no prior audience. From a domain registered six days before launch.

GStack is strong on product judgment, architecture, security, design — and silent on distribution. This skill fills that gap.

## What it does

Interactive marketing-and-distribution review modeled on GStack's office-hours pattern:

- **7 forcing questions** — hard to dodge, refuse evasions. Surface audience reality, channel honesty, first-10-customer specifics.
- **Real competitive web search** — not vibes; actual research into where competitors get users.
- **Channel-by-channel evaluation** — refuse "we'll do all of them"; force 2-3 channel prioritization.
- **Pre-launch audience-build plan** — 30/60/90-day cadence starting now, not at launch.
- **Multi-channel sequenced launch playbook** — refuses single-channel "Show HN" plans.
- **Outside-voice critique** — independent cold-read of the marketing plan.
- **Artifacts:** `marketing_plan.md`, `icp.md`, `launch_playbook.md`, `audience_build_journal.md`.

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

If you lean into these, the skill surfaces it and requires a concrete alternative before continuing.

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

## Contributing

Issues, PRs, and forks welcome. Marketing skill design has weak feedback loops — honest reports from founders who used it (and especially those who shipped after using it) are the most valuable input.

If you use this skill and find a question that should have been asked but wasn't — open an issue. If you find a category of marketing failure the skill doesn't catch — open an issue or PR.

## License

MIT. Use freely. Attribution appreciated but not required.

## Acknowledgments

Built to fill the marketing gap I found in [GStack](https://github.com/garrytan/gstack) (Garry Tan's open-source startup planning skill package). GStack is excellent at what it does; this skill is meant to complement, not replace.

## Author

Ilia Ovsiannikov — building [tldrof.com](https://github.com/remakeai/tldr-of-tldrs) in public. Daily journal at [iliaov.substack.com](https://iliaov.substack.com).
