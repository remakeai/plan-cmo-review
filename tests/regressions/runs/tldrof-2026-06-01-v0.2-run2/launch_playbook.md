# Launch Playbook — TLDR-of-TLDRs

Two cohorts, two gates, two sequences. Synthesized from `marketing_plan.md` Section 5.

---

## Cohort 1 — HN-cohort (Persona A: "Devin")

**Gate:** Calendar Day 20-22 (per design doc Approach C). Acceptable for this cohort; HN benefits from a shipped-product moment.

**Channels (multi-channel; refuse single-channel):** Show HN (primary), IndieHackers, /r/SideProject, X build-in-public + amplification, personal network email, LinkedIn (secondary, low-leverage for this persona).

### Day -22 to -7 (pre-launch ramp)

| Cadence | Activity | Why |
|---|---|---|
| 2/week | X build-in-public posts on architecture (Mailgun inbound, Claude pipeline, bankruptcy onboarding flow) | Build engineering credibility audience pre-launch; produces day-0 amplification material |
| 1/week | Substack technical post | SEO + credibility; Substack subs growing 30-80 by Day 0 realistic |
| daily | Light HN comment presence on adjacent threads (NO product mention) | Name recognition for Show HN day |
| ongoing | DM 5-10 named HN-cohort contacts: "launching in 2 weeks; want a private trial?" | Day -7 soft-launch beta cohort |

### Day -7

| Hour / Day | Action |
|---|---|
| Day -7 | Personal network email to ~50 named contacts; ask 5-10 to amplify launch day |
| Day -7 | Confirm hunter for Product Hunt if doing PH (often skipped if no hunter relationship) |
| Day -5 | HN draft to 2-3 trusted technical reviewers for headline/copy critique |
| Day -3 | Build-in-public preview thread on X with screenshots of bankruptcy magic-moment |
| Day -1 | Final review of: landing page above-fold copy, /onboard flow, error states, mobile responsive |

### Day 0 — Launch day (hour-by-hour)

**TIMING: Submit Show HN between 6-8am PT (Tuesday-Thursday optimal; avoid Friday + weekend).**

| Hour PT | Channel | Action |
|---|---|---|
| 06:00 | Show HN | Submit. Title: "Show HN: tldrof — 50 unread newsletters? Forward them all. Get one digest in 60 seconds." (test alternative: "Show HN: Inbox debt cleared — AI digest of forwarded newsletters in 60s") |
| 06:00-10:00 | Show HN | Camp the thread; reply to EVERY comment thoughtfully; engage with critique honestly; embed loom / screenshot of bankruptcy flow on first relevant question |
| 08:00 | Personal network | Text/DM 5-10 launch amplifiers: "live on HN now — link"; ask honest engagement (NOT vote-asks; HN penalizes) |
| 10:00 | X | Thread with HN link, screenshots, architecture brief; tag 2-3 build-in-public mutuals |
| 12:00 | LinkedIn | Long-form post (different framing — corporate / business-time-saved angle) |
| 14:00 | Email | Send to Substack list (30-80 subs) with launch story |
| 16:00 | IndieHackers | Cross-post (HN-first to avoid duplicate-content penalty); engage in comments |
| 20:00 | Reddit | If HN traction is good, cross-post to /r/SideProject (compliant: short post, link, "feedback welcome") |
| All day | All channels | Reply to every comment / DM / signup question within 1 hour; founder is on-thread |

**Stop conditions if launch failing by mid-day:**
- If Show HN front page miss (<20 upvotes by hour 4): pivot to maximize IndieHackers + Reddit + email push; do NOT spam X with re-asks
- If /onboard / signup / payment broken on launch day: page banner ASAP, hotfix, post Show HN update transparently

### Day 1-7

| Day | Action |
|---|---|
| +1 | /r/Entrepreneur if signal warrants; second X thread with day-1 numbers (signups, time-saved-aggregate) |
| +2 | /r/SideProject if not done day 0; engage IndieHackers thread |
| +3 | First retrospective post on X / Substack: "what I learned from day 1 of launch" — converts curiosity into trust |
| +5 | Email to /onboard-but-not-paid signups: gentle check-in, "anything getting in the way?" |
| +6 | Trial-end-reminder cohort 1 (per Stripe trial flow); track conversion |
| +7 | Product Hunt launch if hunter ready (NEW launch event, different audience) |

### Day 8-30

| Week | Activity |
|---|---|
| Week 2 | First podcast appearance if booked; build content backlog (3-5 launch-retrospective posts across X/Substack/LinkedIn) |
| Week 3 | Vohra "very disappointed" survey to first-cohort users (PMF signal capture) |
| Week 4 | Substack retrospective with traction numbers; pitch 5 more podcasts; first paid Google search test ($50-200) on competitor terms |

---

## Cohort 2 — Corporate (Persona B: "Maria"), PMF-gated

**Gate:** PMF signal (Vohra ≥40% "very disappointed") from concierge-onboarded beta cohort. NOT calendar.

**Channels:** LinkedIn warm-intro DM (primary recruit), concierge 1:1 onboard (primary delivery), vertical paid placement (post-PMF scale), industry-Slack peer referral (post-PMF growth).

### Day -22 to -7 (pre-launch)

| Cadence | Activity |
|---|---|
| 2/week | LinkedIn content pivot — corporate-segment-framed inbox-overload posts; "how a finance director cut newsletter time 80%" angle |
| Day -14 | Write 20-30 personalized LinkedIn DMs to first-degree connections in target verticals (finance, legal, healthcare, agency ops); soft-recruit for private beta |
| Day -7 to -1 | Onboard 5-10 corporate betas via 30-min 1:1 Zoom; founder personally walks through bankruptcy flow + auto-forward setup; collects content sample + reading-speed self-report |

### Day 0 to +14 (HN launch period — corporate cohort RUNS IN PARALLEL, no public launch)

| Day | Action |
|---|---|
| Day 0-14 | Corporate betas dogfooding; founder daily check-in (text or short call); capture content-signature differences vs HN-cohort dogfood; tune Claude prompts for corporate content type (longer-form, narrative, regulatory) |
| Day +7 | Mid-trial 1:1 with each beta: "what's working, what's broken?" |
| Day +14 | Vohra "very disappointed" survey to all corporate betas |

### Day +21 — PMF gate decision

**If ≥40% answer "very disappointed":** Fire next stage. Corporate-cohort launch sequence begins.

**If <40%:** Iterate. Tune dedup quality / summary style for corporate content type. Re-recruit cohort 2 (3-5 fresh corporate betas) for next 14-day cycle. Repeat until PMF gate fires OR 90 days elapsed without it firing (at which point corporate-segment thesis is in serious question; revisit positioning).

### Day +21 to +60 (if PMF fires)

| Action | Detail |
|---|---|
| Launch Corporate Pro tier ($19/mo, $199/yr annual) | Separate landing page / variant; same product, different copy emphasizing M365 / corporate / paid-account-locked use cases |
| LinkedIn content series | 8-12 corporate-segment posts over 6 weeks; case studies from corporate betas (with permission); industry-voice-style writing |
| Paid placement test 1 | $1-3K placement in CFO Dive / Axios Pro / Healthcare Dive (pick 1 vertical based on which betas came from); measure signup + conversion |
| Warm referrals | Ask each paying corporate user "who else like you?" — expect 1-2 intros per paying user |
| Industry-Slack outreach | Founder joins 2-3 corporate-vertical Slack communities; builds presence 4 weeks before any product mention; one helpful post per week |

### Day +60 to +90

| Action |
|---|
| Trade-publication review outreach (pitch CFO / GC / healthcare pubs for product review) |
| Identify 1 industry event for Q3-Q4 (sponsorship or attendance for warm-intro multiplier) |
| Affiliate pilot: identify 1-2 industry creators / consultants for revenue-share partnership test |

---

## Risk callouts (across both cohorts)

| Risk | Mitigation |
|---|---|
| HN miss (lottery) | Multi-channel Day 0 burst; personal network amplification; IndieHackers + Reddit backup; corporate cohort untouched by HN outcome |
| Algorithm shift (X / LinkedIn) | Don't lean on any single channel; email list + Substack as owned-channel insurance |
| Reddit subreddit ban | Strict compliance per sub rules; never spam; engage before posting |
| Corporate PMF gate doesn't fire | Iterate, recruit cohort 2; if 3 cycles fail, revisit corporate thesis |
| Launch on holiday week (drift) | Avoid; submit Tue-Thu; target non-holiday week explicitly |
| Founder burnout from concierge | Cap concierge cohort at 20 users total; if demand exceeds, formalize self-serve flow + waitlist |

---

## What this playbook explicitly REFUSES

- "Show HN as the entire distribution strategy" — multi-channel mandatory
- Calendar-gating the corporate launch — PMF gate mandatory for that cohort
- Cold public launch for corporate segment without concierge dogfood first
- Single audience treated as single launch — split-cohort mandatory
- Audience-build deferred to post-launch — pre-launch ramp mandatory
- Free trial as the only acquisition mechanic — concierge waitlist for corporate
