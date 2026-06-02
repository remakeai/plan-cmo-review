# AuthForge — Launch Playbook (Sequenced, Multi-Channel)

**Source:** Section 5 of `marketing_plan.md`. Day 0 = formal public launch day AFTER PMF gate (≥3 alpha teams in production + ≥2 "very disappointed" Vohra responses).

**Tonal rule (load-bearing):** all public-facing copy on dev surfaces (HN, Reddit, dev-Twitter) follows the dev-tool tonal rule. NO marketing-speak. Lead with technical specifics, honest comparisons including where AuthForge LOSES, code-first links.

---

## Pre-launch (Day -30 to Day -1)

| Day | Channel | Specific action | Owner | Status |
|---|---|---|---|---|
| -30 | Blog | Long-form post: "What I learned shipping auth at Stripe" (no product mention) | Founder | TODO |
| -30 | Newsletter | Email blog readers asking for "auth pain stories" — collect + opt-in | Founder | TODO |
| -28 | DM | Pitch 5 podcasts (Software Engineering Daily, Syntax, JS Party, Devtools.fm, ShopTalk) | Founder | TODO |
| -28 | Discord (private) | Open alpha-team Discord channel | Founder | TODO |
| -21 | Twitter | Build-in-public thread #1: "I'm building an OSS auth library. Here's why." Names Better Auth, Clerk, SuperTokens with respect | Founder | TODO |
| -21 | /r/nextjs | Continue weekly answer-questions presence (no self-promo yet) | Founder | TODO |
| -14 | Blog | "AuthForge: design decisions" — architecture-first; explicit "what we do WORSE than Better Auth at" | Founder | TODO |
| -14 | Personal email | Email 30 named ex-Stripe alumni: soft pre-announce + "would love your take on the repo" | Founder | TODO |
| -10 | Discord (semi-public) | Alpha-team Discord channel goes semi-public; invite-link in blog footer | Founder | TODO |
| -7 | Twitter | Build-in-public thread #2: "10 days to launch. Here's what's in v1; here's what's NOT." Explicit anti-feature list | Founder | TODO |
| -7 | DM | Cold-warm DM to Theo (t3.gg), Lee Robinson, dev-influencers: "Repo's open; would love your take." (NO ask for amplification.) | Founder | TODO |
| -3 | Blog | "Why I think the auth market has room for one more OSS library." Explicit comparison to Better Auth, SuperTokens, Clerk | Founder | TODO |
| -1 | Internal | Final QA pass: Quickstart works on fresh Next.js + SvelteKit install. Docs are tested. Discord is staffed. Newsletter is segmented. | Founder | TODO |

---

## Launch day (Day 0) — hour-by-hour

Time zone: Pacific Time. Goal of timing: hit Hacker News during the 12-17 UTC sweet spot per Show HN data analysis (= 04:00-09:00 PT). Recommend posting at 07:00 PT (= 14:00 UTC, peak HN traffic).

| Time (PT) | Channel | Action |
|---|---|---|
| **07:00** | **Hacker News** | **Post: "Show HN: AuthForge – open-source auth library with $99/mo hosted tier"** Link to GitHub repo (NOT landing page). Body comment: lead with 3 specific architecture trade-offs; name Better Auth + SuperTokens as honest comparables; note where AuthForge LOSES; close with link to docs. |
| 09:00 | Twitter | Thread: 8-10 tweets. Lead with technical specifics ("we went with HTTP-only cookies + rotating refresh tokens; here's the reasoning"). Mention HN link near end. |
| 11:00 | Founder's blog | Launch post goes live (pinned). Includes: 5-minute Next.js Quickstart, transparent comparison chart vs Better Auth / Clerk / Auth0, code samples. |
| 11:00 | Newsletter | Email to entire newsletter list: "AuthForge is out." Short, technical, links to repo + blog + Discord. |
| 13:00 | /r/nextjs | Compliant post. NOT a duplicate of HN copy. Check sub Wiki for posting rules. Lead with the Next.js Quickstart code, not the marketing pitch. |
| 14:00 | Personal emails | Send 50 personal emails: ex-Stripe alumni + top 30 blog commenters. "It's out; here's the link; would love your take." |
| 16:00 | Discord | Open public Discord; pin links to repo + docs + alpha-team channel |
| 18:00 | Self-check | Founder pauses. Reviews HN trajectory. If <50 upvotes by hour 12, do NOT panic; sustained engagement matters more than peak |

**Time-zone notes:** 07:00 PT works for US East Coast morning (10:00 ET) and gives 6-8 hours of European prime time before US folks log off. If founder is European-based, shift +8 to hit 15:00 European = 06:00 PT.

---

## Days 1-7 (Maintain + extend)

| Day | Channel | Action |
|---|---|---|
| +1 | /r/programming | Cross-post (HN-first to avoid Reddit duplicate-content penalty). Compliant; check rules. |
| +2 | /r/sveltejs, /r/golang, /r/node | Vertical subreddits per supported framework. One per day; staggered. |
| +3 | Indie Hackers | Cross-post with "what I learned launching" angle. Lower-priority audience. |
| +5 | Twitter | Day-5 update thread: real numbers (stars, signups, contributor count, top GitHub issues). Tonal: honest, including what BROKE. |
| +7 | Blog | "AuthForge launch: 7 days in. Here's what worked, what didn't, and the bugs we hit." Trust + traction signal. |
| +7 | Discord | First public office hours (1 hour, founder answers questions live) |
| +7 | Product Hunt | OPTIONAL: separate launch event (different audience). ONLY if PMF gate met and there's bandwidth. Skip if launch is firefighting bugs. |

---

## Days 7-30 (Compound the signal)

| Cadence | Action |
|---|---|
| Weekly | 1 long-form blog post; topics rotate through framework tutorials (Next.js → SvelteKit → Remix → Hono → Express → FastAPI) |
| Weekly | Twitter thread synthesizing learnings or numbers |
| Weekly | Newsletter to list (different content from blog; behind-scenes / candid) |
| Weekly | Discord office hours (1hr; build community trust) |
| Weekly | 10 personal DMs / emails to named ICP prospects |
| Bi-weekly | Podcast appearance (if pitches landed) |
| Day 14 | First "user spotlight" post — interview alpha-team CTO who's in production; trust signal |
| Day 21 | First migration tutorial: "How to move from Clerk to AuthForge in 30 minutes." Captures the Clerk-pricing-refugee funnel. |
| Day 30 | 30-day retrospective post. Real numbers. Real lessons. Plan for next 30. |

---

## Risk callouts (carry from `marketing_plan.md` Section 5c)

- **HN miss (<50 upvotes):** do NOT re-launch within 2 weeks (HN rules forbid it). Fallback: owned channels (newsletter, blog, Twitter) + dev-influencer DMs + accelerated podcast outreach.
- **Reddit ban from a single subreddit:** post in multiple vertical subs to mitigate single-channel risk. Check Wiki rules before posting.
- **Better Auth or Clerk ships a counter-announcement same week:** stay calm. The narrative window for new entrants is 2-3 weeks; AuthForge's differentiation is the ex-Stripe + transparent comparison + concierge story, not "first to market."
- **Dev-tool tonal slip:** founder writes copy that "sells." Have one trusted reader review every public post for marketing-speak before publish.
- **Day-0 docs/Quickstart bug:** rehearse the Next.js Quickstart on a fresh laptop the day before launch.

---

## Success criteria for the launch sequence

Not "100 stars + 5 signups." Instead:

- **Day 7:** ≥250 GitHub stars (HN median for successful Show HN); ≥50 newsletter signups from launch; ≥3 named dev-influencer mentions; ≥1 alpha-team posts publicly about using AuthForge
- **Day 30:** ≥500 GitHub stars; ≥150 newsletter signups; ≥10 hosted-tier signups (NOT necessarily paying yet); ≥3 production deployments confirmed; 1 podcast appearance shipped or scheduled
- **Day 60:** ≥1000 GitHub stars (this matches the OSS-conversion-base-rate math far better than 100); ≥3-5 PAYING hosted-tier customers; ≥5 production deployments confirmed; Vohra "very disappointed" ≥40% among active hosted users

Compare to original gate (100 stars + 5 hosted signups in 60 days): the original gate is BOTH too aggressive (5% conversion) AND too lenient (100 stars). The corrected gates are more honest about base rates AND more demanding on the production-deployment signal that actually correlates with PMF.
