# Launch Playbook — tldrof.com

**Reviewer:** plan-cmo-review v0.3.0 (blind regression run B)
**Date:** 2026-06-01
**Launch target:** calendar day 18-22 of build (CEO-locked); conditional on PMF-signal gate passing on private beta day -3

This playbook sequences a MULTI-CHANNEL launch. Show HN is ONE channel, NOT the dominant. Force-prioritizes the moat-segment (Maya, corporate product marketer) over the dogfood-aligned segment (Sam, engineer).

---

## Pre-launch gate (PMF-signal check)

**Day -5 to -3 (private beta day +3 of beta cohort):**
- Run Vohra "very disappointed" survey on the 10-15 private-beta users (CEO PC3's 3-5 HN-cohort friends + the engineer-network 10 from M6).
- Question: "If you could no longer use tldrof, how would you feel? (a) Very disappointed (b) Somewhat disappointed (c) Not disappointed."
- **If ≥30% very disappointed → proceed with calendar gate launch.**
- **If 20-30% → consider 7-day delay for tightening (founder's call).**
- **If <20% → MUST delay; the product is not yet indispensable enough to survive launch backlash.**

The CEO-locked calendar gate is honored IF AND ONLY IF this survey passes. If it doesn't, the calendar slip is the cost of avoiding ship-to-silence.

---

## Sequence

### Day -14 (build day 4-7)

**LinkedIn (founder, organic):** Build-in-public post. Headline: "I'm shipping a consumer SaaS in 3 weeks as a first-time consumer founder. Here's the design doc (link to a public Notion or gist). Here's what I'm scared of. Here's what I'd love feedback on."

Goals: (1) signal to founder's existing 996 LinkedIn followers that something is happening; (2) start the founder-credibility-build that compounds over the 30-day post-launch window; (3) test whether ANY of the 996 semiconductor followers will engage with consumer-SaaS content (likely 5-10% will).

### Day -10 (build day 8-11)

**Lenny's Newsletter classifieds:** Book the slot for launch-week issue. Cost: $400-800.

Classified copy draft (founder iterates):
> **"Outlook user drowning in newsletters? tldrof works with corporate email — no OAuth, no IT approval needed. Forward your pile, get one digest in 60 seconds. Free 7-day trial. [link]"**

**Cold-DM round 1 (LinkedIn):** Send 30 DMs to product marketers (Maya-shaped persona) found via LinkedIn search "Director of Product Marketing" + "Series B/C/D" + relevant industries (fintech, SaaS, devtools).

Template:
> "Hey [name], I'm building a tool for people drowning in newsletter subscriptions who use corporate Outlook (the segment Gmail-based AI tools can't reach). 12 of my private-beta users so far have said the killer feature is the 'inbox bankruptcy' flow — forward a backlog, get one digest. Would you be open to a free private-beta seat (no commitment, no card)? Just want feedback from 5 more people in your shape before I launch in 2 weeks."

### Day -7 (build day 11-15)

**Personal email to engineer-network 10:** Soft pre-announce. Frame as "private beta, want your feedback before public launch in 2 weeks." Goal: 5-7 private-beta dogfood signups in the Sam-cohort.

**Substack post (founder):** "What I learned about consumer SaaS in 3 weeks as a first-time consumer founder." Topic-pivot from founder's existing technical-Substack audience. Will drive 0-5 new subscribers but starts the content-cadence muscle.

### Day -5 (build day 14-15)

**Private beta concierge onboarding** (Superhuman precedent): founder does 30-min Zoom with each of the 10-15 private-beta users. Walks through forwarding setup, watches them experience the magic moment, captures questions / friction points. This is operator-shaped — the doc's watch-item flags this — but it's acceptable for the FIRST cohort only (Vohra personally onboarded the first 200).

### Day -3 (build day 16)

**PMF-signal survey on private beta** (see Pre-launch gate above). Founder makes go/no-go call.

**LinkedIn (founder):** Pre-launch announcement. "Launching Wednesday at 6am Pacific. Here's the corporate-email coverage angle. Here's the bankruptcy magic moment. Here's the link to early-access if you want to skip the line." Should drive 20-50 early signups from LinkedIn at this point.

### Day -1 (build day 17)

**X/Twitter (founder, organic):** "Launching tomorrow. Here's a 30-second screen capture of the bankruptcy flow." Visual demo.

**Final pre-launch checks:** landing page copy, magic-link emails, payment flow, "very disappointed" survey trigger ready for trial users at day +14.

---

### Day 0 — Launch day (build day 18-22; founder's choice within window)

**06:00 PT — Hacker News Show HN post.**

Headline (CRITICAL — must NOT be the engineer-bankruptcy framing; the bankruptcy framing reads as "engineer wrote this for engineers" and limits the audience):

**Recommended:**
> **"Show HN: tldrof – newsletter digest that works with Outlook + corporate email (no OAuth)"**

Body (technical specificity per skill anti-pattern #13 — no marketing-speak; honest comparisons including where you lose):
> "Built this because I'm a TLDR / AlphaSignal / Stratechery subscriber drowning in newsletters AND I noticed every existing tool (Mailbrew, Shortwave, Meco, Refind) is either Gmail-API or has its own inbox. None of them serve Outlook / M365 / corporate users — the segment whose IT often blocks OAuth into work mail.
>
> Architecture: agent-generated forwarding address (you-xxx@m.tldrof.com), Mailgun inbound, Claude Sonnet 4.6 for per-newsletter summarization + cross-newsletter dedup. No OAuth, no inbox access. Works with any email platform.
>
> The killer flow is what I'm calling "inbox bankruptcy" — you can forward a backlog of 50+ unread newsletters and get one digest in ~60 seconds rather than waiting 24h for tomorrow's digest. (Readless does the daily-digest pattern; this product does both, with bankruptcy as the primary onboarding flow.)
>
> Where it's worse than alternatives: no RSS yet (v1.0.5); auto-forward setup helper is Gmail-only at launch (Outlook coming next week); no podcast/YouTube blueprints (v1.2+). Mailbrew has a free tier and broader source mix; tldrof is paid at $9 and focused.
>
> 7-day free trial, $9/mo after. GitHub link to architecture docs (not the full codebase, sorry). Would love to know what's wrong with this take.
>
> [GitHub link to architecture] [landing page link]"

**08:00 PT (HN +2hr) — X/Twitter thread.**

Thread:
> 1/ Shipped a consumer SaaS today. Show HN here: [link]
> 2/ The story: most newsletter aggregators are Gmail-API. That means lawyers, finance, healthcare, and most corporate users with M365 / Outlook can't use them (IT blocks OAuth).
> 3/ I built one that uses forwarding-email-only. Works with any email platform. Bankruptcy flow: forward your unread pile, get a digest in 60s.
> 4/ Honest take on what's worse than alternatives: [list]
> 5/ Honest take on what makes it better: [list]
> 6/ If you're an Outlook user drowning in newsletters, free 7-day trial → [link]

**10:00 PT (HN +4hr) — LinkedIn long-form post.**

Different audience overlap than X. Headline appeals to product/marketing/business-people:
> "I just launched a consumer SaaS today. I'm a first-time consumer founder (background in semiconductor engineering at Micron). Here's what I learned in 3 weeks: [thread of 5-7 specific lessons]. Launch link below if you want to try it."

Tag relevant product-marketing community members.

**13:00 PT (HN +7hr or so — timed to Lenny's send window) — Lenny's classified hits inbox.**

The classified copy from Day -10. ~250K-500K Lenny's readers see it (most are Maya-persona shape).

**21:00 PT (HN +15hr) — Status check.**

If HN frontpage hit: amplify on X, ask private-beta users to upvote / comment authentically. If HN missed: pivot focus to Lenny's-and-LinkedIn-driven traffic, don't dwell.

### Day +1

**IndieHackers cross-post.** Frame: "I just shipped tldrof — here's the launch retrospective day 1." Drive the IH-cohort (which overlaps with Sam-persona).

**Cold-DM round 2:** founder re-engages the 30 Maya-persona contacts from Day -10 with launch link.

### Day +2

**Reddit vertical posts (community-rules-compliant):**
- r/ProductManagement: "I shipped a tool that solves [specific pain]. Here's the AMA / build journal. Not asking for upvotes — interested in feedback." (Strictly follow sub rules; some PM subs allow this, some don't — verify in advance.)
- r/sysadmin: focus on the "tool for corporate users that doesn't require IT approval" angle. Risky — sysadmins are skeptical of consumer SaaS — but the M365 angle is genuinely interesting to them.
- r/legaltech (if rules permit): focus on Daniel-persona angle.

### Day +3 to +6

**Concierge-onboard incoming paid trials** — founder schedules 30-min Zooms with first ~10 paying conversions. Captures objection patterns. Updates messaging based on what real buyers say.

**LinkedIn daily updates** — short post each day, "Launch day +3, here's what's working / what's not." Founder-credibility-build continues.

### Day +7

**Product Hunt launch** as a SEPARATE event. Different audience overlap (more designer, indie-maker, build-watcher) than HN. Hunters needed; if founder doesn't have one, lower the priority — ProductHunt without a hunter signal is lottery odds.

### Day +10 to +14

**Pitch 5 podcasts:**
- Lenny's Podcast — pitch as "indie consumer SaaS founder, here's the 14-day learning"
- Indie Hackers Podcast — pitch as "first-time consumer founder shipped"
- Pragmatic Engineer Podcast — pitch the engineering-meets-marketing angle
- The Lenny's Newsletter Pro live Q&As (if open to public pitches)
- One vertical podcast in legal/finance (if Daniel-segment data exists by then)

**Concierge-onboard the next 10-15 paying users** (founder maintains the Superhuman pattern until ~25 paying users, then transitions to self-serve).

### Day +14

**P6 KILL CRITERION CHECK: 15 paying customers?**

- If yes: continue.
- If no: this is a real go/no-go gate. Founder must NOT explain it away as "we'll iterate." Either pivot or sunset within 7 days of missing the bar. Per design doc: "v1 has failed (P6)."

### Day +21

**First content blog post** ("Tldrof Day 21: traction transparency"). Readwise-pattern transparency-as-marketing. Drive SEO long-tail and X-Twitter shares from indie/maker community.

### Day +30

**P5 KILL CRITERION CHECK: 25 paying customers?**

- If yes: per design doc, "real, expand." Proceed to Section 4's 30-60-90 day audience-build plan.
- If no: per design doc, "v1 has failed; pivot conversation starts." Refer to /office-hours outside-voice reframe (B2B-team pivot).

---

## Channels NOT used (and why)

- **TikTok:** wrong audience for any of the 3 personas; production cost high for solo founder.
- **Paid Google/Meta ads:** capital-intensive; no retention data yet to optimize against; deferred to post-PMF.
- **Influencer partnerships:** trust-takes-time; deferred to month 2-3 if traction warrants.
- **Affiliate programs:** premature for v1; defer to v1.1 + referral mechanic introduction.
- **Vertical legal/finance newsletter sponsorships:** $1-3K per slot; defer until Daniel-persona conversion data exists (post-launch month 1).

---

## Risk callouts (per skill)

1. **HN miss with no recovery.** Mitigated by Lenny's classified hitting same day + LinkedIn-organic traffic + cold-DM re-engagement.
2. **All-on-Twitter dependency.** Tldrof has near-zero X presence; X is amplification not primary channel. Algorithm risk is low because X is not load-bearing.
3. **Single-Reddit-sub ban.** Each sub is treated as independent; compliance with each sub's rules is critical. If banned from r/ProductManagement: lose 1 channel, retain 4+.
4. **Concierge onboarding doesn't scale.** Accepted by design — Vohra precedent. Transition to self-serve at ~25 paying.
5. **Lenny's classified produces 0 paying customers.** Real risk; $400-800 sunk cost. Mitigation: pre-test the classified copy against 5 Maya-persona contacts before the slot fires.

---

## Hour-by-hour day-of-launch checklist

- T-4hr: final landing page check (load tests pass, payment works, magic-link email arrives in spam-clean Outlook inbox)
- T-2hr: founder makes coffee, no eating after launch (focus)
- T-0: HN Show HN post submitted
- T+5min: founder posts the link in the engineer-network 10 personal-email thread + asks for honest comments on HN (NOT upvotes — comments)
- T+30min: founder checks HN ranking; if not in /newest, troubleshoot title; if in /newest, do nothing
- T+2hr: X thread fires (only if HN has at least 5 upvotes; if HN is dead-on-arrival, don't amplify a dud)
- T+4hr: LinkedIn long-form post fires
- T+6-8hr: Lenny's classified land in inboxes (timing depends on Lenny's send schedule)
- T+8-12hr: founder responds to every single HN comment (positive, negative, neutral). Same for X replies.
- T+24hr: status check. Plan day +1 actions based on what fired.

---

## End-of-launch retrospective (write day +14)

Founder writes a retrospective documenting:
- Which channel drove which paying conversions (with UTMs)
- Which messaging variants worked / didn't
- What objections surfaced in concierge onboarding
- What the P6 bar verdict is (15 paying / day 14)
- Specific changes for the 30-90 day plan based on launch data

Re-run `/plan-cmo-review` at day +45 to adjust 30-90 day plan against reality.
