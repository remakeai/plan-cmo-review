# AuthForge — ICP Specification

**Two ICPs. Do not conflate them.** Conflating these two segments is the M0d failure mode that breaks the design doc's first-10-customers plan. The OSS surface serves both, but messaging, pricing, channels, and conversion mechanics are different.

---

## ICP-A — "Marcus" (paying hosted-tier customer)

### Persona

- **Age / role:** 32 / CTO + co-founder
- **Company:** 4-12 person SaaS startup (YC W26, Techstars, or bootstrapped angel-backed)
- **Stack:** TypeScript + Next.js (or Hono / Bun) + Postgres on Vercel + Supabase / Neon / Railway
- **Auth today:** Supabase Auth (graduating out due to B2B org-switching pain) OR Clerk (graduating out due to React-only constraint as team adds Vue/Svelte) OR rolled-their-own with NextAuth/Auth.js
- **Current pain:** custom claims, B2B multi-tenant, SSO request from first enterprise customer, JWT key rotation in production

### Where they spend attention

1. **Pragmatic Engineer** (subscribes)
2. **HackerNews** (daily check)
3. **Theo Browne (t3.gg) YouTube + Twitter**
4. **@leerob, @rauchg, @t3dotgg** on Twitter
5. **Vercel Discord** (active)
6. **YC Slack / Bookface** (W26 cohort channels)
7. **r/nextjs, r/SaaS** (weekly)
8. **Bun Discord** (if shipping on Bun)
9. **JS Party podcast** + **Syntax** + **Software Engineering Daily**

### Adjacent-category spend

- Cursor — $20/mo
- Linear — $8/seat/mo
- Vercel Pro — $20/mo + usage
- Supabase Pro — $25/mo
- Resend — $20/mo
- Clerk Pro (if currently on it) — $25/mo
- Notion — $10/seat/mo
- Sentry — $26+/mo

**Pattern:** comfortable with $20-30/mo per tool. The $99/mo AuthForge price is 4× above adjacent-category band — requires strong justification.

### Complaints in adjacent categories

- Auth0: "Pricing creeps 5-10× over 3 years."
- Clerk: "React-only UI components are limiting as we add new frontends."
- Supabase Auth: "B2B multi-tenancy is a hack on top of RLS."
- Self-rolled: "JWT key rotation is the worst engineering work I do all year."

### Objections to AuthForge

1. "Why migrate auth? It's the riskiest migration." (auth-migration loss aversion)
2. "Why pay $99 when Clerk is $25?" (price-anchoring vs Clerk)
3. "How is this different from BetterAuth?" (BetterAuth is the YC-blessed alternative — the killer comp)
4. "Will the founder still be around in 2 years?" (single-founder risk)
5. "What happens to my data if AuthForge gets acquired?" (Stytch→Twilio 2025 fresh in mind)

### Reasons to convert

1. Framework-agnostic (Clerk's React-only is now a constraint)
2. Self-host parity with managed (Clerk has no self-host fallback)
3. B2B-first design (Supabase Auth and Clerk both bolt B2B on)
4. Concierge onboarding (founder personally helps integrate — Stripe / Superhuman precedent)
5. Founder credibility (ex-Stripe + 20K-reader tech blog)

---

## ICP-B — "Priya" (OSS-DIY adopter, will NOT pay for hosted)

### Persona

- **Age / role:** 28 / senior backend engineer or staff engineer
- **Company:** 50-200 person fintech, healthtech, or regulated-industry company OR FAANG infrastructure team
- **Stack:** Go or Rust backends; self-hosted Postgres, Redis, observability
- **Auth today:** Keycloak (self-hosted, hates it) OR rolled-their-own OAuth2 OR Ory (Kratos / Hydra)
- **Current pain:** ops cost of Keycloak; can't get OSS-clean auth without "enterprise" gates

### Where they spend attention

1. **lobste.rs** (more than HN)
2. **HackerNews**
3. **r/golang, r/rust, r/selfhosted**
4. **GH issues + discussions** on the libraries they depend on
5. **Mailing lists** of OSS projects (Keycloak users list, etc.)
6. **DEF CON / BSides talks** on identity / OAuth security
7. **The Changelog podcast**

### Adjacent-category spend

- Almost nothing personally. Advocates for OSS internally.
- May approve a $1-3K/year support contract IF the company forces an "enterprise support relationship" checkbox.

### Complaints in adjacent categories

- Auth0: "$15K bills for what I could write in 200 LOC."
- Keycloak: "Java + WildFly + cluster config is 3 weeks of ops to get right."
- Managed services: "What about data residency?", "Phone-home telemetry is a non-starter."

### Objections to AuthForge

1. "Is this open-core with the good stuff locked behind paid?" (open-core skepticism)
2. "What's the license? Will it switch to BSL/SSPL in 2 years?" (HashiCorp/Elastic/Redis-style license-change fear)
3. "Is there phone-home telemetry?" (community-killing if yes)
4. "Who controls the project if the founder gets acquired?" (sustainability)

### Reasons to advocate (not pay)

1. Clean MIT, no CLA-required-for-contributing
2. NO phone-home telemetry
3. Plugin SDK with named contributor recognition (HashiCorp HUG precedent)
4. Self-host runs without forced managed dependencies
5. Honest project README ("here's where we're worse than X")

---

## How the two ICPs interact

**Priya's evaluation produces the signal Marcus reads.** Marcus does not directly evaluate AuthForge against Auth0 / Clerk in isolation — he reads lobste.rs comments, GH issue threads, and "AuthForge vs X" comparisons that Priya's segment produces. **OSS credibility (built by serving Priya) is the gating input to ICP-A revenue.**

This is why the OSS SDK serves Priya and the hosted-tier SAAS serves Marcus, but BOTH must exist for either to work.

---

## Messaging map

| Surface | Audience | Tone | CTA |
|---|---|---|---|
| GitHub README | Priya (and Marcus during eval) | Engineer-to-engineer; honest deltas; technical specifics | Self-host quickstart |
| `docs.authforge.dev` | Both | Stripe-quality reference; framework-by-framework tutorials | Integrate in 10 minutes |
| `/pricing` and `/hosted` landing | Marcus only | Outcome-led ("don't run JWT rotation yourself") | Book concierge call |
| Discord | Both | Founder-present, helpful | Ask questions |
| Show HN copy | Priya primarily (Marcus eavesdrops) | Engineer-tone, technical specifics, honest deltas | GitHub link FIRST |
| Vercel Discord / Bun Discord | Marcus | Helpful, contextual, never pitchy | Tutorial links in helpful answers |
| Newsletter | Both | Build-in-public + tutorial of the week | Subscribe to follow |

---

## Objection-handling rehearsal (founder must prep before launch)

| Objection | Response (rehearsed, technical, honest) |
|---|---|
| "How is this different from BetterAuth?" | "BetterAuth has 18 months on me + YC distribution + framework endorsements. They're better for [specific things]. AuthForge is better for [specific things — B2B org-switching, 1-binary self-host, framework-agnostic without TS-only constraint]. If you're starting fresh with Next.js and don't need B2B yet, use BetterAuth." |
| "Why $99 not $25?" | (after Section 6 fix: pricing is $29 self-serve, $199 concierge — the answer becomes natural) "It's $29 to match the market band." |
| "Will you pivot the license to BSL?" | "MIT, written into the CONTRIBUTING file. No CLA. If the project ever changes license, the prior version stays MIT forever." |
| "What if you get acquired?" | "OSS code stays under MIT regardless. If hosted tier shuts down, I'll publish migration tools — written commitment in the docs." |
