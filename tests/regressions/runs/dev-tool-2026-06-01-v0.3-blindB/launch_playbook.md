# AuthForge Launch Playbook

**Gate:** PMF signal, not calendar. Public-launch only when >=3 concierge-onboarded beta teams report "very disappointed" without AuthForge AND >=1 has paid for the hosted tier.

**Calendar Day 60 = check-in, not a release date.**

## Phase 0 — Pre-launch audience build (T-60 to T-7)

| T | Channel | Action | Owner | Done? |
|---|---|---|---|---|
| T-60 | Blog | Add email capture (Convertkit / Beehiiv). Lead magnet: "Auth at scale" ebook from past blog posts | Founder | |
| T-58 | GitHub | Publish public repo. README names wedge, limitations, and links to 3 framework quickstarts | Founder | |
| T-57 | Twitter | Pin tweet: "Building AuthForge in public. Why: [one-liner wedge]. Repo: [link]." | Founder | |
| T-55 | Personal email | Email 10 named people from M6 list. Personal note. Beta access request. | Founder | |
| T-50 | Blog | Post #1: "Why I'm building an OSS auth SDK after 4 years at Stripe" (with email capture) | Founder | |
| T-45 | Beta cohort | Concierge-onboard first 2 beta teams (Zoom session, founder walks them through integration) | Founder | |
| T-42 | Podcast | Pitch 5 podcasts (Syntax FM, SE Daily, Pragmatic Engineer, Changelog, JS Party) | Founder | |
| T-40 | Twitter | Build-in-public thread #1: "Week 1: shipped X, learned Y" | Founder | |
| T-35 | Blog | Post #2: "Auth at scale: what breaks past 10K MAU" (technical, no pitch) | Founder | |
| T-30 | GitHub | Ship Next.js integration tutorial + Hono tutorial. Each = SEO asset. | Founder | |
| T-28 | Beta cohort | Onboard 2 more beta teams. Run Vohra "very disappointed" question with cohort 1. | Founder | |
| T-25 | Twitter | Build-in-public thread #2 | Founder | |
| T-21 | Newsletter | Pitch Bytes / JS Weekly with target launch date | Founder | |
| T-20 | GitHub | Express + Cloudflare Workers integration tutorials | Founder | |
| T-18 | Podcast | First podcast appearance lands (recorded) | Founder | |
| T-15 | Blog | Post #3: "How we're pricing AuthForge (and why we changed our mind)" — public pricing rationale post | Founder | |
| T-14 | Beta cohort | 5 concierge-onboarded teams total. Re-run "very disappointed" — gate decision. | Founder | |
| T-10 | Twitter | Build-in-public thread #3 — preview launch | Founder | |
| T-7 | Personal email | Email ~50 people directly with launch date. Individual notes, not blast. | Founder | |
| T-3 | Twitter | Final pre-launch thread with concierge beta results (real numbers, honest) | Founder | |
| T-1 | Repo | Final check: docs site, quickstart works on fresh clone, GitHub issues template, security.txt, license, contributing.md | Founder | |

**Gate check at T-14:** If <3 of 5 beta teams report "very disappointed," DO NOT public-launch. Extend beta phase 2-4 weeks.

## Phase 1 — Launch day (T+0)

**Day chosen:** Tuesday 9am Pacific (HN traffic pattern optimal; avoid Mon/Fri).

| T+0 | Channel | Action | Notes |
|---|---|---|---|
| +0:00 | HN | Show HN post submitted | Title: "Show HN: AuthForge – OSS auth SDK with a hosted tier". First link = GitHub repo, NOT landing page. Body: technical specifics, what we're worse at, link to comparison post. NO marketing-speak. |
| +0:30 | Email | Email the 50-person personal network with the HN link, asking for HONEST comments (not upvotes — comments are the algorithm signal) | |
| +1:00 | Founder | Monitor HN comments. Reply to every technical question within 15 min for first 4 hours. Tone: engineer answering engineers. | |
| +2:00 | Twitter | Thread with HN link, tagging no one. Lead with the technical novelty. | |
| +4:00 | Lobste.rs | Cross-post IF community rules allow self-post. Different angle than HN (more technical depth). | |
| +6:00 | Beta cohort | Email beta teams: "We launched! Here is the public link." Many will share organically. | |
| +24:00 | Indie Hackers, Pragmatic Engineer Slack | Cross-post (founder has standing) | |
| +48:00 | r/nextjs, r/typescript | Compliant cross-post; lead with technical specifics | |

## Phase 2 — Post-launch (T+3 to T+90)

| T | Channel | Action |
|---|---|---|
| T+3 | Blog | Quick retrospective: "Day 3: what we saw, what we shipped, what we missed" |
| T+7 | (skip Product Hunt — wrong audience class for dev infra) | |
| T+14 | Podcast | Second podcast appearance lands |
| T+21 | Blog | Deep retrospective with traction numbers (honest, including misses) |
| T+30 | Blog | Comparison post: "AuthForge vs Better Auth vs Clerk: when to pick which" — honest, including where AuthForge loses |
| T+45 | GitHub | First major release after public launch (incorporating community feedback) |
| T+60 | Newsletter | First monthly newsletter to email list — "What we shipped this month" |
| T+90 | Launch Week #1 | First quarterly Launch Week (Supabase pattern): 5 days, 5 coordinated releases |

## Risk mitigations active during launch window

- **HN front page miss:** founder's blog amplifies; build-in-public cadence continues; beta cohort dependence carries the trust signal regardless of HN.
- **Better Auth founder engages:** be honest. Don't trash. Acknowledge Better Auth as the OSS-TS-auth leader; differentiate on hosted tier ops AND specific wedge.
- **Negative HN comment thread:** engage substantively in EVERY top comment within first 4 hours. The thread becomes the marketing. "Engineer who answers hard questions" is the trust signal.
- **Repo gets brigaded with frivolous issues:** issue templates that require reproduction steps. Pin a CONTRIBUTING.md.
- **Security report on launch day:** have security.txt + private disclosure email ready. Vulnerable-by-launch-day is brand-killing.

## What success looks like

- T+30: 500+ email subscribers, 1.5K+ GitHub stars, 3+ podcast appearances landed, >=2 paying hosted-tier customers, 5+ concierge-onboarded beta teams expanded, 1 named logo on landing page.
- T+90: 1K+ email, 5K+ stars, >=10 paying hosted-tier customers, first quarterly Launch Week shipped, 1 inbound conference talk invite.

## What failure looks like (and the response)

- T+30: <100 email, <500 stars, <2 paying — DO NOT panic-launch on more channels. Instead, conduct 10 lost-deal interviews. Most likely failure mode: wedge wasn't sharp enough; positioning vs Better Auth was weak. Pivot the wedge BEFORE scaling channels.
