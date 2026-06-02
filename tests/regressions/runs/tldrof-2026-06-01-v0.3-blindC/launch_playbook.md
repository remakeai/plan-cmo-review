# Launch Playbook — TLDR-of-TLDRs (tldrof.com)

**Run:** tldrof-2026-06-01-v0.3-blindC
**Date:** 2026-06-01
**Assumes:** PMF gate alternative recommended (concierge cohort + Vohra survey BEFORE public launch). Calendar version provided as fallback.

---

## Launch GATE — pick one

### Option A (RECOMMENDED): PMF-signal gated

- Day 0-13 of "launch window": concierge cohort. Founder personally onboards 10-20 paying via 15-min Zoom each.
- Day 14: run Vohra "very disappointed" survey on concierge cohort.
  - <30% very disappointed → HOLD public launch. Iterate product. Repeat survey weekly.
  - 30-40% → proceed to public launch sequence below at day 14.
  - ≥40% → strong signal; proceed aggressively.
- Day 14+: public launch sequence (timeline below shifts to day 14 = "Day 0 public")

### Option B (FALLBACK if founder insists on calendar): Calendar gated

- Day 0 = ~build day 22 per CEO review locked decision.
- Public launch sequence runs immediately.
- Risk: launching whether or not the product is retention-strong. If concierge cohort isn't run AT ALL, no PMF evidence exists before public launch.

---

## Pre-launch sequence (Day -30 to Day -1)

### Day -30 to -7 (audience-build sprint per Section 4)

**Weekly cadence:**
- Mon: LinkedIn long-form post #1 of week
- Tue: 5 personal outreach emails to M6 named list + warm referrals
- Wed: 1 community engagement (r/ProductManagement / r/M365 / etc.) — pure value add
- Thu: LinkedIn long-form post #2 of week
- Fri: Concierge intake calls (15 min each) with anyone who responded to Tue outreach

**By day -7:** should have ≥6 LinkedIn posts published, ≥30 outreach emails sent, ≥3 paying users from concierge, ≥1 newsletter sponsorship booked for Day +14.

### Day -7

- **Email to all 30-50 named contacts:** "Launching publicly Tuesday. Could you (a) share with 2 people who'd benefit, (b) post a 1-line review on Twitter/LinkedIn day-of if you've found it useful?"
- Pre-draft Show HN copy; submit to 2-3 trusted readers for tonal review
- Pre-draft LinkedIn launch post; submit for tonal review
- Confirm sponsorship placement is locked for Day +14

### Day -3

- LinkedIn long-form: "I've been quietly building tldrof.com for ~6 weeks; launching publicly Tuesday. Here's what I learned about inbox overload from my first 10 users." Includes 1-2 named quotes from concierge cohort (with permission).
- Send to all concierge users: "Launching Tuesday. The post will be public Tuesday morning. If you have a moment Tuesday to amplify, here's what would help: [share LI post / comment on HN / post quick review]."

### Day -2

- Final ping to network with launch links pre-filled (LinkedIn post URL, Show HN URL placeholder)
- Verify all production systems green (Mailgun, Resend, Stripe, Supabase)
- Verify SPF/DKIM/DMARC propagation (per CEO post-skill-cleanup item 1)
- Verify Resend deliverability to Gmail + Outlook + Proton test addresses
- Write Day 0 monitoring dashboard query

### Day -1

- Sleep. Eat. Don't tinker.
- Pre-schedule Show HN post for 8am PT Tuesday (most active US/EU overlap).

---

## Day 0 — Hour-by-hour

### 6:30am PT — wake / coffee / final systems check

- Vercel dashboard green
- Sentry no overnight alerts
- Stripe webhook handlers responsive
- Mailgun MX healthy

### 7:45am PT — pre-fire

- Pull up Show HN draft one final time
- Pull up LinkedIn draft
- Open monitoring dashboard
- Get someone (partner / friend) to text you "go" when ready

### 8:00am PT — Show HN POST

**Title format:** `Show HN: TLDRof – Forward newsletters, get a digest in 60 seconds`

**Body copy (~150-300 words, dev-tool tonal register per skill Section 3):**

```
Hi HN — I built tldrof.com to deal with my own newsletter pile.

You sign up, get a unique forwarding address (you-abc123@m.tldrof.com),
forward whatever's piled up in your inbox, and 60 seconds later you
see a deduped digest in your browser with how many minutes you saved.

Architecture:
- Mailgun inbound on m.tldrof.com → webhook → Postgres
- Two Claude calls per digest: parallel per-newsletter summary, then
  one cross-newsletter dedup + attribution pass
- Supabase Realtime CDC pushes summaries to the /onboard page as
  they finish; first digest renders in 60s, full backlog of 50+
  completes in ~2 min
- Magic-link auth (no passwords); $14/mo or $108/yr

Comparisons:
- Readless.app ($4.90/mo) is the closest comp. They're cheaper and
  have an RSS option I don't have. Their first digest takes ~24h;
  mine renders in 60s. They don't have a bulk-backlog flow; that's
  the main use case I built for.
- Meco is a different shape entirely (Gmail OAuth + reader app).
- The forwarding architecture works with any email platform; doesn't
  need OAuth into your inbox.

Roadmap honest: v1.0 ships Gmail auto-forward-helper today; Outlook
/ Apple Mail / Proton / corporate-IMAP in v1.0.5 (~4 weeks).

Would love feedback, especially on: dedup quality (try forwarding a
day of dev TLDRs and see), and any edge cases on the magic-moment
render. The first 50 HN signups get founder concierge onboarding
(15 min Zoom) if you want it.

Code: [link to repo if open-source]
Site: https://tldrof.com
```

**Post-submit:** check HN within 5 min for "new" page rank; if it lands "new" page, comment within 15 min answering an early question to keep visibility.

### 8:05am PT — LinkedIn long-form post

**Tonal register: builder-for-knowledge-workers, NOT dev-for-dev.**

Different copy from HN post. Lead with Priya-cohort lived experience:

```
Three weeks ago I was at 4,300 unread newsletters and decided to
declare inbox bankruptcy. I've tried this before — unsubscribed
hard, switched to a reader app, tried Notion AI. None of it stuck.

Here's what I built instead:

[brief story]

Today is launch day. tldrof.com is live. $14/mo, $108/yr, 7-day trial.

First 50 LinkedIn folks who try it get me personally onboarding
them — 15 minute Zoom, I'll set up your forwarding rules and walk
you through your first digest. DM me here or sign up and reply
"LinkedIn concierge" in the welcome email.

Three things I learned building this:
1. [insight 1]
2. [insight 2]
3. [insight 3]

If you've also been wrestling with newsletter overload, would
love your feedback.
```

### 8:10am PT — Notify concierge cohort

- Email to all paid concierge users: "Launch is live. HN: [link]. LinkedIn: [link]. Any amplification would mean the world."
- Wait for organic ripple; do NOT call them and demand it.

### 8:30am-12pm PT — HN babysit + LinkedIn reply

- Reply to EVERY HN comment within 15 minutes. Honest, technical, no marketing-speak. Acknowledge where Readless is better.
- Reply to every LinkedIn comment within 30 minutes.
- DO NOT post the HN link on Twitter yet; wait for HN traction first to avoid duplicate-content suppression.

### 12pm-2pm PT — assess HN trajectory

- If front page (top 30): keep babysitting through evening US, Asia morning
- If second page (rank 30-90): one quality reply to keep visibility; pivot focus to LinkedIn
- If buried (<page 3): accept; HN is one of four channels, don't double down

### 2pm PT — Twitter thread

If HN is doing OK (top 100), post X thread:
```
Today I launched tldrof.com — 60-second digest of your
newsletter pile.

Show HN here: [link]
LinkedIn write-up: [link]

Built it because Readless didn't have a magic moment and I
needed one. [thread continues with build-in-public details]
```

If HN is buried, X thread anyway but soft: "Quietly shipping today" framing.

### 4pm-6pm PT — late-day amplification

- Personal text/DM to 5 closest contacts: "Live today; any amplification welcome"
- Reply to anyone tagging tldrof on X / LinkedIn / HN

### Evening — review

- Tally: signups, paying conversions, channel attribution (UTM-tracked)
- Note any objection patterns from HN comments
- Write Day 1 plan based on signal

---

## Day +1 to +7

### Day +1

- IndieHackers cross-post: same body as HN with framing adjusted for IH audience ("Solo founder, here's the build story")
- Reply to all comments on Day 0 channels
- Outreach to any new responders from network amplification

### Day +2

- Reddit cross-posts to compliant subs ONLY:
  - r/productivity (check self-promo rules first; usually allowed with caveats)
  - r/Lenny (small, might not allow)
  - r/M365 (small, might allow if framed helpfully)
  - SKIP r/SideProject (wrong audience)
  - SKIP r/Entrepreneur (wrong audience for the corrected ICP)

### Day +3 to +5

- Pitch 5 podcasts (Lenny's Newsletter podcast, Pragmatic Engineer, Indie Hackers, MicroConf On Air, Mind The Product)
- Continue replying to launch-day comments
- Run first weekly metrics review (filter_setup_rate, trial-to-paid, Vohra)

### Day +5

- Product Hunt launch (separate event)
  - Coordinate with PH hunter (sourced in launch -30 window)
  - Same hour-by-hour discipline as HN but at Pacific midnight (when PH launches happen)

### Day +7

- Send first concierge-cohort weekly check-in: "How was week 1?"
- Identify any churn signal from trial cohort
- Tweet/LinkedIn 1-week milestone post if numbers warrant

---

## Day +8 to +30

### Day +14

- **Newsletter sponsorship placement #1 GOES LIVE.** Track UTMs aggressively. Compare paid-cust-acquired to sponsorship cost; calculate per-paying-CAC.
- Run Vohra "very disappointed" survey on all paying users (cumulative).

### Day +21

- Podcast guest spot #1 (if booked 4 weeks ago)
- Substack/LinkedIn long-form: "Two weeks in — what I'm learning from paying users"

### Day +30

- P5 measurement: ≥25 paying users at $9/$14 mo? Document numbers.
- If yes: write retrospective post, pitch second sponsorship
- If no: do NOT write hype post; conduct cohort-level retro internally before public commentary

---

## Risk callouts

- **HN miss is recoverable.** Concierge + LinkedIn + sponsorship cover.
- **LinkedIn algorithm under-reach on launch day:** comment / DM-amplify manually with first 30 reactions to fight the algorithm.
- **Concierge cohort negative Vohra signal at day 14:** do NOT proceed with sponsorship. Pause. Investigate. Iterate. Cost: ~$5K saved. Value: ~30 days of wasted launch energy avoided.
- **Mailgun outage on launch day:** failover to backup MX (per Eng review D8). Pre-tested in days 13-16.
- **Founder burns out hour-by-hour on Day 0:** scheduled hard stop 6pm PT. Day 0 is not the only day; sustained presence matters more than 14h of launch-day stress.

---

## What's explicitly NOT in this playbook

- Paid ads on launch day — premature
- Influencer partnerships — premature
- B2B enterprise outreach — wrong motion
- Affiliate program — premature
- Press / TechCrunch outreach — low ROI for a $14/mo solo launch
- Video / YouTube launch content — defer to v1.0.5+
- Multiple sponsorships in launch week — concentrate budget on one, evaluate

---

END launch_playbook.md
