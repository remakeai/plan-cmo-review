# AuthForge ICP

## Named persona
**Maya Chen** — staff engineer, 25-person seed-stage SaaS (YC-adjacent or comparable). Composite, but constructed from real archetype.

## Attributes
- Role: senior or staff engineer, often the de-facto platform lead at a small team
- Team size: 5-50 engineers
- Currently using: Auth0, Clerk, or rolling auth themselves with sessions+JWT
- Trigger event: Auth0 next-tier pricing crossover ($400/mo → $1500/mo+), or Clerk MAU surprise, or compliance asking for SAML SSO they don't have
- Budget authority: can spend $99-$500/mo on infra tools without VP sign-off
- Time poverty: 30 minutes a week to evaluate alternatives; will not "try it for fun"

## Where attention is currently spent (≥5 specific)
1. **The Pragmatic Engineer** newsletter (Gergely Orosz)
2. **Lenny's Newsletter** (occasionally; less core)
3. **Hacker News front page** (daily skim)
4. **r/ExperiencedDevs** subreddit
5. **Specific Twitter/X accounts:** Supabase team, Vercel CEO/CTO, Planetscale alumni, the AuthForge founder (already)
6. **lobste.rs** if invited
7. **Software Engineering Daily** podcast occasionally
8. **GitHub trending in their language ecosystem**
9. **Their own org's Slack / Discord** with peer engineers at sibling startups

## What they currently pay for in adjacent categories
- Vercel/Netlify ($20-200/mo)
- Sentry ($26-200/mo)
- PostHog ($0-300/mo)
- Linear ($10/seat)
- Cursor or Copilot ($20/seat)
- Auth0/Clerk (the pain point we're attacking)
- Database (Neon/Planetscale/Supabase) ($25-500/mo)

## What they complain about in adjacent categories
- **Pricing surprises at scale** (Auth0 famous for this)
- **Vendor lock-in** — "If we leave, what's the escape hatch?"
- **Pricing per-seat** when team grows fast
- **Enterprise tax** charged for basics (SAML for $1000/mo extra)
- **Closed-source = no debuggability** when things break in production at 2am

## Objection patterns to AuthForge
1. **"Why not just SuperTokens?"** — direct twin question. Need an honest answer (different positioning narrative + better DX for Next.js stack initially + founder credibility).
2. **"This is new — can I trust security in a v1?"** — auth is security-critical; conservatism is rational.
3. **"$99/mo is fine, but we need SSO/SAML"** — many small-team buyers actually need enterprise features (compliance push).
4. **"Why not just use Supabase Auth since we're already on Supabase?"** — only counters if buyer isn't on Supabase.
5. **"Will you still be around in 2 years?"** — single-founder OSS+hosted has a graveyard. Trust signaling matters.

## Reasons they would convert
1. **Pricing escape from Auth0/Clerk pricing trap** — 70-90% cost reduction at their scale
2. **OSS escape hatch** — if AuthForge disappears, they keep the SDK
3. **Founder credibility** — ex-Stripe + popular dev blog reduces the "will they be here in 2 years" risk
4. **Specific framework integration** — first-class Next.js or Remix support that Clerk doesn't have, or that Supabase Auth doesn't cleanly support
5. **Concierge migration help from the founder** — for the first 10-20 paying customers, this is the close

## Anti-ICP (explicitly NOT targeting these)
- **Solo developers on side projects.** They will star the repo, use the free SDK, never pay. Welcome them; do not tune product for them.
- **Enterprise (1000+ employees) buying SAML SSO as the primary need.** Use WorkOS or stay on Auth0/Okta. AuthForge v1 is not enterprise-ready.
- **Teams already deeply Supabase-coupled.** They should use Supabase Auth.
- **GitHub stargazers as a category.** Stars are top-of-funnel awareness; buyers come from operational pain at scale.
