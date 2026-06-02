# AuthForge — ICP Specification

**Source:** Section 2 of `marketing_plan.md` (CMO review v0.3.0, 2026-06-01)
**Corrected ICP per Step 0.5 M0e dogfood-mismatch finding.** The pre-correction ICP ("backend engineers building auth into their apps") was a category, not a persona, and risks mis-tuning the product to a developer hobbyist audience rather than to the paying buyer.

---

## Named persona — Maya, CTO at "Telemetric" (composite)

- **Age:** 32
- **Role:** CTO + co-founder of a 6-person B2B SaaS (4 engineers, 1 designer, 1 GTM)
- **Company stage:** Seed-stage; ~50 paying B2B customers; ~$15K MRR; 8 months from raise
- **Background:** Staff Engineer at a previous Series A; 8 years professional experience; built her own auth at her previous job and remembers the pain
- **Why she's the buyer:** at 6 people, she IS the buyer for every dev infra decision; founder + technical co-founder; no procurement, no CFO friction; can decide on $99/mo in 5 minutes if the value is clear

## Stack

- **Frontend:** Next.js 16 (App Router), TypeScript, React
- **Backend:** Next.js API routes + a few standalone Hono services; tRPC layer
- **Database:** Postgres (Neon)
- **Hosting:** Vercel (frontend), Render (backend services)
- **Auth (current):** Clerk free tier; eyeing the Pro $25/mo upgrade jump; nervous about per-MAU costs scaling as B2B customers add coworkers (B2B = 5-30 seats per customer)
- **Adjacent infra she pays for:** Vercel ($20-150/mo), Linear ($8/user/mo = $48/mo), Sentry ($26/mo), Resend ($20/mo), PostHog ($0-450/mo), Supabase ($25/mo when on it), GitHub Team ($4/user = $24/mo), Stripe (usage-based)
- **Total monthly dev infra spend:** $200-800/mo depending on the month

## Where she spends attention (≥5 named places)

1. **Pragmatic Engineer newsletter / podcast** (1.1M newsletter; 500K-650K podcast episode reach; no paid sponsorships, but earned mentions / podcast guest appearances are accessible)
2. **Bytes newsletter** (~200K JS-focused devs; sponsorship-accessible)
3. **Lenny's Newsletter** — occasionally, more for PM-adjacent content than for eng-direct
4. **/r/nextjs** — checks weekly; participates occasionally
5. **/r/sveltejs** and **/r/programming** — passive lurker
6. **HackerNews front page** — daily skim, evening
7. **Theo (t3.gg) YouTube + Twitter** — high-trust dev creator; her cohort weights his endorsements
8. **Lee Robinson** (formerly Vercel DevRel) — Next.js authority
9. **Indie Hackers** — occasionally; mostly for revenue benchmarking
10. **Software Engineering Daily** podcast — listens to weekly
11. **JS Party**, **Devtools.fm**, **Syntax** podcasts — variable; will listen to AuthForge episode if guest is interesting
12. **GitHub releases / following pages** — checks watchlist daily
13. **dev-Twitter (timeline + dev-influencer follows)** — multiple times daily

## What she pays for in adjacent categories (revealed preference)

- **Vercel** despite "Netlify is fine" — pays premium for DX + team-aligned defaults
- **Linear** despite "Notion is free" — pays for product taste + speed
- **Sentry** despite "Datadog covers it" — pays for category-best
- **Resend** despite "SendGrid is cheaper" — pays for modern API + dev-first taste

**Pattern:** Maya pays MORE for tools with engineering-team taste and developer-first API design. She does NOT bottom-shop on dev infra. She trust-shops near the top of the band.

This means: AuthForge at $29 or $199 (with clear value) wins. AuthForge at $99 (colliding with Clerk Pro+SSO) loses on direct comparison. AuthForge at $4.90 ("cheapest auth library") would signal "commodity" and lose.

## What she complains about in adjacent auth categories

- **Auth0:** "The pricing is opaque and the docs got worse after Okta. I don't trust I won't get a $5K bill next month."
- **Clerk:** "The DX is amazing but I'm watching the per-MAU math and I'm scared. My B2B customers add seats and my bill goes up. I want a flat-rate option for B2B."
- **Supabase Auth:** "It's fine if you're all-in on Supabase. I'm not. And the self-host has weird restrictions."
- **NextAuth.js / Auth.js:** "It's free but it took me a week to figure out which version's actually maintained, and now Better Auth is the recommended path. I don't want to bet on the wrong horse again."
- **Better Auth:** "Looks good but feels too new to bet a company on. I want to see who else uses it in production."

## Objection patterns AuthForge will face

1. **"Why not just use Better Auth?"** — most common. Counter: "Better Auth is great. We have a different bet: post-Stripe taste on the API, full migration support from Auth0/Clerk, and a hosted tier that doesn't surprise you with per-MAU bills."
2. **"Is this safe at scale?"** — security objection. Counter: ex-Stripe credibility + concrete architecture decisions (HTTP-only cookies, rotating refresh tokens, named threat model) + visible production adopters.
3. **"What if you shut down?"** — abandonment risk. Counter: MIT-licensed; full self-host path; we publish migration tooling FROM AuthForge to a self-managed instance as part of v1.
4. **"$99/mo is more than Clerk's free tier."** — pricing objection on entry. Counter (if pricing restructure is adopted): "$29/mo Starter tier with no MAU caps." Counter (if not): "$99/mo includes hosted instance + support; Clerk's $25/mo is per-MAU and gets expensive at B2B seat counts. Run the math at 5K MAU and 20 seats per customer."
5. **"Who else is using this in production?"** — social proof. Counter: name 3-5 alpha-team adopters by name (with permission) on the website + in launch post.

## Reasons she WILL convert

1. **OSS-with-real-managed-tier** — she gets escape hatch from vendor risk
2. **Ex-Stripe engineering credibility** — signals taste + quality on day one
3. **Transparent comparison content** — admitting "Better Auth is better at X" signals honesty and lets her form her own judgment
4. **Concierge migration support from Clerk** — solves the actual switching pain
5. **Predictable pricing (flat or low-per-MAU)** — solves the Clerk per-MAU anxiety
6. **5-minute Next.js Quickstart that actually works** — DX trial
7. **Named alpha-team adopters** — social proof for "safe to bet on"
8. **Founder's blog already in her reading rotation OR a high-trust referral (Theo, Lee Robinson, podcast)** — pre-trust transfers

## What AuthForge should NOT do for Maya

- Send her cold outbound sales emails
- Gate the docs behind a signup
- Use marketing-speak in launch copy ("revolutionary" / "enterprise-grade" / "seamless")
- Hide the Better Auth / Clerk comparison
- Price below $25/mo (signals commodity)
- Lead with the hosted tier; lead with the OSS repo and let the hosted tier be the upgrade path
