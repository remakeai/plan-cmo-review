# Launch Playbook — tldrof.com

Companion artifact to `marketing_plan.md`. Skill: plan-cmo-review v0.2 (Mode B, Section 5).

## Launch architecture: hybrid 2-stage (per Section 5a, supersedes calendar-only gate)

**Stage 1 — Private beta + concierge onboarding (Day 20-22 → Day 35).**
**Stage 2 — Public launch (Day 35-42 if PMF gate hits).**

**PMF gate to Stage 2:**
- Vohra "very disappointed" survey response ≥40% across first ~20 private-beta users
- AND `filter_setup_rate_48h` ≥30% on Gmail-enabled users
- AND ≥3 unprompted word-of-mouth referrals from Stage 1 cohort

If gate misses: pivot conversation (re-design, re-position, re-target) before public exposure.

---

## Stage 1 — Private beta (Day 20-22 → Day 35)

### Goal
Validate PMF on 15-25 actual users; build a small testimonial/word-of-mouth seed before public exposure.

### Cohort source
- 10-person M6 list (per `marketing_plan.md` Section M6).
- ~10-15 additional invitees from Audience-Build Sprint Days 1-15 outreach.
- Total: 20-25 private-beta seats.

### Onboarding mechanic — CONCIERGE (per Superhuman precedent)
- Each user gets a 15-min 1:1 Zoom call with founder.
- Founder walks through: generate forwarding address, set up Gmail auto-forward filter, forward their backlog live on the call, see 60-second magic moment together, troubleshoot any issues.
- Call ends with founder asking: "Would you be willing to do a 1-week check-in and a 'very disappointed' survey at Day 7?"
- All Yes (which they will, given the concierge experience).

### Per-user lifecycle
| Day from signup | Founder action |
|---|---|
| Day 0 | 15-min concierge onboarding Zoom call |
| Day 1-6 | Watch their delivery; reach out personally if first digest is rough |
| Day 7 | DM with Vohra survey: "On a scale, how would you feel if you couldn't use tldrof tomorrow? [Very disappointed / Somewhat disappointed / Not disappointed]" + qualitative "what's missing" |
| Day 14 | If Very Disappointed → ask for testimonial + ask if they'd refer 1-2 friends |
| Day 14 | If Not Disappointed → personal follow-up: "what would have to change?" |

### Measurement during Stage 1
- Vohra % (live dashboard).
- filter_setup_rate_48h per cohort (per CEO post-skill cleanup item 2).
- Word-of-mouth referrals (track via UTM + asking).
- Retention day-7 / day-14.
- Trial-to-paid % (CC-required trial per Section 6 Option B recommendation).

### Stage 1 risks + mitigation
- **Founder time:** ~5-7.5 hr/wk concierge for 2 weeks. Reduce build scope (defer picker fallback to v1.0.5) if needed.
- **Cohort bias:** M6 list = founder's network = friendly cohort. Mitigation: include 5-7 cold-DM converts (less friendly, more honest signal).
- **Survey sample size:** n=20-25 is thin. Mitigation: weight the qualitative signal heavily; don't over-index on % alone.

---

## Stage 2 — Public launch (Day 35-42 assuming PMF gate hits)

### Launch posture commitment (per Premise-Level Findings recommendation #1)

**Pick Maya-cohort launch. M365/corporate-Karen claim is OUT of v1.0 launch copy.**
The forwarding architecture's structural coverage advantage stays in the doc (technical truth), but landing-page headline + Show HN title + Substack launch issue all target Maya. Karen is v1.0.5+ once segment-validated.

### Multi-channel sequence (force ≥3 channels; sequenced not simultaneous)

| Day | Time (US ET) | Channel | Specific action | Risk callout |
|---|---|---|---|---|
| **T-3** | Fri 9am | X | Build-in-public thread: "Launching Tuesday — here's the demo" (60s screen recording of bankruptcy moment) | Set thread up to convert to launch CTA on T-day |
| **T-1** | Mon 10am | Personal email | Send to ~50 known contacts with private-beta testimonials embedded | "Soft pre-announce; ready for your friends Tue" |
| **T-1** | Mon 5pm | TLDR / Bensbites / Pragmatic Engineer press kit | Pitch as meta-story: "newsletter for people drowning in newsletters" | 0-1/3 likely to bite; OK |
| **T-day** | Mon 7pm (= Mon 00:00 UTC — per Show HN by the Numbers, optimal slot) | **Show HN** | Headline: **"Show HN: I built TLDR-of-TLDRs because I had 50 unread newsletters"** | Link to landing page + 60s demo embedded in OP comment |
| T + 1hr | Mon 8pm | X | Reply-quote to founder's earlier T-3 thread: "We're live on HN — [link]" | Tag relevant accounts: Lenny, Swyx, Eugene Yan |
| T + 2hr | Mon 9pm | Lenny's Slack | Post in #show-and-tell ONLY IF founder has 3+ weeks of helpful comment history; otherwise defer to T+7d | Channel-destroy risk |
| T + 4hr | Mon 11pm | LinkedIn | Long-form post for the 996 followers (low expectation but compounds; possible amplification from semiconductor friends to wider network) | — |
| **T + 24hr** | Tue 7pm | **IndieHackers** | Cross-post the launch retrospective + cohort numbers from first 24h | Different angle: solo-founder lessons |
| T + 48hr | Wed 7pm | **r/SideProject** | Compliant post (no link in title; description matches rules) | Mod risk; have backup channel ready |
| T + 72hr | Thu 9am | **Substack** | "Launched on HN — here's what happened" issue (compounds founder narrative AND drives Substack subscribers to product) | Honest numbers required |
| T + 7d | Mon 7pm | **Product Hunt** | Separate launch event (different audience overlap); coordinate with a PH hunter ahead of time | 0-1/1 hunters available; have backup PR plan |
| T + 10d | Various | **Podcast outreach** | Pitch 5 podcasts with Day 10 traction numbers + private-beta testimonials | Aim 1/5 conversion |
| T + 14d | Fri 9am | **Substack** | "14 days of tldrof: 15 paying users hit / missed, here's what we learned" | Per P6 success criterion |
| T + 30d | Fri 9am | **Substack + X** | Cohort metrics post with honest day-30 retention | Per P5 success criterion |

### Day-0 contingency plan

**If HN miss (no traction by Hour 4):**
- Don't panic-post elsewhere yet. HN's 48-hour half-life means a slow start CAN recover by Tuesday morning.
- IndieHackers + LinkedIn + Substack carry the launch on Day 1 if HN is dead.
- Personal email amplification (T-1 list) drives signups regardless of HN.

**If HN hit (front page top 30):**
- Hold all other channels for 24 hours to maximize HN concentration of traffic.
- Founder personally responds to EVERY HN comment within 2 hours (Vohra-precedent: founder presence is part of the product story).
- Aim for ≥100 signups Day 0; ≥10 paying converts in Week 1.

**If HN hit then Sundayed (top traffic decays fast):**
- Roll into IH on Day 1 with retrospective.
- Lenny's post becomes Day 7 (after gathering numbers).

### Launch-day founder schedule

| Time (ET) | Action |
|---|---|
| Mon 6pm | Final ops check (Mailgun + Anthropic + Stripe + Supabase all green; warmup-cron health). |
| Mon 6:30pm | Post-prep tweet draft, IH draft, LinkedIn draft loaded into Buffer / drafts. |
| Mon 7pm | Post Show HN. |
| Mon 7-8pm | Watch HN dashboard. Respond to first comments within 5 min. |
| Mon 8pm | Post X amplification. |
| Mon 9pm | Decide on Lenny's post (yes if helpful-comment history; otherwise defer). |
| Mon 11pm | LinkedIn post. |
| Mon 11pm-1am | Continue HN comment response; respond to every signup-day-0 personally with a thank-you. |
| Tue 6am | Wake up; check overnight signups; respond to any waiting DMs. |
| Tue 9am | Decide IH cross-post timing. |
| Tue 5pm | First full-day metric review; adjust Day 2 plan. |

### Risk callouts

- **HN miss = single-channel-launch failure** if not mitigated. Mitigation: multi-channel sequence per above. Even if HN is 5 upvotes, IH + LinkedIn + Substack + personal-email + cold-DM-driven traffic should produce 30-60 signups Day 0.
- **Lenny's slack posting too early** (channel-destroy risk). Mitigation: 3-week-helpful-comment-history rule; if not met, defer to T+7d.
- **Founder burnout during launch week**. Mitigation: build-scope cuts during private beta to free Stage 2 energy.
- **PMF gate misses but founder ships publicly anyway** (impatience risk). Mitigation: explicit PMF gate criteria written in advance; founder pre-commits to honoring the gate before private beta starts.
- **Pricing-decision-not-made by launch copy time** (causes scrambled landing page). Mitigation: founder commits to trial mechanic decision by Day 7 of this plan.

---

## What's NOT in this playbook (deliberate exclusions)

- **Paid acquisition.** Not v1.0. Reconsider v1.0.5 if Stage 2 surfaces specific high-CAC-tolerable channels.
- **Influencer / creator partnerships.** Not v1.0. Build relationships during Stage 1; activate v1.0.5+.
- **Affiliate program.** v1.0.5+ (need 50+ paying users + retention data before recruiting affiliates).
- **Referral mechanic in-product.** v1.0.5+ (eng work).
- **Corporate/Karen segment outreach.** v1.0.5+ (segment not yet validated; product not yet tuned).
- **YouTube channel.** v1.0.5+ if founder narrative is strong enough to warrant.

---

## Success criteria (mapped to existing P5/P6 + new PMF gate)

| Stage | Day | Criterion | Failure mode |
|---|---|---|---|
| Stage 1 PMF | Day 30 | Vohra ≥40% + filter_setup_rate_48h ≥30% + ≥3 word-of-mouth referrals | Pivot before public launch |
| Stage 2 P6 | Day 35+14 = Day 49 | 15 paying conversions in first 14 days post-public-launch | v1 has failed per P6 |
| Stage 2 P5 | Day 35+30 = Day 65 | 25 paying users at $9/mo | v1 has failed per P5; pivot starts |
| Long-term | Day 35+120 = Day 155 | 100+ paying + v2 smoke-test conditions | Strategic Ladder Rung 2 earnable |

Note: Day numbers shift if Stage 1 misses gate and re-runs OR if launch slips.
