# AuthForge ICP Specification

**Source:** Step 0A M1 (forcing question) + Step 0.5 M0e (dogfood-vs-buyer pivot)

## Primary persona — Daniel (tech lead, small B2B SaaS)

| Attribute | Value |
|---|---|
| Name (composite) | Daniel |
| Role | Tech lead / Senior backend engineer |
| Team size | 4 engineers (within 12-person YC seed company) |
| Stack | TypeScript, Next.js, Postgres, Vercel, Linear, Sentry |
| Stage | Seed-stage YC company, ~$1-3M raised, ~12 months runway |
| Age | 28-34 |
| Geo | US (SF/NYC majority), Europe secondary |
| Buying authority | Decides on dev infra up to $200/mo without approval; team agreement needed above |
| Time-to-decision | 2-6 weeks from first exposure to first paid charge |

## Attention surfaces (where Daniel currently spends time)

1. **Pragmatic Engineer** (Gergely Orosz) — weekly newsletter, paid subscriber
2. **Dev-Twitter:** @t3dotgg (Theo Browne), @leerob (Lee Robinson, Vercel), @shadcn, @dan_abramov, @rauchg, @bekacru (Better Auth founder — direct competitor signal)
3. **Next.js Discord** — actively reads #help and #showcase
4. **Syntax FM podcast** — weekly listener
5. **Software Engineering Daily** — episodic listener
6. **r/nextjs, r/typescript** — passive reader, lurker not poster
7. **GitHub Trending (TypeScript)** — weekly check
8. **Lenny's Newsletter** — occasional reader for PM-adjacent content
9. **Hacker News** — daily scroll, occasional comment

## What Daniel currently pays for (adjacent SaaS)

| Tool | Price | Why he pays |
|---|---|---|
| Cursor | $20/mo personal | AI coding assist |
| Linear | $8/seat company | Project tracking — clean UI, fast |
| Sentry | $26+/mo company | Error tracking, predictable pricing |
| Vercel | $20/seat company | Hosting, deploy DX |
| Clerk | Free (10K MAU), $25/mo Pro looming | Current auth — but pricing scales painfully |
| GitHub Copilot | $19/seat company | Code completion |
| Datadog (occasional) | $$$ | Logs — but evaluating cheaper alts |

**Pattern:** Daniel pays for tools that are (a) priced predictably, (b) have excellent DX, (c) save him operational time. He does NOT pay for tools that require ops investment or have unpredictable cost spikes.

## What Daniel complains about in adjacent categories

- **Clerk:** "Pricing breaks past 10K MAU. $0.02/MAU is fine until I have a viral moment and suddenly owe $400."
- **Auth0:** "Enterprise vibes. Heavy. Pricing opaque. Migration off would be a nightmare."
- **Supabase Auth:** "Forces me onto Supabase for the whole stack. I want Postgres-on-Neon AND best-in-class auth, not a bundled compromise."
- **Better Auth:** "Free, OSS, growing fast. But I'd have to maintain it myself when something goes sideways at 3am. No hosted option."
- **Cognito:** "Documentation is from another century. Console UX is a punishment."

## Objections Daniel will raise to AuthForge

1. **"Why not just Better Auth?"** — Most important objection. Founder must have a one-liner answer that survives skeptical inspection. If the answer is "we have a hosted tier," Daniel asks: "What stops Better Auth from launching one in 90 days?"
2. **"Who's maintaining this in 5 years?"** — First-time-shipper risk; needs ex-Stripe credential + transparent commitment.
3. **"Can I migrate off cleanly?"** — Lock-in fear; AuthForge should ship a documented `users` table export from day 1.
4. **"What's my SSO/SCIM story?"** — If gated behind expensive enterprise tier, Daniel skips.
5. **"Have you hit production scale?"** — Will ask for a named adopter or load test results.
6. **"What about compliance (SOC 2, GDPR)?"** — Often delegated to security review, but he wants to know AuthForge has a roadmap.

## Reasons Daniel will convert (in priority order)

1. **Pricing predictability past 10K MAU.** If AuthForge offers flat $49 Team / $199 Business with NO per-MAU surprise, Daniel migrates from Clerk.
2. **Ex-Stripe credential.** Daniel trusts that the founder knows what production-grade auth looks like.
3. **Honest "worse at X" positioning.** Daniel reads transparency as a trust signal.
4. **5-minute quickstart on Next.js.** If `npm i authforge && AuthForgeProvider` works in 5 minutes, he's hooked.
5. **Self-host AND hosted both viable.** Daniel evaluates self-host for the future; uses hosted for now. The optionality matters.
6. **Public roadmap with SSO/SCIM dates.** Even if not shipped yet, knowing it's coming Q3 lets Daniel plan.

## Secondary persona (B2B-enterprise, defer to v1.0.5)

- "Sarah" — Director of Platform Engineering at a 200-person FinTech. Needs SOC 2 attestation, SCIM, SSO, audit log, self-hosted-with-support contract. Pays $2K-$20K/mo. NOT v1 ICP — feature surface not ready. Note for roadmap.

## Anti-ICP (do NOT optimize for)

- Solo OSS hobbyists (won't pay for hosted)
- Enterprise infosec teams (Auth0 / Okta won that battle)
- Crypto/Web3-native auth (different problem class entirely)
- Mobile-first consumer apps (SSO with Apple/Google dominates that space)

## Customer-development plan (this week)

Founder must talk to 5 Daniels before pricing or wedge is locked. Specific questions:

1. "What would make you migrate off Clerk?"
2. "If I priced at $49/mo flat for up to 25K MAU, how does that compare to what you'd expect to pay?"
3. "Walk me through what you'd evaluate in a new auth SDK in your first 30 minutes."
4. "What's your one-liner reason to NOT pick Better Auth?"
5. "What would scare you about adopting a 6-month-old auth library?"

Record all 5. If responses cluster on a wedge (compliance, pricing predictability, ops quality, AI-agents), that's the wedge.
