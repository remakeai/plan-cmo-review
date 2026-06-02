# AuthForge Launch Playbook

**Multi-channel sequenced launch. NOT a "Show HN and hope" plan.**

## Pre-launch gate (must be true before pulling Day 0 trigger)

- [ ] Time-to-hello-world for a Next.js developer is <5 minutes (timed by 3 external testers)
- [ ] Docs site live with copy-paste React components for: email/password, Google OAuth, GitHub OAuth, team invites
- [ ] GitHub repo: README quality > code quality. Clear value prop in first 3 lines. Animated demo GIF.
- [ ] Pricing page live with 3-tier structure (per Section 6b restructure)
- [ ] 3-5 named small-team SaaS customers actively running AuthForge in dev environment (concierge cohort)
- [ ] At least 1 unprompted referral inside the concierge cohort
- [ ] Founder blog post drafted: "Why I left Stripe to build AuthForge" (embargoed for Day 0)
- [ ] Twitter launch thread drafted with screenshots and decisions
- [ ] LinkedIn post drafted
- [ ] Product Hunt hunter identified (relationship in place)
- [ ] List of 10-20 dev-Twitter influencers prepared with personalized DM templates

**If ANY of the above is missing, push launch by 1-2 weeks. Calendar-gate is fine for dev tools but not at the cost of shipping unprepared.**

---

## Pre-launch sequence

### Day -30 to Day -8: Audience build
- 2 blog posts/week on auth topics (positioning + technical depth)
- 1 build-in-public Twitter thread/week
- Launch newsletter; promote in every blog post
- Show up in Reactiflux / T3 / IH Discord communities — substantive, not promo
- Set up concierge cohort: 5 named small-team SaaS engineers using AuthForge in dev

### Day -7: Soft pre-announce
- Personal email to ~50 friends, ex-Stripe colleagues, YC network: "I'm launching AuthForge next Monday. Here's a beta link if you want to play. No need to upvote anything — just want your honest take."
- Goal: surface bugs + get 10-15 people genuinely interested.

### Day -3: Build-in-public Twitter thread
- "I'm launching the auth tool I wish existed when I was at Stripe — Monday morning. Here's a sneak peek. [GIF demo] Thread →"
- Pre-warms the algorithm for Day 0 amplification.

### Day -1: Final checks
- Verify all links work, payment flow tested, docs site loads fast
- Schedule social posts via Buffer/Typefully for Day 0 timing
- Confirm 3-5 influencer DMs ready to send Day 0 +2hr
- Confirm Product Hunt hunter ready (for Day +7 separate launch)

---

## Day 0 (Monday, Pacific time) — hour-by-hour

| Time (PT) | Channel | Action |
|---|---|---|
| **5:00 AM** | Hacker News | Post Show HN: "Show HN: AuthForge — Auth SDK for [chosen wedge stack] (open source)". Title is critical: use the wedge from action item #1. Link to GitHub repo (HN audience prefers code-first link over landing page). |
| **5:15 AM** | Founder blog | Publish "Why I left Stripe to build AuthForge" (was embargoed until now) |
| **6:00 AM** | Twitter | Launch thread: hook tweet + 8-10 reply tweets with screenshots, decisions, story. Link to HN at end (not the start — HN penalizes when title-link is to social media). |
| **6:30 AM** | Email blast | To the 50-person network: "It's live on HN. If you've tried the beta and it was useful, would love a genuine comment. No fake upvotes." |
| **7:00 AM** | Newsletter | First-ever newsletter blast (if subscribers exist): "AuthForge is live. Here's the story." |
| **7:30 AM** | Influencer DMs | Send 10 prepared personalized DMs to dev-Twitter influencers (Theo, Lee Robinson, Rauch, Shadcn, etc.) with: "AuthForge is live, [specific reason it matches your taste], here's the HN link if you find it interesting." NOT a request to retweet — let them choose. |
| **9:00 AM** | LinkedIn | Long-form post (different audience overlap): more polished "why I built this" framing aimed at engineering managers / CTOs. |
| **11:00 AM** | Hacker News | Monitor comments. Respond to every question within 30 min for first 6 hours. This is the most important thing to do all day. |
| **2:00 PM** | Discord communities | Share in Reactiflux #showcase, T3 Discord #show-and-tell, Theo's Ping — ONLY if you've been active in those communities and have rapport. Otherwise skip — drive-by promo gets ignored or banned. |
| **All day** | Personal | Stay at desk. Reply to every comment, email, DM within 30 minutes. Take breaks but be reachable. |

### Day 0 explicit DO NOTs

- DO NOT post to r/programming (auto-removal + ban risk is high)
- DO NOT ask people to upvote on HN (against rules; ban risk)
- DO NOT cross-post the exact same content to multiple platforms simultaneously (HN penalizes; LinkedIn / Twitter audience differs anyway)
- DO NOT respond defensively to negative HN comments. Acknowledge, offer to discuss, move on.

---

## Day +1 to Day +7

| Day | Action |
|---|---|
| **+1** | Cross-post to IndieHackers (let HN have its day first). Tweet update on Day 0 traction numbers (be honest — "we hit #14 on HN, 300 stars, 45 hosted trial signups"). |
| **+2** | Compliant cross-post to r/SideProject (NOT r/programming). Read sub rules first; some require disclosure that you're the maker. |
| **+3** | Reply to every HN comment that came in after Day 0 (HN comments compound for 48 hours). |
| **+5** | First "AuthForge launch week" retro blog post: what worked, what didn't, what's next. Honest. |
| **+7** | Product Hunt launch (separate event, different audience). Hunter pre-arranged. Coordinate with PH community Slack. |

## Day +8 to Day +30

| Period | Action |
|---|---|
| **+8 to +14** | Podcast outreach: pitch Software Engineering Daily, Syntax.fm, JS Party, ChangeLog, MFM, Indie Hackers Podcast. Pitch angle: "Ex-Stripe engineer on what's broken in auth tooling." |
| **+14 to +21** | Follow up with first 50 hosted signups personally. Concierge-onboard the ones who didn't activate. |
| **+21 to +30** | First case-study blog post with named paying customer (if consent granted). Begin SEO content cadence — 1 evergreen "[stack] auth" post per week. |
| **Throughout** | Continue 2 blog posts/week + 1 Twitter thread/week. Drop nothing — momentum compounds. |

---

## Recovery scenarios

### Scenario: Show HN flames out (<20 upvotes, falls off front page in 2 hours)
- Don't panic. HN is a lottery; failure is the base rate.
- Pivot energy to blog + Twitter + outreach amplification.
- Republish Show HN ~6 months later with new feature / milestone (HN allows re-posts with material updates).
- The multi-channel sequence means HN failure does NOT kill the launch.

### Scenario: Product Hunt #1 of the day
- Reply to every comment within 1 hour for 24 hours.
- Pre-prepare 5 short video demos to share when appropriate.
- Push HN cross-post to next week (don't burn both launches in one week).

### Scenario: Critical bug surfaces on Day 0
- Pin a comment on Show HN acknowledging it + ETA for fix.
- Tweet about it openly. Build-in-public honesty CONVERTS — defensiveness kills.
- Ship fix within 24 hours; tweet the fix.

### Scenario: Influencer retweet drives 10K+ traffic spike
- Ensure landing page + docs site can handle traffic (CDN + caching pre-launch verified).
- Have newsletter signup CTA prominent — convert traffic spike into long-term audience.

---

## Single-channel-failure protection

- HN failure ≠ launch failure (blog + outreach + Twitter independent)
- Twitter algorithm shift ≠ launch failure (blog + newsletter + Discord independent)
- One Discord community ban ≠ launch failure (multiple communities + own surfaces)
- Single influencer says no ≠ launch failure (10 DMs sent, expect 2-3 to engage)

The whole point of multi-channel sequencing: no single failure point kills the launch.
