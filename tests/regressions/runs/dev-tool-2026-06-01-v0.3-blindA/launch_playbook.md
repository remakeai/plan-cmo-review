# AuthForge — Launch Playbook

**Status:** Draft v1. Updated when launch-gate signals approached.
**Launch type:** Multi-channel sequenced. NOT a single-HN-shot.
**Launch gate (Section 5a):** signal-driven, not calendar-driven. Soft-launch fallback if signals not met.

---

## Launch-gate decision table (run on day 55)

| Signal | Threshold | On day 55? | Decision |
|---|---|---|---|
| Concierge-onboarded ICP-A users reporting dependence after 14 days | ≥5 | ___ / 5 | If <5 → SOFT launch only |
| Organic GitHub stars (blog/SEO sources, not gamed) | ≥250 | ___ / 250 | If <250 → SOFT launch only |
| Integration tutorials live AND ranking on long-tail queries | ≥8 live, ≥3 ranking | ___ / 8 | If <8 live → SOFT launch only |
| Named adopters with logos in README | ≥5 | ___ / 5 | If <5 → SOFT launch only |

**Hard launch:** all 4 gates met → execute sequence below.
**Soft launch:** 3+ gates short → OSS-only release on day 60, NO HN moment, build to gates and re-evaluate at day 90.

---

## T-30 to T-1 (pre-launch warmup)

### T-30 days
- Tutorial cadence continues (2/wk per Section 4 cadence)
- Founder Twitter cadence: 3 threads/wk
- Discord open, founder shows up Wed 4-5pm PT
- Named-adopter outreach: 25 cold emails sent, target 10 confirmed by T-14
- Hunter recruitment: identify Product Hunt hunter for T+7 launch (target: ~4-5 hunters with track record in dev tools)

### T-14 days
- Personal email to 100-person VIP list (ex-Stripe, YC peers, blog newsletter VIPs): "Launching AuthForge in 2 weeks. Want early access + opinion?"
- Target: 20-30 responses; 10 give pre-launch feedback that informs README

### T-7 days
- Twitter build-in-public thread previewing launch (no link to product yet — tease)
- Newsletter: "Why I built AuthForge — launching in a week"
- Discord pinned message: "Launch on [date]. Be ready."

### T-3 days
- GitHub v1.0.0 tag cut. Release notes are technical, honest, name what's beta
- README finalized with 5+ named-adopter logos
- Show HN copy finalized (template in main plan; tonal review by 2 dev-Twitter friends)
- Show HN post-time selected: **Tuesday 6:30am PT** (HN best practice — early Pacific = midday Eastern + early Europe wakes up = sustained engagement through US workday)

---

## Day 0 (launch day) — hour-by-hour

| Time (PT) | Channel | Action | Risk |
|---|---|---|---|
| 6:00am | Pre-launch | Coffee. Final HN-copy review. | — |
| 6:30am | **Hacker News** | Submit Show HN. Title: "Show HN: AuthForge — TypeScript-first framework-agnostic auth SDK + optional hosted tier" | If buried in <2hr, launch is severely impaired |
| 6:32am | Internal | Send heads-up to 5 trusted dev-Twitter friends with HN link (they may or may not vote — never ASK for a vote, that's against HN guidelines) | Low |
| 6:45am | **HN comments** | Founder lives in comments — engineer-tone, honest, never defensive. Link to GitHub repo (not landing page) when relevant. | Critical for retention on front page |
| 8:30am | **Twitter** | Thread linking HN discussion (NOT direct link to landing page) — pulls Twitter audience into HN | Medium |
| 9:00am | **Newsletter** | "AuthForge is live — HN discussion here" (drives newsletter subs into HN) | Low |
| 10:30am | **r/programming** | Compliant cross-post. Title MUST match HN tone. Follow self-promo rules (founder must have prior comment history). | Ban risk if rules ignored |
| 10:30am | **r/typescript** | Cross-post (different subreddit, no duplicate-content sin) | Low |
| 10:30am | **r/golang** | Cross-post (if Go SDK is shipped) | Low |
| 12:30pm | **lobste.rs** | Submit ONLY IF invited by an existing user OR if founder has lobste.rs history. lobste.rs is hostile to marketing — DO NOT submit if uncertain. | High burn risk |
| 2:30pm | **Discord** | "We're live" announcement; founder camps in #general for next 12 hours | Low |
| 5:00pm | **HN comments** | Continue answering — by end of US workday, HN front-page momentum is decided | Critical |
| 8:00pm | **Retrospective draft** | Founder logs what worked / what didn't in private journal for newsletter post tomorrow | Low |

### What to NOT do on day 0

- Do NOT email a "we launched!" blast to the full newsletter list — the launch is on HN; the newsletter blast is day +1 with traction context.
- Do NOT submit to Product Hunt on day 0 — PH is a separate event at T+7.
- Do NOT submit to IndieHackers on day 0 — different audience, lower priority, day +2.
- Do NOT respond defensively to HN criticism. Acknowledge, engage technically, never argue.
- Do NOT use the word "revolutionary," "best-in-class," "game-changing," "enterprise-grade," "seamless," "robust," "world-class" anywhere on day 0. (Per Section 3 dev-tool tonal rule.)

---

## Day +1 to Day +7

| Day | Action |
|---|---|
| +1 | Newsletter retrospective: "24 hours post-launch — what's working, what's broken, what's next." Honest. Include the HN comment criticisms. |
| +1 | IndieHackers cross-post |
| +2 | Discord office hours — extended, founder live 2 hours |
| +3 | Twitter: respond to every quote-tweet of the launch (high-leverage) |
| +4 | Pitch 3 podcasts (target: SED, JS Party, Changelog) referencing launch traction |
| +5 | Update GitHub README with launch testimonials from concierge-onboarded users |
| +7 | **Product Hunt launch** — recruit hunter pre-launch, schedule for Tuesday 12:01am PT |

---

## Day +8 to Day +30

| Week | Action |
|---|---|
| +2 | Podcast recordings (booked at day 30-60 pre-launch are now happening) |
| +2 | Newsletter: "Week 2 retrospective + first paying customer story" |
| +3 | Conference talk pitch (if applicable: Next.js Conf, ViteConf, JSConf) for ~6 months out |
| +4 | "30-day post-launch" blog post with traction numbers, lessons, next-90-day roadmap |

---

## Risk callouts (recap from Section 5)

- **HN miss:** mitigated by warm Twitter + newsletter + Discord; survivable, not catastrophic.
- **lobste.rs ban / r/programming removal:** founder must have comment history; if not, skip these channels.
- **BetterAuth counter-launch:** they may publish a "we already do that" thread within 24hr. Mitigation: honest deltas in own launch copy (drafted in main plan).
- **Single-channel concentration:** mitigated by multi-channel sequence.
- **Founder burnout in HN comments:** mitigated by pre-launch rehearsal of top 10 expected objections (see `icp.md` objection-handling).

---

## Post-launch handoff to growth (day +30 onward)

- Switch from launch-mode dashboard (hourly) → weekly dashboard (Section 8)
- Re-run `/plan-cmo-review` at day +60 to evaluate progress + adjust
- Decide on hosted-tier expansion (or deferral per outside-voice reframe in main plan)
