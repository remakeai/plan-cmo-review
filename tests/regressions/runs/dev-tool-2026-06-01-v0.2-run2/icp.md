# AuthForge — ICP Specification

## Persona: Maya — Technical Co-founder / CTO, seed-stage SaaS startup

### Demographics + context

- **Role:** Technical co-founder or first engineer at a 4-12 person YC-style startup
- **Stage:** post-pre-seed, pre-Series-A
- **Tech stack:** Next.js / TypeScript / Postgres / Vercel; React Native if mobile
- **Vertical:** any B2B SaaS, dev tools, fintech, healthtech — non-regulated-enough to not need WorkOS Enterprise
- **Background:** Big Tech alum or repeat founder; ships fast; has opinions about DX
- **Currently using for auth:** Clerk ($25-$200/mo bracket), OR rolling-her-own with Lucia/NextAuth and regretting the maintenance

### Where attention currently lives (≥5 specific)

1. **Hacker News** — daily skim of top 30
2. **Dev Twitter** — @t3dotgg, @leerob, @swyx, @rauchg, @adamwathan, @peerrich, @sidoti, AuthForge founder
3. **Lenny's Newsletter, The Pragmatic Engineer** — weekly read
4. **Vercel / Next.js / Linear blogs** — when posted
5. **/r/nextjs, /r/SaaS** — occasional
6. **YouTube** — Theo (t3dotgg), Web Dev Simplified, Fireship, Cosmos
7. **Discords** — Next.js, Vercel, Cursor, Linear

### Adjacent-category pay patterns

- $20/mo: Vercel Pro, Cursor, ChatGPT Plus, Resend, Buttondown, Linear Standard
- $50-100/mo: Linear Team, Posthog Pro, Vercel team usage
- $200+/mo: only for tools that visibly save engineering hours (e.g., Clerk if past 10K MAU; Datadog; Sentry team plans)

Maya pays for tools. The question isn't WTP; it's value match.

### Adjacent complaints (about Clerk specifically, since it's the modal incumbent)

- "Expensive past 10K MAU — the pricing curve gets ugly"
- "UI customization is limited; theming feels constrained"
- "Closed-source for our entire auth layer makes me nervous; what if Clerk pulls a Twitter API moment?"
- "Migration off Clerk later will be painful; locked-in early"

### Objection patterns to AuthForge

1. "Why switch from working Clerk integration? Migration risk."
2. "Solo founder = is this maintained? Bus factor of 1."
3. "$99/mo flat — is that actually cheaper than Clerk for my MAU?"
4. "Self-host vs hosted — what's the value of paying for hosted if I can self-host MIT?"
5. "Is the DX as good as Clerk's drop-in components?"
6. "What's the SOC2 story? My customers ask."

### Reasons Maya converts

1. **Trust the maintainer** (founder's blog credibility + ex-Stripe reputation is load-bearing)
2. **Drop-in Next.js components** match or beat Clerk's DX
3. **Pricing materially better** than Clerk past 10K MAU
4. **Owns her auth data** — escape from vendor lock-in is a real value prop for engineering-led teams
5. **Active community** — Discord/GitHub feels alive, not abandoned
6. **Compliance roadmap visible** — SOC2 timeline credible

### Discovery path (from Step 0A M2)

1. Reads founder's blog post "What I learned about auth at Stripe" (existing 20K-readers surface)
2. Follows founder on Twitter; sees build-in-public threads
3. Sees Show HN post, primed by blog/email/Twitter audience
4. Tries OSS SDK; integration in <10 min (TTHW)
5. Stays on OSS for prototype; converts to hosted on 10K MAU OR team growth OR compliance trigger

Realistic time-to-paying: 6-12 months from first touch.

### NOT the ICP (explicit out-of-scope)

- Enterprise buyers — WorkOS owns this; AuthForge can't compete on SSO/SCIM/compliance day 1
- Hobby developers / weekend projects — they'll self-host OSS and never pay; valuable for awareness, not revenue
- Devs already happy with Clerk at <10K MAU — switching cost too high; no pain
- Devs on Supabase platform — Supabase Auth wins bundle effect
- Non-Next.js / non-Remix / non-SvelteKit stacks initially — DX-first wedge needs framework focus
