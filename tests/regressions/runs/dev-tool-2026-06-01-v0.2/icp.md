# AuthForge — ICP Specification

**Companion to `marketing_plan.md`.** This is the named persona AuthForge's marketing should target. NOT "backend engineers." A specific person.

## Primary persona: "Priya"

**Role:** Lead backend engineer / tech-lead at a 5–25 person Series A startup
**Tenure:** 4–8 years backend; first or second tech-lead role
**Stack:** Modern — Node.js (most common), Python, or Go; TypeScript-first; deployed on Vercel / Render / Fly / Railway
**Team shape:** No dedicated security or identity engineer. Auth is "Priya's job by default."
**Current auth situation:** One of:
  - Using Auth0, annoyed at the pricing curve and the "Okta-ification" of the product
  - Using Supabase Auth, annoyed at the coupling to Supabase DB
  - Rolled own with Passport.js / NextAuth, annoyed at maintenance burden
  - Has had at least one painful auth-related incident in the last 6 months (session bug, password reset edge case, OAuth provider change)

**Triggering moment:** First enterprise customer just asked for SOC2 attestation. Priya looked at the gap and panicked because auth audit logs / MFA enforcement / SSO are weak in current setup.

**Time profile:** Time-poor. Ships features daily. Cannot spend 2 weeks evaluating 5 auth providers.

**Money profile:** Money-acceptable. Will pay $50–500/mo per workspace for infra she trusts without manager approval; needs approval above that.

**Trust profile:** Trust-led. Buys based on (a) personal recommendation, (b) credible founder presence, (c) docs quality, (d) "have I seen this on HN/Twitter for months." Will NOT buy on price.

## Where Priya spends attention (≥5 specific places)

### Newsletters
- **Bytes** (JS/TS-heavy, ~150K subs) — high relevance
- **JavaScript Weekly** (~280K subs)
- **Console.dev** (dev-tool focused, ~50K subs)
- **Pragmatic Engineer** (engineering leadership, ~700K subs) — career content but high overlap
- **TLDR Web Dev**

### Podcasts
- **Syntax** (Wes Bos + Scott Tolinski) — JS/TS dev audience
- **Changelog** + **JS Party**
- **Software Engineering Daily**
- **Backend Banter**
- **The Stack Overflow Podcast**

### Twitter accounts followed
- @kentcdodds, @theo, @t3dotgg, @rauchg (Guillermo from Vercel), @adamwathan (Tailwind), @leeerob, @samselikoff
- Founder team accounts: @clerkdev, @supabase, @auth0

### Communities (lurker, not commenter)
- Hacker News (reads daily, comments rarely)
- r/node, r/typescript, occasionally r/programming
- Reactiflux Discord
- The Vercel/Next.js discord
- Sometimes Indie Hackers

### Conferences (watches recorded talks, rarely attends)
- React Conf, Next.js Conf
- Local Node.js meetups

## What Priya currently pays for (adjacent categories)

| Tool | Approx price | Notes |
|---|---|---|
| GitHub Team | $4/seat/mo | Approved without thought |
| Vercel / Render | $20–200/mo | Approved without thought |
| Linear | $10/seat/mo | She championed this |
| Sentry | $30–80/mo | Bought after a production incident |
| PostHog | Sometimes — varies | A/B test focus |
| Datadog | $200+/mo | Bought when ops complexity grew |
| ChatGPT Plus / Claude Pro | $20/mo personal | Daily use |
| GitHub Copilot | $10–20/seat/mo | Approved without thought |

**Anchor pricing for "infra I trust":** $30–200/mo per service is normal. AuthForge Team tier at $199/mo lands in this anchor; $99 flat undersells.

## What Priya complains about in adjacent tools

- "Pricing creeps unpredictably" (Auth0, Datadog)
- "Support is non-existent below enterprise tier"
- "Vendor lock-in is real — export stories are bad"
- "Setup is more painful than the docs imply"
- "I can't tell what tier I need without doing math on a calculator"
- "Free tiers are bait-and-switch — pricing jumps 5x at the next tier"

## Specific objections Priya will raise to AuthForge

1. "OSS-core means I'm betting on a 1-person project — what's your runway? what happens in 18 months if you stop?"
2. "Why would I pay $99/mo when Clerk's free tier covers my 8K MAU?"
3. "How do I migrate off Auth0 — what's the actual data-export script?"
4. "SOC2 attestation? Audit logs? MFA enforcement? Can you generate a SOC2 evidence report?"
5. "Is this opinionated or configurable? I don't want to spend 2 weeks tuning it."
6. "Why is your overage pricing 20x cheaper than Clerk's? Are you sustainable?"
7. "Do you have SSO? SAML? SCIM? I'll need them when my next enterprise customer asks."

## Specific reasons Priya will convert (OSS → paid hosted)

1. **Has been using OSS in production for 30+ days** and just hit her first ops pain — a key rotation she has to do manually, or an audit-log query she can't run efficiently.
2. **Landed an enterprise customer** who's asking for SOC2 evidence or SAML SSO; hosted Business tier offers a faster path than DIYing it.
3. **Founder personally onboarded her** (concierge call) and she trusts the team to be reachable when something breaks.
4. **3am page risk** — she realizes she doesn't want to be the one paged when auth breaks; hosted SLA shifts that risk.
5. **Annual billing discount** makes the math easier to defend to her manager.

## Negative ICPs (do NOT target)

- **Solo indie hackers with no MAU** — won't pay, will use OSS forever, will create support load.
- **Enterprise security teams** — wrong sales motion; they need procurement + InfoSec review + SAML day 1. Not v1 ICP. Defer to year 2.
- **Hobbyists / students** — use OSS only. Fine to have them, don't market to them.
- **Teams already happy with Clerk** — switching cost > value delta. Don't target.

## Validation plan

Founder commits to **10 user interviews this month** with people who match the Priya persona. Specific screening:
- 5–25 person team
- Backend lead role
- No dedicated security engineer
- Currently using Auth0/Supabase Auth/rolled-own
- Has been asked for SOC2 attestation in the last 12 months

If 10 interviews can't be sourced from the founder's existing network within 30 days, that itself is a signal that the audience asset is less ICP-aligned than assumed (outside-voice critique #2).
