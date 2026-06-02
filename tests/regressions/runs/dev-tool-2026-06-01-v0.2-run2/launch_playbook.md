# AuthForge — Launch Playbook

## Launch gate (PMF-signal-driven, not calendar)

Launch fires when ALL of the following are true:

1. ≥40% of alpha concierge cohort (target n=5-10) answers "very disappointed" to "how would you feel if AuthForge disappeared" (Sean Ellis / Vohra test; precedent: Superhuman)
2. ≥3 of the 10 hand-recruited paying prospects have AuthForge integrated into a production app
3. ≥1 unprompted referral from the alpha cohort
4. Email list ≥1,500 subs
5. GitHub waitlist repo ≥500 stars from pre-existing audience

If hit by day 60 → launch on next Tuesday-Thursday at 9am PT.
If not hit by day 60 → extend pre-launch 30 days, iterate based on alpha feedback, re-evaluate.

**Founder must justify in writing if overriding to calendar gate.** Acceptable override: time-bound external moment (Vercel partner launch, YC Demo Day, vertical conference). Not acceptable: "I want to ship by X date."

---

## Sequenced launch (multi-channel, T-30 to T+90)

### Pre-launch ramp (T-30 to T-1)

| When | Channel | Action |
|---|---|---|
| T-30 | Blog | Post "What I learned about auth at Stripe" (no AuthForge mention; credibility prime) |
| T-28 | Twitter | Thread version of T-30 blog post; tag relevant accounts respectfully |
| T-21 | Blog + Twitter | Begin weekly build-in-public thread series |
| T-14 | Blog | Post "Why Clerk is great and where it falls short" (positioning piece; soft AuthForge tease at end) |
| T-14 | Email list | First newsletter sent (assumed list size ~1K-2K from earlier capture) |
| T-7 | Email | Soft pre-announce: "Launching next week — here's early hosted-tier access for subs" |
| T-7 | 1:1 | Personal email to 10 hand-recruited prospects: "we go live next week — want migration help?" |
| T-5 | Twitter | Countdown thread day 1 of 5 |
| T-3 | Blog | Launch primer: "AuthForge launches Friday — what it is, why I built it, who it's for" |
| T-1 | Twitter | Final hype thread; cross-link blog primer |

### Launch day (T+0; Tuesday-Thursday, 9am PT)

| Time | Channel | Action |
|---|---|---|
| T+0 / 9:00am PT | Hacker News | "Show HN: AuthForge — open-source auth SDK for Next.js (alternative to Clerk)" — title format crucial; "Show HN" prefix mandatory; specific framework wedge in title |
| T+0 / 9:05am | HN comments | Founder posts first comment with "why I built this" context; commits to replying for 6 hours |
| T+0 / 9:15am | Email | Blast email list: "We're live on HN — here's the link, your support means everything" |
| T+0 / 9:20am | Twitter | Launch thread (5-8 tweets): hook, problem, solution, demo gif, pricing, HN link, ask for support |
| T+0 / +1hr | HN comments | Reply to first wave of comments; engage substantively, never defensively |
| T+0 / +2hr | Twitter | Quote-tweet supporters; engagement burst |
| T+0 / +4hr | LinkedIn | Long-form launch post (different audience overlap; tag ex-Stripe colleagues) |
| T+0 / +6hr | HN comments | Second engagement window if post is still on front page |

### Launch week (T+1 to T+7)

| Day | Channel | Action |
|---|---|---|
| T+1 | IndieHackers | Compliant cross-post; founder story angle |
| T+1 | /r/nextjs | Compliant cross-post (read sub rules first); framework-specific angle |
| T+2 | /r/SideProject | Compliant cross-post |
| T+2 | /r/webdev | Cross-post if rules allow |
| T+3 | Personal outreach | Founder emails 10 hand-recruited prospects directly: "we're live, schedule a 30-min concierge setup call" |
| T+5 | Discord (Next.js, Vercel) | Soft mention in #show-and-tell or equivalent channels; respect community rules; no spam |
| T+7 | Product Hunt | Separate launch event; pre-arrange hunter relationship |
| T+7 | Blog | "Week 1 numbers" transparency post; ship the actual metrics |

### Post-launch compounding (T+8 to T+90)

| Week | Activity |
|---|---|
| T+2w | First podcast appearance airs (booked pre-launch) |
| T+2w | Second integration tutorial drops (SEO seed) — "Auth in Next.js App Router with AuthForge" |
| T+3w | Twitter cadence sustained; weekly build-in-public continues |
| T+4w | Blog: "30 days post-launch: real numbers, what worked, what didn't" |
| T+4w | Second podcast appearance |
| T+5w-T+12w | Integration tutorial cadence: 1/week — Remix, SvelteKit, Astro, T3 stack, Convex, Vercel templates |
| T+6w | Email newsletter cadence sustained (monthly minimum) |
| T+8w | Apply for Vercel integration listing |
| T+8w | Third podcast appearance |
| T+12w | "90 days post-launch: state of AuthForge" retrospective post + email |

---

## Channel-specific tactical notes

### Hacker News specifics

- **Title:** Must lead with "Show HN: AuthForge — [specific value prop]." Avoid hyperbole. Industry data: median Show HN = 2 points; 50+ pts = top 6%; 250+ pts = top 1%.
- **Time:** Tuesday-Thursday, 9-11am PT statistically best (most weekday HN-reader engagement).
- **First comment:** founder comment within 5 min of post, providing context, story, why-built, what's different. Set comments tone.
- **Engage for first 6 hours minimum:** disappear from comments = HN punishes. Stay calm, never defensive. "Great question — here's what we tried" beats "Actually you're wrong."
- **Don't ask friends to upvote** (HN detects vote rings; can shadowban). Do email list + tweet linking the post; organic.
- **Have the HN-front-page-load-test ready:** Vercel scaling, image CDN warm, signup flow tested at 100 RPS.

### Twitter/X specifics

- Pre-launch: 3-5 threads/week, daily replies in dev-Twitter circles
- Launch day: 5-8 tweet launch thread, NOT one mega-tweet
- Post-launch: continue build-in-public weekly; metrics transparency builds trust

### Reddit specifics

- **DO NOT post to /r/programming directly.** Mods strict; auth SDKs read as self-promo; bans common.
- **Better targets:** /r/nextjs, /r/SaaS, /r/webdev, /r/SideProject — each has different rules; read them.
- **Wait 24 hours after HN** before Reddit cross-post; never cross-post to multiple subs same day.
- **Lead with story, not pitch:** "I left Stripe to build OSS auth — here's the post-mortem of week 1" outperforms "Check out AuthForge."

### Product Hunt specifics

- **Don't co-launch with HN.** Separate events, different audiences. Day T+7 minimum.
- **Pre-arrange a hunter** (not the founder) for first-degree credibility.
- **Featured assets:** gallery images, demo video, taglines, pre-written maker comment.

### Podcast guesting specifics

- **Pitch list (book pre-launch):** Lenny's Podcast, syntax.fm, Changelog, The Pragmatic Engineer, ShopTalk Show, Software Engineering Daily
- **Ex-Stripe credibility opens doors.** Lead pitch with "I led X at Stripe, now building OSS auth — here's what I want to talk about."
- **Don't pitch product directly.** Pitch a topic (auth security pitfalls, OSS-vs-closed in infra, etc.). Product mention is natural in the conversation.

---

## Risk callouts

- **HN miss:** plan survives — email list + Twitter + cold outreach + cross-posts carry. HN is not load-bearing.
- **Reddit ban from /r/programming:** likely if posted; SKIP that sub; go narrower.
- **Trust ceiling (solo founder):** "is this maintained?" objection. Mitigations: public maintenance commitment in README, named advisor/co-maintainer, transparent issue/PR response cadence.
- **Competitor counter-positioning:** Clerk could ship "OSS Lite"; Better Auth could position as the dev-Twitter darling. Mitigation: ship faster + lean into ex-Stripe credibility moat.
- **First-week server load:** if HN hits, expect 10K+ unique visitors in 24h. Test the signup flow at scale BEFORE T+0.
- **Customer support flood:** founder reserves 6-8 hours of T+0 day for support, not just HN comments.
