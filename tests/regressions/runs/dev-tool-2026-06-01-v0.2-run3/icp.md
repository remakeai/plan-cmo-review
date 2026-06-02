# AuthForge ICP Specification

## Primary persona: Maya

**Demographics**
- 28 years old
- Senior backend engineer
- 12-person seed-stage SaaS in San Francisco / NYC / remote-US
- Stack: TypeScript / Next.js / React / Postgres / Vercel / Supabase (database, NOT auth — they're shopping)
- 3-7 years experience; previously at a mid-size scaleup
- Reports directly to CTO; has tool-budget authority up to ~$200/mo without escalation

**Situation right now**
- Company just raised seed; design-partner deals in pipeline for next month
- CTO told her: "figure out auth this sprint, we need to ship sign-in + Google OAuth + invite-team flow in 10 days"
- She CAN self-host anything but won't — her time at $130K + equity is more valuable than $50-100/mo of tool spend
- Risk-averse on vendor lock-in (CTO has burned her before with vendor exits)

## Where Maya spends attention RIGHT NOW

1. **GitHub trending + repos her CTO shares in Slack**
2. **YC Bookface "auth-and-identity" alumni Slack channel** (her CTO is YC alum)
3. **Indie Hackers** — lurks, doesn't post
4. **Hacker News** — checks ~3x/week, reads Show HN occasionally
5. **Specific dev-Twitter accounts**: @t3dotgg (Theo), @leeerob (Lee Robinson, Vercel), @rauchg (Guillermo, Vercel), @shadcn, @jaredpalmer, @colinhacks
6. **Google searches for "[stack] auth tutorial"** when stuck — e.g., "nextjs 15 server components auth", "postgres rls with supabase auth"
7. **Reactiflux Discord, Theo's Ping community, T3 stack Discord**
8. **Vercel docs + Supabase docs** when she's evaluating adjacent tools
9. **YouTube**: occasionally watches Theo, Web Dev Cody, Lee Robinson keynotes

## What she currently pays for in adjacent categories (WTP evidence)

| Tool | Price | Why she pays |
|---|---|---|
| Vercel | ~$20/mo/seat | Saves her 5+ hrs/week vs self-hosting |
| Supabase | $25 base + usage | Postgres + storage + edge functions in one |
| Linear | $10/seat | Replaces JIRA pain |
| PostHog | usage-based | Analytics + flags + replays |
| Resend | $20/mo | Transactional email |
| Sentry | $26-80/mo | Error monitoring |
| ChatGPT Plus | $20/mo personal | Coding assist |

**Pattern:** Maya pays $20-100/mo PER TOOL when the tool saves her engineering time. She doesn't price-shop within this band; she trust-shops based on DX, docs quality, and reputation in her dev-Twitter feed.

## What she complains about in adjacent categories (positioning ammunition)

- "Auth0 pricing cliff at 7K MAU is brutal — we got hit overnight."
- "Supabase Auth is fine but I can't customize the Google OAuth scope easily."
- "Clerk is great but my CTO doesn't want another closed-source vendor; we already have 12 SaaS subscriptions and one is going to deprecate or 10x price next year."
- "I tried NextAuth/AuthJS but the maintainer burnt out and now the docs are stale and the OAuth providers break randomly."
- "I don't want to write our own auth — every senior eng who has done it has war stories."

## Objections she'll raise to AuthForge

1. **"How do I know you'll be around in 2 years?"** — solo OSS project risk. ANSWER: ex-Stripe + MIT license + active GitHub = you can always fork or self-host indefinitely. Founder presence answers this over time.
2. **"Why not just use Clerk? It works."** — incumbent inertia. ANSWER: needs sharper differentiation than "simpler/more flexible." Likely needs vertical wedge.
3. **"$99/mo is more than Clerk Pro for less."** — pricing objection. ANSWER: restructure pricing per Section 6b.
4. **"I don't have time to evaluate a new auth tool right now."** — biggest objection. ANSWER: time-to-hello-world <5 min, copy-paste examples in docs (Stripe-style), one-call concierge onboarding offer.
5. **"Can we self-host if we outgrow the hosted tier?"** — exit-cost concern. ANSWER: yes, MIT SDK is identical to what hosted runs. Explicitly market this.

## Reasons she'll convert

- Founder is ex-Stripe — instant DX trust signal
- OSS + MIT = no lock-in fear
- 5-minute time-to-hello-world in docs
- Copy-paste React components that match her stack
- Founder is responsive in Discord/Twitter/email — she can ask the maintainer directly
- Pricing transparent + reasonable vs Auth0
- Specific wedge that matches her stack (if positioning sharpens per action item #1)

## NOT the ICP — explicit exclusions

- **Indie hackers shipping side projects** — they self-host the free SDK and never pay. Welcome as community but don't tune product for them.
- **Fortune 500 / regulated enterprise** — needs SOC2, SSO unlimited, audit logs, dedicated infrastructure. AuthForge v1 doesn't have this; pitching them wastes founder time.
- **Agency contractors** — use whatever the client mandates; not a buyer persona.
- **Crypto/web3 projects** — wallet-first auth is a different product. Stytch and Privy already won this niche.

## Validation criteria for ICP fit

Before launch, founder should have:
- At least 10 conversations with named "Maya"-shaped engineers at seed/A-stage SaaS
- At least 3 of those say "yes I'd pay $29-99/mo for this if it shipped today"
- At least 1 verbal commitment to be design-partner / first paying customer
- At least 1 of those engineers naturally referring AuthForge to a colleague unprompted

If these fail to materialize, ICP is wrong and Section 2 + 5 need revision before launch.
