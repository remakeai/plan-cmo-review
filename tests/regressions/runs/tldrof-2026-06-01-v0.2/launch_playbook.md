# Launch Playbook — tldrof.com

**Companion to:** `marketing_plan.md` (full premise audit + ICP + channel selection)
**Mode:** Multi-channel sequenced launch with hybrid PMF-signal-and-calendar gate (replaces design doc's calendar-only Day 18 Show HN gate).

---

## Launch gate decision (do this BEFORE the playbook below)

**Design doc default:** Day 18 (now 20–22 per CEO review) calendar gate. Show HN morning of, cross-post to X.

**Recommended (per skill Section 5a + Step 0.5 M0a/M0d findings):** Hybrid gate.

### Gate conditions

**Hard outer calendar bound:** Day 60 from today (2026-06-01 → ~2026-07-31). Public launch must fire by then.

**PMF-signal soft gate (must pass BEFORE public Show HN / multi-channel launch fires):**
- ≥10 manually-onboarded private-beta users by end of build window
- ≥70% of them report using the product 3+ days/week for the prior 2 weeks
- ≥50% answer "very disappointed" to Vohra question ("How would you feel if you could no longer use this?")
- `filter_setup_rate_48h` ≥ 50% in the private-beta cohort (per CEO post-skill-cleanup item 2)

**If PMF signal hits before day 60:** launch immediately on the next Tuesday 7am PT.

**If PMF signal does NOT hit by day 60:** launch anyway (the calendar bound), but with explicit acknowledgment that the launch is a continuation of beta, not a victory lap. Treat as discovery, not as scale. Run launch sequence below regardless.

**Why hybrid:** pure-PMF gating delays indefinitely (founder won't ship). Pure-calendar gating ships whether or not the product is indispensable (skill anti-pattern #8). Hybrid bounds both risks.

---

## Pre-launch sequence (Day -60 → Day 0)

### Day -60 to -22 (NOW until end of build window, ~16 days remaining)

| Day | Channel | Action | Time cost |
|---|---|---|---|
| -60 (today) | Twitter/X | Create account; bio "Building tldrof.com — eliminate newsletter debt in 60s. Solo founder. Day N of build." Follow 50 ICP accounts (Pieter Levels, Lenny Rachitsky, Sahil Bloom, Marc Lou, Tony Dinh, Daniel Vassallo, founders of Readless / Meco / Readwise / Mailbrew alumni). | 30 min |
| -60 to -22 (daily, weekdays) | Twitter/X | 1 build-in-public post/day (screenshot of architecture, latency math, bug, decision, lesson). Reply 5x/day to ICP tweets. | 30 min/day |
| -60 to -22 (weekly Sunday) | Substack | 1 long-form post: "Day N of building TLDR-of-TLDRs: this week I [shipped/learned/decided X]." Cross-post Twitter threads to Substack. | 1-2 hr/week |
| -55 | Cold email | Compile 50-person personal-network outreach list: (a) 20 HN-cohort friends/peers, (b) 15 newsletter creators/authors (Lenny, Pragmatic Engineer, TLDR team, Bensbites, Latent Space, 10 Substack writers in adjacent space), (c) 15 founder-network contacts who might evangelize. | 2 hr |
| -55 to -7 | Cold email | Send 5 outreach emails/week. Pitch: free annual access for private-beta + feedback + (if they like it) one social post. Target: 10 said-yes by day -22; 20 by day -7. | 1 hr/week |
| -50 | LinkedIn | Post first long-form: "Why I'm leaving semiconductors to build a consumer product." Sets up the founder story. Use the existing 996-follower base. | 1 hr |
| -45 | Indie Hackers | Join + soft-presence. Comment helpfully on 3 posts/week. Do NOT self-promote yet. | 30 min/week |
| -35 | r/SideProject | Lurk + comment helpfully on 1-2 posts/week. Read community rules carefully. Do NOT self-promote yet. | 15 min/week |
| -30 | Substack | Write the "Why this product" essay. Sets the foundational narrative for launch-day cross-channel posting. | 2 hr |
| -22 (end of build window) | All | Take stock: how many private-beta said-yes? Twitter follower count? Substack subscribers? Adjust launch timing accordingly. | review |

### Day -21 to -7 (private beta + PMF measurement window)

| Day | Action | Time cost |
|---|---|---|
| -21 to -14 | Onboard private-beta users 1:1 via 30-min video call (Vohra pattern). Take detailed notes. | 5-10 hr total |
| -21 to -7 | Daily check-in via email or DM with each private-beta user. "How was today's digest? Anything weird? Save you any time?" | 30 min/day |
| -14 | Personal-network soft pre-announce email to remaining 30+ contacts: "Soft-launching in ~2 weeks. Reply if you want early access." | 1 hr |
| -10 | Survey private-beta cohort: Vohra question (very disappointed / somewhat disappointed / not disappointed if could no longer use). Measure `filter_setup_rate_48h`. | 30 min |
| -10 | **PMF-gate decision moment.** If signal hits, schedule launch for next Tuesday. If not, decide: extend beta 2 weeks, or launch-as-discovery per calendar bound. | 30 min |
| -7 | Substack long-form: "What I built in 20 days — and what I learned." 2,000-3,000 words. Sets up the launch-day story (founder journey + product reveal). | 3 hr |
| -7 | Begin **launch-day prep**: write Show HN draft, write Indie Hackers long-form draft, write LinkedIn long-form draft, write Product Hunt copy (defer publish to day +7), prep launch-day thumbnail/screenshots/demo GIF. | 4 hr over 3 days |

### Day -3 to -1 (launch ramp)

| Day | Channel | Action |
|---|---|---|
| -3 | Twitter/X | Build-in-public thread previewing launch: "Day N — finishing line. Tuesday I'll show you what I built." Include 1 screenshot of the 60-second magic moment. |
| -2 | Personal network | Final email to 50-person list: "Launching Tuesday 7am PT on HN. If you're around, an upvote / comment helps." (HN voting-ring policy: ASKING for upvotes is against guidelines. Phrasing: "I'd love your feedback / comments / thoughts" — feedback-soliciting is fine.) |
| -1 | Twitter/X | Build-in-public post: "Tomorrow's the day. Here's the architecture diagram I would have wanted to see at the start." Visual content tends to perform best for reach. |
| -1 | All-team check | Verify: Stripe webhooks working, Mailgun MX up, Anthropic Tier 2 confirmed, Resend SPF/DKIM/DMARC green, RUNBOOK.md printed and at hand, founder caffeinated. |

---

## Launch day (Day 0) — hour-by-hour

**Time zone:** US Pacific, because HN traffic peaks 7-10am PT. Most ICP traffic is US-based.

| Time | Channel | Action |
|---|---|---|
| Mon evening prior | All | One last check: production verify, RUNBOOK at hand, drafts queued. Get full sleep. |
| Tue 6:45am PT | Setup | Coffee. Open monitoring dashboards (Vercel, Sentry, Anthropic console, Stripe). Open the 5 draft launch copies in tabs. |
| Tue 7:00am PT | **Hacker News** | **Post Show HN.** Title: "Show HN: TLDR-of-TLDRs – 50 unread newsletters? Forward them all, get one digest in 60 seconds" (under 80 chars). First comment from founder account: link to a 60-second demo GIF + brief technical summary + invitation for feedback. |
| Tue 7:00-9:00am PT | HN | Reply to every comment within 5 minutes. Pre-written response to "How is this different from Readless?" ready to paste. Pre-written response to "Just use ChatGPT" ready. Pre-written response to "I tried Mailbrew" ready. Be HUMAN, not corporate. |
| Tue 9:00am PT | **Twitter/X** | Quote-tweet your own pinned post about the launch with a thread (5-7 tweets). Link to HN post. Tag NO ONE specifically (don't beg). |
| Tue 9:00am PT | **Personal network** | Email blast to 50-person list: "Live now: [HN link]. Feedback welcome." |
| Tue 10:00am PT | Slack DMs (if founder is in any relevant Slack communities) | Soft-mention in 2-3 channels max. Read rules. |
| Tue 11:00am PT | **LinkedIn** | Post the long-form (different audience overlap — 996-follower hardware base + whatever the founder built in last 60 days). Same launch story, more founder-journey framing. |
| Tue 12:00pm PT | HN | Continue replying to every comment. If HN traction is good (>30 points, >10 comments), comment thread is becoming the de-facto sales page. Treat it like one. |
| Tue 2:00pm PT | Twitter/X | Second thread: "First-hour numbers: X signups, Y completed magic moments, time-saved median is N min." Real-time transparency wins on Twitter. |
| Tue 4:00pm PT | HN | Still replying. By now you know whether the launch is in the "made front page" tier or the "92% bucket" tier. |
| Tue evening | Recovery | Eat. Sleep. Do NOT touch the codebase tonight — production stability matters more than features. |

---

## Post-launch sequence

### Day +1

| Time | Channel | Action |
|---|---|---|
| 8am | All metrics | Dashboard review: total signups, paid (post-trial-end will be later — track free-trial conversions), magic-moment-completion rate, churn signals, error logs |
| 10am | HN | Final round of comment replies. Add a "thanks everyone" comment if appropriate. |
| 12pm | Twitter/X | Recap thread: "24 hours in — X signups, Y paying-trial-actives, Z lessons. Here's what I'd do differently." Transparency wins. |
| 4pm | Substack | Post the recap as long-form. Cross-link to HN + Twitter. |

### Day +2

| Time | Channel | Action |
|---|---|---|
| 9am | **Indie Hackers** | Long-form launch story (different framing than HN — focus on the solo-founder-journey angle). "How I built TLDR-of-TLDRs in 20 days as a solo founder." |
| 1pm | Reddit r/SideProject | Compliant cross-post. Read sub rules; post per template. |

### Day +3 to +6

| Day | Action |
|---|---|
| +3 | Resume Twitter cadence (1 build-in-public post/day, replies). |
| +4 | Reach out via DM/email to 5 newsletter authors with traction numbers ("we did X in 48h; would you be interested in a guest column / sponsored placement?"). |
| +5 | Substack: "What we shipped in week 1." |
| +6 | Prep Product Hunt launch for day +7 (separate audience event; do NOT skip). |

### Day +7

| Time | Channel | Action |
|---|---|---|
| 6:00am PT | **Product Hunt** | Launch. Separate audience from HN; some overlap but different mechanics. Hunter relationship matters; if no hunter relationship exists, self-launch is fine but ranks lower. |
| 9:00am PT | Twitter/X | Cross-link to PH. Different framing — "Today we're on Product Hunt. Different audience than HN; let's see what they say." |
| 11:00am PT | All | Reply to every PH comment. Same 5-min response time. |

### Day +14

| Action |
|---|
| Substack: "Two weeks in — what's working, what's not, what's next." Concrete numbers (paying, churn, top channel by signups, top channel by paying). |
| Newsletter-author outreach round 2 (now with 2-week traction data). |
| Decision moment: is P6 hit (15 paying)? If yes, scale Twitter cadence + plan v1.0.5. If no, return to concierge-onboarding mode — schedule 10 more manual onboarding calls in week 3. |

### Day +30

| Action |
|---|
| Substack: month 1 retrospective. |
| Decision moment: is P5 hit (25 paying)? If yes, plan v1.0.5 fast-follow + corporate-segment exploration. If no, pivot conversation per design doc. |
| Reach out to 5 podcasts in vertical for guesting. Have specific traction story ready. |
| Begin SEO content cadence: 1 comparison/pricing post per week ("tldrof vs Readless", "tldrof vs Meco", "tldrof pricing 2026", "best newsletter summarizers 2026"). Target Readless's SERP turf with a 12-month patience horizon. |

### Day +60

| Action |
|---|
| Mode-C audience-build sprint 90-day review. Run `/plan-cmo-review` again with launch data. Re-evaluate channel mix; cut what isn't working; double down on what is. |

---

## Channel-specific guidance

### Hacker News specifics

- **Title format:** "Show HN: [product name] – [one-line value prop]" — under 80 chars total
- **Avoid:** "Launched", "Launching", excessive marketing words. HN penalizes clickbait.
- **First comment:** within 30 seconds of post going live, post a comment from the founder account with: link to live demo, 1-2 sentence backstory ("I built this because..."), invitation for feedback. This first-comment serves as the "above the fold" sales pitch on the comment page.
- **Critical: NEVER ask for upvotes.** Voting-ring detection is automatic; asking is grounds for shadowban.
- **Reply within 5 minutes for first 4 hours.** The HN ranking algorithm rewards engagement velocity in the first 4 hours.
- **Pre-written responses to expected comments:**
  - "How is this different from Readless?" → bankruptcy framing + 60s vs 24h + auto-forward helper + structural moat
  - "Just use ChatGPT" → bulk-forward + automated daily + dedup + time-saved math + no copy-paste
  - "Mailbrew was great" → mailbrew got absorbed into Readwise Reader; we're a daily-digest-specific play; if you liked Mailbrew you'll like this
  - "What's the privacy model?" → forwarding architecture, never touch your real inbox, see [link to privacy page]
  - "$9/mo is expensive" → math: 30 newsletters × 3 min each = 90 min/day saved; at $9 the breakeven is ~1.8 hours of your time at $5/hr; we think your time's worth more
  - "Solo founder, what happens if you stop?" → solo founder yes; sustainability via $9/mo recurring; data exportable; honest answer
- **HN front-page math (2026):** ~150-200 points threshold for typical front-page visibility; ~30-50 points for "interesting Show HN" category visibility. Realistic v1.0 target: 30-100 points and 200-500 signups. NOT 500 points and 5,000 signups. Treat expectations accordingly.

### Twitter/X specifics

- **Build-in-public cadence:** daily during build, 3-5x/week post-launch. Visual content (screenshots, GIFs, charts) outperforms text 3-5x for reach.
- **Reply ratio:** 3:1 reply-to-post is the documented engagement-loop ratio for growing accounts.
- **Don't beg:** never ask for retweets or follows directly. Compounding comes from useful content.
- **Quote-tweet pattern:** when launching, quote-tweet your own pinned post about the build, don't just post a fresh tweet. The QT signals continuity.
- **Hashtag use:** `#buildinpublic` for build posts. Skip other hashtags (low signal in 2026).

### LinkedIn specifics

- **Long-form posts** (>300 words) outperform short posts on LinkedIn algorithm.
- **Lead with personal story** ("I left semiconductors to build a consumer product. Here's why and what I'm learning.") — LinkedIn audience rewards personal narrative.
- **Post mid-week** (Tue-Thu, 9am-11am ET) for max reach.
- **Don't link out aggressively** in the first comment — LinkedIn algorithm penalizes external-link posts. Put the link in a comment ("Link in comments") and replyMethods to comments.

### Indie Hackers specifics

- **Long-form launch posts** with revenue/traction numbers do well. Be specific.
- **Don't post until you have data.** Day +2 (24 hours post-HN-launch) is better than day 0.
- **Engage with comments for at least 48 hours.** Community is active and conversation-driven.

### Reddit r/SideProject specifics

- **Read the sticky / wiki rules carefully.** Most subs have weekend-only self-promo, or strict templates.
- **Post template** (typical): tldr, problem statement, what you built, how to try, what you learned, ask for feedback. Don't use marketing copy.
- **Engage with every comment for 24 hours minimum.** Reddit audiences punish drive-by promotion.

### Product Hunt specifics

- **Hunter relationship matters less in 2026** than it did historically; self-launch is fine but ranks lower without an existing PH presence.
- **Launch Tuesday-Thursday** for max community attention.
- **First 4 hours = the entire game.** PH's daily ranking algorithm front-loads early-day upvotes.
- **Reply to every comment within 1 hour.** Same pattern as HN.
- **Have multiple visual assets ready:** product GIF, screenshot, founder photo, logo. PH posts with rich media perform 2-3x better.

---

## Risk callouts (reprised from marketing_plan.md)

| Risk | Pre-launch mitigation | In-launch mitigation |
|---|---|---|
| HN miss / front-page no-show | Multi-channel sequence (this playbook has 4 launch-event channels in 7 days) | Continue with Indie Hackers / r/SideProject / PH per sequence; do not panic; one channel won't make or break v1.0 |
| Readless competitive collision in HN comments | Pre-write 5 response templates above | Paste-ready; be human, not defensive |
| 60-second magic-moment fails under load | CEO A2 Tier 2 + concurrency cap of 5 (already in design); rehearse with 50-email backlog day -7 | Have Sentry alerts firing; rollback playbook in RUNBOOK.md (CEO post-skill-cleanup item 5) |
| Site goes down at launch peak | Vercel auto-scale (CEO/Eng review covered); have Vercel team's emergency support contact handy | Stripe pause-new-subs flag flippable from RUNBOOK.md |
| Twitter cross-post fails to land (no engagement) | Build the audience pre-launch (Mode C sprint) so launch isn't first impression | Don't double-down; let the cross-channel sequence run |
| Founder hits "creative block" or burnout post-launch | Pre-write Substack / IH / PH copy DAY -7, scheduled to publish | Launch day itself is one day; the next 60 days of audience compounding are where the work actually is |

---

## Launch-day checklist (consolidate into RUNBOOK.md per CEO post-skill-cleanup item 5)

- [ ] HN draft posted at 7:00am PT Tuesday
- [ ] Founder first-comment posted within 30 seconds
- [ ] Stripe webhook test passed within last 24h
- [ ] Mailgun MX verified day-of via `dig`
- [ ] Resend SPF/DKIM/DMARC verified green day-of
- [ ] Anthropic Tier 2 confirmed
- [ ] Sentry alerts armed for: zero-digests-6h, Anthropic 429-spike, Stripe webhook failures
- [ ] 5 pre-written HN response templates pasted into a draft file, ready to copy
- [ ] Twitter draft ready for 9am PT post
- [ ] LinkedIn draft ready for 11am PT post
- [ ] Personal-network email ready for 9am PT blast
- [ ] Indie Hackers draft ready for day +2 9am PT
- [ ] r/SideProject draft ready for day +2 1pm PT
- [ ] Product Hunt draft + assets ready for day +7 6am PT
- [ ] RUNBOOK.md printed (or ALWAYS-ON tab open)
- [ ] Founder full sleep night before
- [ ] Caffeine on hand
- [ ] No code changes day-of (production stability > new features)
