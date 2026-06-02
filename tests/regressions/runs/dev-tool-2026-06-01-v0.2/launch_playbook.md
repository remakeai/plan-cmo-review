# AuthForge — Launch Playbook (v0.2)

**Companion to `marketing_plan.md`.** Hour-by-hour and day-by-day launch sequencing for the Show HN moment, embedded in a longer pre-launch and post-launch arc.

**Launch gate (revised):** NOT calendar — gated on (a) ≥3 of 5 design-partner pilots reporting dependence (use ≥3x/week for 4 consecutive weeks) AND (b) ≥2 of 5 pilots converted to paid hosted. If both pass, launch in the following 2-week window. If not, iterate before launch.

---

## Pre-launch (Day -90 to Day -1)

### Day -90 to Day -60: Foundation
- Set up landing page with newsletter capture
- Identify and email 30 small-team backend leads in network → enroll 5 design partners (free hosted pilot, 60 days, in exchange for product feedback + future testimonial)
- Pitch 5 podcasts (Syntax, Changelog, Software Engineering Daily, Backend Banter, JS Party)
- Write blog post #1: "What I learned auditing 12 startup auth implementations" (audience-warmth, not launch-related)
- Begin Twitter cadence: 3 posts/week, 1 thread/week

### Day -60 to Day -30: Building reach
- Blog post #2: "Why I left Stripe to fix open-source auth" — THIS is the post the launch will hang off of; ensure it can stand on its own as an HN-worthy long-read
- Pitch guest posts to Bytes / Console.dev / JS Weekly
- First 2 podcast episodes go live → amplify each on Twitter + blog
- Newsletter at ~200–500 subs
- Design partners using OSS in production; collect dependence + conversion data weekly

### Day -30 to Day -7: Pre-launch warmth
- Soft pre-announce to newsletter ("launching in ~4 weeks, here's a sneak peek + design partner case studies")
- Blog post #3: comparison piece ("AuthForge vs Auth0 vs Clerk: the honest tradeoffs" — must include the parts AuthForge LOSES, not just wins; this is what makes it trustworthy on HN)
- Twitter build-in-public: weekly progress thread, screenshots, design-partner quotes
- Final SDK polish; ensure Time-to-Hello-World is <10 minutes (industry benchmark — 3-4x conversion lift below this threshold)

### Day -7: Personal network outreach
- Email ~50 specific people you know personally: ex-Stripe colleagues, indie hacker friends, founders in your network
- Specific ask: "We launch next Tuesday. If it resonates, an HN upvote and a share would mean a lot. Here's the link to bookmark." (Don't ask for *fake* engagement; ask for *real* engagement from genuine connections.)
- DO NOT spam. ~50 personalized notes, not a mass email.

### Day -3: Twitter build-in-public thread
- Founder posts a thread previewing the launch. Topics:
  - The "why" (rerun of the blog post 2 thesis)
  - Design partner quotes (with permission)
  - "Show HN on Tuesday — here's what to expect"
- Use existing 3K-follower audience to seed momentum

### Day -1: Final prep
- HN post drafted, reviewed by 2 trusted devs (NOT for fake upvotes — for *honest* title-and-text feedback)
- Title formula candidates:
  - "Show HN: AuthForge – Open-source auth without the Auth0 bill"
  - "Show HN: AuthForge – I left Stripe to build auth I'd actually want to integrate"
  - "Show HN: AuthForge – Self-host auth in 10 minutes, or use our hosted tier"
- Pick ONE. Test with 2 dev friends for click instinct.
- Newsletter draft queued for Day 0 +24hr send
- All channel content prepared and scheduled

---

## Launch day (Day 0) — hour by hour

| Hour (Pacific) | Channel | Action | Why |
|---|---|---|---|
| **06:30** | Hacker News | Post Show HN | HN sweet spot is 6–8am PT for front-page momentum |
| **06:35** | Founder presence | Pin browser tab to HN post; respond to first comments in real time for first 2 hours | Engagement in first 2 hours determines front-page survival |
| **08:30** | Twitter | Launch thread referencing HN post; tag a few friends asked in advance to amplify (with permission) | Cross-channel push once HN has initial traction |
| **10:30** | LinkedIn | Long-form post (different audience overlap; minimal LinkedIn investment but free reach) | Different audience surface |
| **12:00** | Newsletter | Send launch email to subscribers | Warmest cohort — high conversion |
| **14:00** | r/programming | Cross-post — *NOT* a copy of HN; reframed for r/programming community ("Open-sourced our auth library — here are the technical tradeoffs we made") | Different community, different framing required |
| **15:00** | r/node | Cross-post with framework-specific framing ("Node devs: here's a new auth library — would love feedback") | Smaller, more engaged audience |
| **18:00** | HN | Continue responding to comments; do NOT downvote critics; address concerns honestly | Founder presence is the #1 trust signal on HN |
| **22:00** | Day-1 wrap | Post brief retrospective thread on Twitter: "Day 1 numbers, what surprised me, what's next" | Sustain narrative momentum |

---

## Post-launch (Day +1 to Day +30)

### Day +1 to Day +7
- Daily Twitter updates with traction numbers (transparent, including misses)
- Respond to every issue/PR on GitHub within 24 hours
- Personally email every paid signup with onboarding offer (Vohra/Superhuman concierge pattern)
- IndieHackers post on Day +2 (different audience; cross-post-with-distance pattern to avoid duplicate-content penalty)

### Day +7
- **Product Hunt launch** as a separate event (NOT same-day as HN; PH crowd is different from HN crowd; deserves its own moment)
- Pre-arrange hunter relationship and PH-specific assets (visuals, GIF demo)

### Day +14
- First podcast guest spot from earlier pitching drops → amplify everywhere
- Begin "AuthForge integrations" content series — one per framework per week (compound SEO surface)
- Reach out to authors of "Auth0 alternative" listicles to be added

### Day +30
- **Retrospective blog post** with real numbers ("We launched 30 days ago. Here's what happened.")
- Specific data: HN traffic, signup conversion, paid conversion, what worked, what didn't
- This post historically outperforms the launch itself for long-term trust building

### Day +60
- Re-run `/plan-cmo-review` (self-check). Measure against this plan.

---

## Risk callouts

| Risk | Mitigation |
|---|---|
| HN flops (<50 upvotes) | Existing audience absorbs. Newsletter + Twitter + design partners + content keep momentum. The launch is one moment, not the strategy. |
| HN takes off but conversion is poor | Investigate Time-to-Hello-World; instrument funnel; iterate docs and onboarding before broader push. |
| r/programming bans for self-promo | Read sub rules in advance. Post as participant, not marketer. Have a non-AuthForge comment history if possible. |
| Single negative HN top comment kills momentum | Respond fast, transparently, and don't be defensive. Acknowledge legitimate concerns publicly. |
| Wrong launch title chosen | A/B test mentally with 2 devs day before. If unsure, pick the most specific (least generic) of the 3 candidates. |
| Founder burnout in first week | Pre-schedule rest. Trust the audience to do some of the work. Don't try to be in every comment thread. |

---

## What success looks like at Day +30
- ≥5 paying hosted customers (one of the original gate criteria; revised gate above)
- Newsletter at ≥1,000 subs
- ≥2 podcast appearances live
- ≥1 guest post placed
- ≥3 of 5 design partners renewed/expanded
- HN post outcome: irrelevant to success (could be 500 upvotes or 50 — neither makes or breaks)

## What failure looks like at Day +30
- <2 paying hosted customers
- No movement on conversion despite OSS adoption — confirms M0d concern
- Founder ran out of time on audience-build, slipped to <20% time allocation

If failure pattern, return to `marketing_plan.md` Section 6 / 7 and seriously consider the outside-voice reframe (#4 in marketing_plan.md outside-voice section).
