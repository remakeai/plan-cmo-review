# AuthForge Launch Playbook

**Skill:** plan-cmo-review v0.3.0
**Dev-tool motion class — v0.3 tonal rule LOAD-BEARING in this document.**

---

## Gate (before any of this runs)

Public launch only after BOTH:
- **PMF signal:** ≥40% of alpha-cohort design partners answer "very disappointed" to "how would you feel if you could no longer use AuthForge" (Vohra/Superhuman test).
- **3 paying design partners minimum** (NOT stargazer self-signups; real paying conversations with named buyers).

If gate doesn't fire by Day 60, **delay launch** rather than calendar-launching cold. Calendar launch into no PMF signal burns the one HN shot.

---

## Pre-launch (Day -30 → Day 0)

| Day | Channel | Action |
|---|---|---|
| -30 | Blog/newsletter | Newsletter migration complete. Weekly cadence in flight. |
| -28 | Docs | Next.js + Remix integration tutorials live (start SEO clock) |
| -21 | Docs | SvelteKit + Fastify tutorials live |
| -14 | Newsletter | "Why we built AuthForge" — architecture deep-dive, honest section on Clerk's UI advantage and Auth0's enterprise maturity |
| -14 | Docs | Hono + Rails tutorials live |
| -10 | GitHub | README finalized with: technical specs first, comparison table, named adopters (if any), contributor recognition section, code-first quickstart |
| -7 | Personal network email | Soft pre-announce to ~50 contacts (Stripe alumni, design partners, named YC founders) |
| -7 | Slack/Discord | Quiet heads-up to existing dev-tool communities the founder is in (NOT promotional — informational) |
| -3 | Twitter/X | Build-in-public thread: technical decisions thread (not "launching soon!" thread). Link GitHub repo, not landing page. |
| -1 | Blog post | Detailed launch post on existing blog. Title: "I built an open-source auth SDK — here's what's actually different and where it loses." Honest comparison table inline. Publish at 6am PT for HN-prep visibility. |

---

## Launch Day (Day 0) — hour-by-hour

### Pre-launch checks (T-2h, ~6am PT)
- [ ] GitHub repo live, README final
- [ ] Docs site live, all 6 framework tutorials published
- [ ] Landing page live (but NOT linked first on HN)
- [ ] Founder logged into HN, Twitter, Reddit, LinkedIn
- [ ] Phone on, calendar cleared for 12 hours
- [ ] First Show HN comment draft ready (founder introduces self, links docs, invites questions)

### T-0 — Hacker News (8am PT recommended for SF working hours)

**Title (LOAD-BEARING — anti-pattern #13 applied):**
> Show HN: AuthForge – open-source auth SDK with optional managed instance

**Title patterns explicitly REFUSED:**
- ~~"Show HN: AuthForge – the revolutionary new way to do auth"~~
- ~~"Show HN: AuthForge – best-in-class authentication for modern apps"~~
- ~~"Show HN: AuthForge – seamless, enterprise-grade auth in 5 minutes"~~
- ~~"Show HN: AuthForge – reimagining identity for the AI era"~~

**Body (post in first comment per HN convention):**
> Hi HN — I'm [name], previously at Stripe. I've been building AuthForge for the past few months: an MIT-licensed authentication SDK with an optional managed-instance tier.
>
> Quick technical specs:
> - Hybrid JWT + session model (configurable per route)
> - ~50KB SDK bundle (gzip)
> - First-class adapters for Next.js, Remix, SvelteKit, Fastify, Hono, Rails
> - Self-host with Postgres or SQLite; managed instance at $49+/mo
>
> Honest comparisons (because you'd ask anyway):
> - **Clerk** has a much better pre-built UI component story. If you want a drop-in `<SignIn/>` and never want to touch CSS, Clerk wins.
> - **Auth0** has the most mature SSO/SAML/compliance story. AuthForge v1 does not have SAML — it's on the roadmap. If you need SAML today, use Auth0 or WorkOS.
> - **Supabase Auth** is the right choice if you're already on Supabase. AuthForge is for teams who want auth standalone.
> - **SuperTokens** is the closest direct alternative. Honest delta: AuthForge bets harder on first-class Next.js/Remix DX and pairs the OSS SDK with a content engine for migration tutorials. If neither matters to you, SuperTokens may be the better pick.
>
> Where AuthForge wins, in my opinion: pricing at scale (10x cheaper than Auth0 at 100K MAU), OSS escape-hatch, and an integration story per framework that's a single file.
>
> Repo: github.com/[org]/authforge (start here)
> Docs: docs.authforge.dev
> Landing page: authforge.dev (if you prefer)
>
> Happy to answer technical questions. I'll be in this thread all day.

**Why this works (per Section 3 / Section 5c tonal rule):**
- Leads with technical specifics (bundle size, framework adapters, JWT/session)
- Names competitors honestly INCLUDING WHERE AUTHFORGE LOSES (Clerk UI, Auth0 SAML, SuperTokens)
- Code-first ordering: GitHub repo before landing page
- "Engineer wrote this for engineers" register; no marketing-speak vocabulary
- Anti-pattern #13 actively avoided throughout

### T+30min — monitor + respond
- [ ] Founder responds to every top-level comment within 1h
- [ ] No "thanks for the kind words!" platitudes — answer technical questions technically
- [ ] If criticized, acknowledge specifically. Do NOT defend. "You're right that we don't have SAML — it's planned for Q3" is correct posture.
- [ ] Pin the comparison-table comment if HN allows / paste it as a comment if asked

### T+2h — Twitter/X amplification
**Thread copy (5-7 tweets):**
> 1/ Just shipped AuthForge — open-source auth SDK + optional managed instance.
> 2/ Why I built it: at scale, Auth0 pricing hits hard (~$1500/mo at 100K MAU). Clerk has the best UI but locks pricing too. Wanted an OSS escape hatch.
> 3/ Architectural decisions: hybrid JWT+session, ~50KB bundle, first-class framework adapters (Next.js, Remix, SvelteKit, Fastify, Hono, Rails).
> 4/ Honest comparison: Clerk wins on pre-built UI. Auth0 wins on enterprise/SAML maturity. AuthForge wins on pricing at scale + OSS portability.
> 5/ Self-host free forever. Managed instance $49/mo if you don't want to run it.
> 6/ Code: [GitHub link]. HN discussion: [HN link]. Questions welcome.

**REFUSED tweet patterns:**
- ~~"🚀 Excited to announce AuthForge..."~~ (rocket emoji + "excited" register)
- ~~"The future of auth is here..."~~
- ~~"Game-changing auth platform now live"~~

### T+4h — r/programming
**Post title:**
> [Show & Tell] AuthForge: open-source auth SDK with optional managed instance — would love feedback

**Post body:** condensed version of HN body. Link to GitHub first. Acknowledge SuperTokens as comparable. Engage in comments technically; never promotionally.

### T+6h — lobste.rs (if invited)
**Title:** "Show: AuthForge open-source auth SDK"
**Tags:** auth, oss, javascript, rust (or per actual language)
**Body:** technical-first, ~50% of HN body. Lobsters audience punishes marketing speak harder than HN.

### T+24h — r/ExperiencedDevs
**Frame as discussion, not announcement:**
> Engineering trade-offs in building an open-source auth SDK from scratch — what I chose and why
>
> [Discuss JWT vs session debate, multi-tenant model, framework-adapter design — link AuthForge as context, not as launch]

### T+48h — LinkedIn
**Founder personal post,** brief:
> Shipped AuthForge this week — open-source auth SDK with optional managed instance for teams hitting pricing pain on Auth0/Clerk. Self-host free; managed at $49/mo.
>
> Technical write-up: [blog]. Repo: [GitHub].

---

## Post-launch (Day +7 → +30)

| Day | Action |
|---|---|
| +7 | Product Hunt launch (auxiliary — don't optimize for #1) |
| +10 | Pitch 5 dev-podcasts (Changelog, Software Engineering Daily, Pragmatic Engineer pod-circle, Software Defined Talk, JS Party) |
| +14 | Newsletter retro: traction numbers, what worked, what didn't (honest) |
| +21 | Ship 2-3 more framework integration tutorials (compounding SEO) |
| +30 | Public 30-day retro on blog + newsletter. Vohra-style metrics included. |
| +30 | Re-run /plan-cmo-review for post-launch growth phase |

---

## Risk callouts (launch-specific)

- **"This is just SuperTokens" comments:** acknowledge directly. "Fair — SuperTokens is the closest comparable. Here's the honest delta: ..." Do NOT pretend they aren't comparable.
- **"$49/mo for managed is too expensive for a side project" comments:** correct response is "side projects should self-host free; the managed tier is for teams." Don't drop price under pressure.
- **HN flag risk:** code-first framing + honest comparisons + responsive engagement minimize this. If flagged anyway, do NOT resubmit — accept and shift weight to Reddit/blog distribution.
- **Solo-dev signup surge:** if hosted-tier free-trial gets 100+ signups from solo devs, do not panic-optimize for them. Stay on M6 named-outreach for the first 10 paying.

---

## Anti-pattern checklist (v0.3 dev-tool tonal rule)

Before publishing ANY launch copy, run this checklist:

- [ ] Zero superlatives (revolutionary, best-in-class, enterprise-grade, world-class, game-changing, seamless, robust)
- [ ] Technical specifics in the first 2 sentences
- [ ] At least one honest comparison naming a competitor where AuthForge LOSES
- [ ] GitHub repo link before landing page link
- [ ] Reads like an engineer wrote it (test: would the founder be embarrassed to send to a former Stripe colleague?)
- [ ] No "Excited to announce" / "We're thrilled" / rocket emojis
- [ ] No trend-piggybacking ("for the AI era", "for the agentic future")

If ANY box is unchecked, rewrite. Anti-pattern #13 is the highest-cost mistake for dev-tool launches.
