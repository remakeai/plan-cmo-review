# Marketing Plan — TLDR-of-TLDRs (tldrof.com)

**Skill:** plan-cmo-review v0.3.0
**Run:** tldrof-2026-06-01-v0.3-blindC
**Date:** 2026-06-01
**Status:** FINAL

---

## Founder situation snapshot

- Founder: ex-Micron engineer, solo, California, technical background
- First consumer product. No prior shipped consumer wins. No B2C marketing track record
- Audience surface area (declared at run start):
  - LinkedIn: ~996 followers, semiconductor/hardware professionals (CATEGORY-MISALIGNED to TLDR-of-TLDRs ICP)
  - Substack: ~11 subscribers
  - Twitter/X: no relevant following for this product
  - No prior shipped consumer products
- Product dogfooded on technical newsletters: TLDR, AlphaSignal, dev-focused sends
- Design doc target ICP (per P2/P3): inbox-overloaded knowledge workers, HN-cohort, plus M365/corporate-locked-out users
- Locked launch plan in design doc: Show HN on calendar day 18 (now ~20-22), $9/mo, 7-day free trial, Stripe Checkout

**Evidence-that-overrides-default check:** none apply.
- No prior ≥$10K MRR consumer/B2B product
- No published consumer-marketing track record (Substack at 11 subs)
- ICP-aligned audience surface area ~ zero (LinkedIn is wrong category; Substack subs too few; no Twitter)
- No documented prior failed launches with retro

**Verdict: Working under the marketing-naive default. Premise-challenge in Step 0.5 is load-bearing. Default refusal posture is "challenge" not "accept."**

---

# PREMISE-LEVEL FINDINGS BLOCK (top of doc, highest-leverage section)

Four of the five M0a-M0e premise audits FAIL. The marketing-naive default is fully load-bearing here. **The marketing plan that follows is not optimization within the design doc's framing; it is a reframing of the design doc's marketing assumptions.** If only one finding is acted on, make it M0e (dogfood/buyer audience mismatch).

| # | Premise | Verdict | Headline implication |
|---|---|---|---|
| M0a | Show HN is the right launch platform | **FAILS** | HN is the founder's familiar surface, not the paying ICP's surface for two of the three ICP segments. Move HN from "the launch" to "one of three launch channels" and underweight it. |
| M0b | No canonical-success comparable was named | **FAILS** | Design doc anchors on Readless (direct competitor losing on positioning) instead of Superhuman / Readwise (canonical successes at this motion class). Adopt concierge + bootstrapped-product-led playbook. |
| M0c | All in-scope features serve the paying ICP | **FAILS** | At least 3 anti-features identified: (1) self-serve magic-link signup with 7-day trial for a trust-led ICP, (2) $9/mo "match the floor" pricing that signals commodity to time-poor segment, (3) Strategic-Ladder Rung 2-4 architecture cost (blueprints join table, per-blueprint prefs, optionality-preserving DB) shaping v1 narrative and surface area. |
| M0d | The free-trial mechanic validates the paying ICP | **FAILS** | 7-day no-CC trial selects for time-rich free-shoppers (HN comparison-trial cohort); time-poor/money-rich M365 corporate-locked-out segment buys on trust, not on trial-shopping. The validation cohort and the paying cohort are different humans. |
| M0e | Dogfooding on dev newsletters matches the paying ICP | **FAILS, catastrophically** | Product tuned on dev-tech newsletters (TLDR, AlphaSignal). Paying ICP per design doc P4 includes lawyers, finance, healthcare, government, agency operators on custom-domain email. First-cohort dogfood entrenches the wrong audience signature: dedup of "AI news" vs dedup of "industry digests + client news + regulatory alerts" are different products. |

**Required fixes before launch (load-bearing, BOTH pivots per anti-pattern #14):**

1. **Pivot the TARGET audience** in landing copy, ICP doc, and first-cohort outreach AWAY from "TLDR / AlphaSignal subscribers" and TOWARD a *specific* non-technical segment the design doc's structural-coverage moat actually serves. Recommended: **M365 corporate-knowledge-worker segment with newsletter overload AND ≥1 paid-account-locked subscription they cannot repoint** (because that's exactly the segment Readless cannot serve and where the $9 price doesn't look expensive). NOT "indie hackers" or "HN-cohort."
2. **Pivot the dogfood subjects** to include 2 weeks of buyer-aligned inputs before launch. Founder forwards: industry-vertical newsletters in 2-3 named verticals (e.g., Stratechery + Axios Pro Rata for finance/strategy adjacency, Morning Brew + The Information for generalist exec, plus one vertical: Lenny's + IndieHackers for ops, OR The Hustle + Morning Brew for marketing-exec adjacency). Tune the dedup prompt against THIS mix. NOT just dev newsletters.
3. Concrete fix: M0e is **not** "defer the paying ICP to v1.0.5"; that preserves the mismatch. M0e is **change who you build for THIS week** and **change what you forward to your test address THIS week**.

The rest of the plan derives from these fixes. Sections below carry the load.

---

## Step 0 — Pre-review system audit

### Existing context found

- Design doc is unusually well-developed (~1500 lines, four founder editorial passes, CEO review + Eng review locked decisions, Strategic Ladder, full implementation specs)
- Product wedge is clear: "inbox-bankruptcy" digest with forwarding-address architecture
- Pricing locked at $9/mo with 7-day trial
- Launch plan in design doc: Show HN on day 20-22, cross-post to X / founder's network, no paid acquisition
- Distribution Plan section is the WEAKEST part of an otherwise strong doc — about 30 lines vs hundreds on engineering specs. **The design doc itself proves the build-it-and-they-will-come thesis: distribution is a downstream concern.** That gap is what this skill exists to catch.

### Founder audience audit (numeric, real surfaces)

| Surface | Count | ICP-aligned? | Useful for v1 launch? |
|---|---|---|---|
| LinkedIn | ~996 | NO — semiconductor / hardware professionals | Marginal. ~5-15 might be interested as overworked white-collar pros; no leverage on the core HN-cohort or M365 segments. |
| Substack | ~11 | Unknown — too few to matter | Effectively zero. |
| Twitter/X | ~0 for this product | NO | Zero. |
| Prior shipped consumer products | 0 | n/a | Zero. |
| Personal blog readership | none stated | n/a | Zero. |
| Existing communities (founder is "known in") | none stated | n/a | Zero. |
| **Effective ICP-aligned audience for tldrof.com** | **~0-15** | | Functionally zero. |

**This is a Mode-C-trigger profile by audience count alone.** See Step 0B for mode-selection logic and the v0.3 tie-breaker.

### Competitive landscape (web-search verified)

See Section 1 below for the full table. Key finding from Step 0 search pass: **Readless.app already exists** as a direct competitor at the $4.90/mo price point with the same forwarding-architecture pattern. Meco exists at $35/year with Gmail-OAuth model. Both already have traction; the design doc treats Readless as confirmation that the market is real (correct) and the founder editorial pass 4 correctly identified the bankruptcy / repointing-impossible wedge against Readless (also correct).

What the design doc MISSES from competitive analysis: **the canonical-success comparables.** Superhuman ($30/mo, $825M acquisition), Readwise ($10-13/mo, ~$14M ARR, bootstrapped, 4M users). Both are the proof-of-playbook for this motion class. The design doc never references them.

---

## Step 0.5 — Premise audit (5 questions, M0a-M0e)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong hypothesis |
|---|---|---|---|
| 1 | Launch on Show HN | P2 / Distribution Plan / Approach C day 18 | HN audience overlaps founders + dev-tool buyers, not the M365-corporate-locked-out segment the moat actually serves. Lottery on the segment that overlaps; near-zero reach on the segment that doesn't. |
| 2 | Audience class = HN + AI-Twitter cohort | Target User / P2 | Founder's familiar surface ≠ the paying ICP the structural moat enables. |
| 3 | $9/mo price point, 7-day no-CC trial | Constraints / P6 | Anchored on competitor-band thinking (Readless $4.90, Meco $3/mo). Doesn't reflect M365-corporate-locked-out WTP, which is closer to Superhuman's $30 anchor than Readless's $4.90. |
| 4 | Dogfood on dev TLDRs | Approach C days 5-9 | Selects the product's tuning signature for "AI news dedup" not "industry intelligence dedup." Entrenches the wrong audience signature in v1 cohort. |
| 5 | Calendar-driven launch gate (day 18, now ~20-22) | The Assignment / P6 / Approach C | Retention-driven consumer subscription should be PMF-signal-gated (Vohra "very disappointed"), not calendar-gated. Calendar fires whether or not the product is indispensable. |
| 6 | Auto-forward-helper Gmail-only for v1.0 (post-CEO PC2) | CEO Review Locked Decisions | Cuts the M365 corporate segment OUT of v1.0 — the very segment the structural moat is supposed to win. Internal contradiction. |
| 7 | Self-serve onboarding throughout | P3 magic moment / operator-shape watch-item | Concierge onboarding is the canonical-success playbook for premium consumer subscriptions (Superhuman). Watch-item correctly identifies operator-shape RISK; wrongly defaults the resolution to "always self-serve." |

The "likely-wrong" column is the hypothesis the M0 questions test.

---

### M0a — Launch-platform audience-class fit

**Question:** Is Show HN the right audience class for TLDR-of-TLDRs, or just the platform the founder is familiar with?

**Founder's likely-naive answer:** "Show HN is where I hang out, and lots of indie products launch there. AI products especially. I read HN every day. It's the obvious launch venue."

**Web-search verdict:** Show HN is a **CATEGORY ERROR** for the design doc's stated paying ICP per P4 (M365 corporate-locked-out, lawyers, finance, healthcare, government, agency operators). The "Hidden Signal" base-rate cited above [HN audience research](https://www.indiehackers.com/post/my-show-hn-reached-hacker-news-front-page-here-is-how-you-can-do-it-44c73fbdc6) shows HN front-page consumer conversions in the 0.01-0.09% paying range (Basecamp got 14 paying customers from 105K HN visits; Groove got 12 paying customers from 33K visits). [HN works for dev tools, APIs, OSS, CLI tools; weak for consumer apps and non-technical SaaS](https://smollaunch.com/compare/product-hunt-vs-hacker-news).

The HN cohort overlap with TLDR-of-TLDRs is REAL but is a SUBSEGMENT of the actual paying ICP — namely "technical founders / engineers who subscribe to dev TLDRs and have ≥$9/mo discretionary SaaS budget." That subsegment is real but small and is ALSO the segment Readless already serves and the segment most likely to comparison-shop on the $4.90 price.

**Verdict: PREMISE FAILS.** Not "kill HN" — HN remains useful for the dev-newsletter subsegment AND for "indie founder built this" social validation. But HN is **not** "the launch"; it's one channel among three, and it should NOT be channel #1 in priority. The corporate-locked-out segment is unreachable via HN.

**Cascading implications:**
- M2 (discovery path) must show a path that does NOT start with "they see my Show HN post" for the corporate-locked-out segment.
- Section 5 (launch playbook) must put HN at most as one of three sequenced channels, with explicit non-HN channels carrying the corporate segment.
- Section 3 (channels) must rank LinkedIn organic, vertical newsletters, and concierge-outreach above HN for the corporate segment specifically.

---

### M0b — Canonical-success comparable

**Question:** Name the most successful product in this category at this motion class. What did they do that the current plan does NOT?

**Founder's likely-naive answer:** "Readless.app exists at $4.90 — that proves the market. Meco does similar with Gmail OAuth. Refind and Mailbrew tried similar things. So the comparable set is the direct competitors."

**Web-search verdict:** Direct competitors are NOT canonical successes. They are the alternatives. The canonical successes for this motion class (premium consumer subscription with retention-driven economics) are:

- **Superhuman** — $30/mo, $825M Grammarly acquisition Jul 2025, ~$700M ARR. [Mandatory 30-minute one-on-one concierge onboarding for every new user (Vohra did first hundreds personally)](https://review.firstround.com/superhuman-onboarding-playbook/). Single attribute positioning ("speed"). PMF-gate: 40% "very disappointed" Sean Ellis test before public expansion (went from 22% to 58% before unlocking growth).
- **Readwise** — $10-13/mo, $14M ARR (2026), bootstrapped, [explicit choice to NOT raise VC](https://news.ycombinator.com/item?id=19530469). 4M registered users, 3M MAU, 82% YoY growth. Acquisition channels: [strategic partnerships with EdTech companies, content-creator collaborations, expanding developer API ecosystem](https://www.fueler.io/blog/readwise-usage-revenue-valuation-growth-statistics). 30-day free trial then paid (no freemium). [Annual plans renew at 83.4%, 4x weekly subs](https://www.revenuecat.com/state-of-subscription-apps/).
- **(Bonus) Morning Brew / The Hustle** — content-business comparables. Both built audience FIRST, monetized via newsletter ad-revenue THEN subscription, sold for nine figures. The Hustle acquired by HubSpot 2021; Morning Brew acquired by Insider Inc. 2020. Their playbook: audience-first, content-cadence-as-primary-channel, ~5 years to scale.

**Specific deltas between canonical-success playbooks and current plan:**

| Canonical success | What they did | What current plan does | Delta |
|---|---|---|---|
| Superhuman | Concierge onboarded first ~200 users personally | Self-serve magic-link signup, no concierge | Plan **explicitly excludes** concierge under "operator-shape watch-item" |
| Superhuman | Gated public launch on Vohra 40%-very-disappointed | Calendar gate (day ~20-22) | No PMF-signal gate at all |
| Superhuman | $30/mo single price, premium-positioned | $9/mo, race to Readless's $4.90 floor | Plan anchors LOW; canonical success anchored HIGH |
| Readwise | Bootstrapped, 30-day trial, no freemium | $9/mo, 7-day no-CC trial | Trial length wrong + no CC wrong for a retention-driven product |
| Readwise | Annual billing pushed hard | Monthly only at v1.0 | Misses 83.4% annual retention vs ~half monthly |
| Readwise | Content + integrations + creator partnerships | Show HN + X cross-post | No content engine, no partnerships strategy |

**Verdict: PREMISE FAILS.** Design doc has zero canonical-success anchoring. It anchors against Readless (a competitor that may itself be losing) instead of against Superhuman/Readwise (proven precedents at the motion class). This is the #1 reason the marketing plan was thin.

**Cascading implications:**
- Section 5 launch playbook must add: concierge-first cohort option (founder personally onboards first 10-20 paying users) BEFORE any public launch
- Section 6 pricing must propose: hold $9 OR move to $14-19 with explicit premium positioning; do NOT move to Readless's $4.90 floor
- Section 4 audience-build must include: content cadence (Readwise playbook), partnerships approach (something the design doc does not contemplate at all)

---

### M0c — Anti-feature surface

**Question:** Name 2+ in-scope features that contradict stated positioning, trust model, or business model.

**Founder's likely-naive answer:** "Every feature serves the user. I cut a lot already — picker is a fallback, archive scraping is v1.0.5, Playwright automation is v1.1. What's left is core."

**Line-by-line audit of in-scope v1.0 features:**

1. **Self-serve magic-link signup + 7-day no-CC trial.** Positioning claims trust ("we never touch your inbox"), premium-positioned coverage moat (corporate-locked-out segments), and retention-driven business model. Magic-link no-CC self-serve mechanic **serves comparison-shopping HN-cohort users**, NOT corporate-locked-out or trust-led buyers. **ANTI-FEATURE.** Anti-feature relative to the corporate segment. The corporate-segment fix would be: waitlist + concierge intake + invoice-billing option.

2. **$9/mo price point matching the cheaper competitor band.** Positioning per P4 emphasizes corporate / regulated-industry coverage, which is a TRUST-LED segment. Price-band-matching commodity competitors **signals commodity** to exactly the trust-led segment. **ANTI-FEATURE for the structural-moat segment.** The corporate-segment fix would be: $14-19 with explicit positioning vs Readless ("for users with paid newsletters they cannot repoint").

3. **Strategic Ladder Rung 2-4 architecture (blueprints join table, per-blueprint prefs, optionality-preserving DB).** Engineering wise these are ~30-minute decisions that look cheap. But they shape v1 NARRATIVE: founder will be tempted to mention "this is Rung 1 of a four-rung ladder" in launch copy, which **dilutes the wedge.** v1 launch copy must NOT mention Rungs 2-4. (The design doc actually says this — but anti-feature-as-narrative still flags as risk.) **NARRATIVE ANTI-FEATURE risk.** The fix: gag-order on Strategic Ladder for all launch copy. v1 is a standalone product, full stop.

4. **MCP wrapper / read-only API for power users** (mentioned as v1.1 not v1.0, so this one survives — but worth flagging for v1.1 review). Power-user MCP integration serves the developer subsegment, which is precisely the segment Readless already adequately serves at $4.90. If v1.1 adds MCP, it doubles down on the wrong segment.

5. **Auto-forward-helper Gmail-only per CEO PC2.** Internal contradiction: the structural moat in P4 IS the M365 / Outlook / Proton / corporate-IMAP coverage. Cutting auto-forward-helper to Gmail-only for v1.0 cuts THE moat segment OUT of v1.0. Either ship the full multi-client auto-forward in v1.0, or stop claiming corporate-coverage in the launch positioning. **ANTI-FEATURE (or anti-positioning).** Either fix the feature or fix the positioning to match what ships.

**Verdict: PREMISE FAILS.** ≥3 named anti-features. The cleanest single-fix recommendation: keep the Gmail-only auto-forward, but then pivot launch positioning to "Gmail user with newsletter overload" (which is HN-cohort and IH-cohort) rather than "structural coverage of corporate / regulated industries." Be honest about which segment v1.0 actually serves.

**Cascading implications:**
- Section 6 must propose two pricing alternatives (hold $9 OR move to $14-19)
- Section 5 must call out the auto-forward Gmail-only contradiction explicitly
- Section 2 (ICP) must pick ONE segment as v1.0 primary and the other as v1.0.5

---

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the 7-day no-CC trial select for the wrong segment?

**Founder's likely-naive answer:** "7-day trial is standard. We added 7 days specifically because the time-saved math compounds across a week — that's a Vohra-style loss-aversion gate. Industry-standard. Stripe's defaults work."

**Diagnostic mapping:**

| Acquisition mechanic | Segment attracted | Match to corporate-locked-out paying ICP? |
|---|---|---|
| 7-day free trial, no CC required (current plan) | Time-rich comparison shoppers, HN/IH browsers, AI-tool collectors | **NO.** Corporate buyer time-poor, trust-shops, doesn't try-and-cancel. |
| 7-day trial WITH CC at signup | Cautious buyers, casual subscribers | Better than no-CC. Still wrong segment for time-poor corporate. |
| Waitlist + concierge intake | Committed prospects who signal intent by waiting | **YES** for corporate, especially with "request demo" framing. |
| Referral from someone they trust (peer, vertical-publication, ops-lead) | Trust-led buyers | **YES** for corporate. |
| Paid placement in vertical newsletter / publication | Subscribers of that publication | **YES** for corporate IF placement is in a vertical publication. |

**Founder editorial pass 2 actually noted** the 7-day-trial loss-aversion psychology, which is correct REASONING for the trial length, but the WHOLE FRAME assumes a try-and-cancel segment in the first place. For corporate buyers who don't try-and-cancel because they have higher switching cost from trying anything at all, the entire 7-day mechanic is wrong.

**Verdict: PREMISE FAILS** for the corporate segment. For the HN/IH-cohort segment, the 7-day no-CC trial is roughly the right mechanic, so the fix is segment-specific:

- **If v1.0 primary segment = Gmail HN/IH-cohort:** 7-day no-CC trial is fine. Acknowledge: validation cohort = paying cohort for THIS segment.
- **If v1.0 primary segment = corporate-locked-out:** Replace 7-day no-CC trial with concierge intake (founder personally onboards via 15-min Zoom, sets up filter, confirms paid-subscription forwarding works). Charge after intake. Smaller cohort, much higher conversion.

This is why M0c's segment-picking decision is upstream of M0d. Pick the segment first; then pick the mechanic that matches.

**Cascading implications:**
- Section 5 launch playbook must offer a concierge-intake option as an alternative to self-serve trial
- Section 8 metrics must track filter_setup_rate_48h (already added post-CEO) AND concierge-intake-completion-rate if that path is offered
- Section 6 must surface that trial length is segment-dependent, not segment-neutral

---

### M0e — Dogfood audience-class match

**Question:** Is the audience the product is dogfooded on the same audience that will actually buy it?

**Founder's likely-naive answer:** "I'm the user. I subscribe to TLDR, AlphaSignal, dev-focused sends. I am the HN-cohort. The product works for me — that's the strongest validation possible. The forwarding architecture is content-agnostic; any newsletter type works."

**Reality check:**

The design doc itself names two ICP segments:
- Primary v1: HN-cohort + AI-adjacent technical professionals
- Secondary (post-launch): M365 / corporate-locked-out, lawyers, finance, healthcare, government, agency operators

The founder dogfoods on TLDR, AlphaSignal, dev-focused sends — i.e., the FIRST segment ONLY. The structural-moat-justifying SECOND segment is not in the dogfood mix at all.

This matters because:
1. Dedup tuning will be calibrated for "this AI news story appeared in 3 newsletters" patterns. Industry intelligence dedup (e.g., "this M&A appeared in Axios Pro Rata + Term Sheet + The Information") is structurally different — narrower-audience publications, less story overlap, MORE attribution importance, different signal-density patterns.
2. Time-saved math anchored on dev-newsletter word counts. Industry newsletters often have longer-form articles; ratio of "time saved" will look different.
3. Newsletter-source identification heuristics (the lookup table for top ~50 known providers) will be seeded with dev newsletters. The first 10 corporate users will hit unknown-sender fallback constantly.
4. Per-newsletter summarization prompt tuning will favor the linguistic register of dev newsletters (terse, technical, headline-dense). Industry / professional newsletters have different register (longer-form, fewer items, more analysis).
5. The founder's "willing to read every morning" gate from Success Criteria DOES NOT TEST whether a non-technical corporate user would be willing to read every morning. It tests the founder's own gate, which is a different person.

**The deferral failure mode (anti-pattern #14) is alive in this design:** the doc names the corporate segment as "secondary (post-launch expansion)" — i.e., defer the paying-ICP-aligned segment to later, keep the dogfood-aligned segment in v1. This is EXACTLY the deferral pattern M0e refuses.

**Verdict: PREMISE FAILS, CATASTROPHICALLY.** The plan correctly identifies the mismatch (corporate segment as secondary, structural moat as v1 architectural fact) but PRESERVES the mismatch by deferring corporate to post-launch and keeping dev-newsletter dogfood.

**The correct fix is BOTH pivots, this week, before any user-facing feature work continues:**

(a) **Pivot the target audience** in marketing materials, landing copy, ICP doc, first-cohort outreach. Recommended primary: **knowledge workers on Gmail OR M365 with ≥3 newsletter subscriptions including at least one industry/vertical newsletter** (a slightly broader segment than pure corporate-locked-out, because the M0a HN audience-class problem combined with M0c auto-forward Gmail-only contradiction makes "pure corporate-locked-out" too small for v1.0 to validate). Defer pure-corporate-locked-out to v1.0.5 once auto-forward helper supports M365.

(b) **Pivot the dogfood subjects.** Two weeks before launch (today, given the ~20-22 day build is mid-flight), founder MUST add to the test forwarding-address: Morning Brew + Axios AM + Stratechery + Lenny's + one industry-vertical newsletter (e.g., Term Sheet for finance OR The Information Pro for tech-business OR a legal/healthcare/agency-ops newsletter that the founder can credibly read for two weeks). Tune dedup and summarization prompts against THIS mix. Calibrate time-saved math against THIS mix. Seed newsletter-source lookup table against THIS mix.

If only (a) is done, the product ships calibrated wrong. If only (b) is done, the product is calibrated right but launches at the wrong audience. Both pivots are required.

**Cascading implications:**
- M1 (audience reality forcing question) must use the corrected ICP, NOT the dogfood ICP
- Section 2 (ICP spec) is the corrected ICP
- Sections 4, 5 (audience-build + launch playbook) sequence channels to reach the corrected ICP first

---

### Step 0.5 verdict summary

- M0a: FAILS — HN is wrong audience class for corporate segment, lottery for technical subsegment
- M0b: FAILS — no canonical-success anchoring; Superhuman + Readwise playbooks absent
- M0c: FAILS — ≥3 anti-features (self-serve trial, $9 commodity pricing, Gmail-only auto-forward contradicting corporate-coverage claim)
- M0d: FAILS for corporate segment, holds for dev-newsletter HN/IH subsegment — segment-pick determines mechanic
- M0e: FAILS CATASTROPHICALLY — dogfood/buyer mismatch with active deferral pattern

**4/5 fail. Plus one additional finding (auto-forward Gmail-only contradicting corporate-coverage moat) that wraps M0c and M0e together.**

Premise-level findings block at top of doc is the highest-value output of this run. The rest of the plan implements the fixes.

---

## Step 0A — Forcing questions (M1-M7)

These are simulated honest naive answers from a technical founder new to consumer marketing, with skill pushback. Step 0.5 findings flow in.

### M1 — Audience reality

**Question:** Name a specific person who would actively seek out your product. Not "indie hackers." Where do they hang out RIGHT NOW?

**Founder (naive first answer):** *"An indie hacker / AI-adjacent engineer / founder who reads TLDR and AlphaSignal and is drowning in newsletters."*

**Skill pushback:** That's a demographic category, not a person. And per M0e, that's the dogfood-aligned audience, not necessarily the paying ICP. Try again, named or composite, with 5 specific attributes AND 3 named places they spend attention right now.

**Founder (second answer):** *"Composite: 'Priya, 34, Director of Product at a 200-person fintech in SF. Subscribes to Lenny's, Morning Brew, Stratechery, Axios Pro Rata, The Information, and TLDR AI. Inbox at 3,000+ unread. M365 Outlook locked behind corporate SSO; can't add browser extensions to work email. Has tried Notion AI inbox, gave up. Spends $20/mo on ChatGPT Plus, $10/mo on Notion personal, has expensed Lenny's premium. Currently spends maybe 20 min/day scrolling newsletter previews on her phone during her commute. Reads Lenny's full, skims everything else, archives unread by Friday.'"*

*Places she spends attention right now:* Lenny's Newsletter (Substack), Lenny's podcast, Reforge community (paid), occasionally LinkedIn for PM content, occasional Pragmatic Engineer.

**Skill: ACCEPT.** Five attributes, three named places. Specific enough to do channel work against.

**Note:** "Priya" is a Gmail-or-corporate-email user with ≥3 industry/vertical newsletters. This is the corrected ICP per M0e, and the segment that v1.0 plus v1.0.5 auto-forward expansion can serve.

---

### M2 — Discovery path

**Question:** Walk through how Priya specifically discovers tldrof.com. Minimum 3 steps. Step 1 is NOT "she sees a Show HN post."

**Founder (naive first answer):** *"Show HN hits front page → her engineer husband sends her the link → she signs up."*

**Skill pushback:** That requires (a) Show HN front-page hit (lottery odds), (b) Priya's engineer husband being an HN reader, (c) him remembering to forward to her, (d) her then doing something about it. Each step has <20% probability. Combined < 1%. Try again, with a path that's plausible for THIS persona without HN as a load-bearing step.

**Founder (second answer):** *"Path A — Lenny mentions tldrof.com in a Friday roundup ('what I'm trying this week') → Priya reads Lenny religiously → she clicks → signs up. Path B — A colleague on Slack says 'I've been using this thing to dedupe my newsletters, saved me 30 min/day' → Priya asks for link → signs up. Path C — Sponsored placement in a newsletter she already reads (Morning Brew? Axios Pro Rata?) → click-through → sign up."*

**Skill: ACCEPT** with caveat. Path A requires getting Lenny to mention; this is HARD but possible (sponsorship, hard outreach, or a credible product-led ping). Path B requires existing user base. Path C is paid acquisition the design doc explicitly excludes from v1. Realistic time-to-discovery: weeks to months for organic Path A or B; days for Path C. For the launch window, Path B (referral via existing user) is the only credible one with zero existing audience — which means the **first 10-20 users must come from concierge outreach by the founder**, not via inbound channels.

---

### M3 — Pre-launch audience

**Question:** Show evidence of an audience you already have.

**Founder (honest answer):** *"I have ~996 LinkedIn followers from my Micron days, mostly semiconductor people. ~11 Substack subscribers (started this year, mostly friends). No Twitter following for this product. No prior shipped consumer products. Zero ICP-aligned audience."*

**Skill: ACCEPT** as honest "zero" — which triggers Mode-selection toward Mode-C-territory. The 996 LinkedIn is category-misaligned for tldrof.com (semiconductor ≠ Priya). Use as an additional signal: founder is starting from genuine zero relative to this product's ICP.

---

### M4 — Channel honesty

**Question:** Name ONE distribution channel where you have a credible, demonstrable advantage over a generic founder.

**Founder (naive first answer):** *"I can build it. I'm a strong engineer; I shipped Micron infra at scale. I can ship clean, secure code fast."*

**Skill pushback:** That's product, not distribution. Try again.

**Founder (honest answer):** *"I don't have a distribution advantage. Maybe I can write the engineering side of a 'how we built this' post that the dev-tech audience would find credible — but I have no track record of writing publicly. Honestly, I have zero distribution advantage."*

**Skill: ACCEPT** as honest "I don't have one yet" — which becomes the first work item, not a future-tense aspiration. The first work item is "concierge outreach + content cadence starting today" (Section 4), NOT "wait for inbound after launch."

---

### M5 — Competitor traffic source

**Question:** Where does Readless get its users from?

**Founder (naive first answer):** *"I don't know. I assume Reddit and product-hunt. I'll check before launch."*

**Skill pushback:** "Will check" is not enough. Commit to the research before next session OR provide a real best-guess with evidence path. SimilarWeb is free for top-100K. Backlink scan via Ahrefs free tier. Their content history is public on readless.app/blog.

**Founder (research-pass answer):** *"Quick check: Readless.app blog has dozens of comparison articles (Readless vs Meco, Readless vs Feedly, Readless vs Inoreader, TLDR Newsletter Review, etc.) — they're playing the comparison-SEO playbook. Their long-tail keyword strategy is comparison-rank-or-die. So a major Readless channel = comparison-SEO and tool-roundup SEO. Probably some Reddit / Product Hunt. I'd guess SimilarWeb shows under 50K monthly visitors with the bulk from organic search on comparison terms."*

**Skill: ACCEPT.** Important strategic implication: Readless's primary acquisition channel is SEO via comparison/tool-roundup content. tldrof.com competing on the SAME SEO terms is a long-uphill slog (Readless has the head start AND has been investing in the content). DIFFERENT SEO strategy: target "inbox bankruptcy" and "M365 newsletter manager" and "newsletter dedup for Outlook" long-tail queries Readless does NOT rank for. Section 3 channel rank reflects this.

---

### M6 — First 10 paying customers

**Question:** Name the specific path to your first 10 paying customers.

**Founder (naive first answer):** *"Show HN → 10 sign up → maybe 1-2 convert to paid."*

**Skill pushback:** Show HN conversion rate per the search above runs 0.01-0.09% for consumer SaaS. To get 10 paying from Show HN, you need ~10K-100K visitors. That's a front-page hit with sustained traction. Even if you get it, those are the dev-newsletter segment, not Priya. Try again — named 10 humans you would email tomorrow.

**Founder (second answer):** *"Honestly I'd struggle to name 10 today. Let me try: (1) my ex-Micron product manager who reads industry newsletters, (2) my sister who's in healthcare comms and gets ~15 industry emails/day, (3) two friends from my masters program who are in PM roles, (4) my landlord who runs a small agency, (5-6) two Reforge alumni I know peripherally via LinkedIn, (7) one acquaintance who's a partner at a small VC, (8-10) ... I'd need to ask my network for warm intros."*

**Skill pushback:** Of those 10, how many ARE the corrected ICP (Priya-shaped — knowledge worker, ≥3 newsletters including ≥1 industry)? Probably 5-7. Good enough to start. Two action items: (a) email all 10 by end of THIS week with a concierge-intake offer ("I'm building this, here's the magic moment, I'll personally onboard you, $9/mo or free for 90 days in exchange for weekly feedback") — concierge-intake is the right mechanic per M0d for THIS cohort because trust-shopping. (b) Ask each: "name 2 more people you'd recommend this to" → warm intro chain.

**Skill: ACCEPT** the modified version. First 10 paying = 6-7 from named network + 3-4 from warm referrals. Time-to-10: 2-4 weeks from concierge-outreach start. This is the realistic v1.0 launch cohort — NOT Show HN.

---

### M7 — Time allocation

**Question:** What percentage of pre-launch time are you spending on audience-building vs building?

**Founder (honest answer):** *"Probably 95% building, 5% (or less) audience. I started the Substack but I've written 2 posts in 6 months. I haven't done outreach. The CEO review said to add 2-3 backup channels but I haven't started them yet. I've been heads-down on the Mailgun pipeline."*

**Skill: REJECT.** 5% on audience for a founder at zero ICP-aligned audience is incompatible with "I want 15 paying within 14 days of launch" (P6) or 25 paying within 30 days (P5). The build window is 20-22 days remaining; with current ratio that's ~1 day on audience total. P6 and P5 are math-impossible without redirecting time NOW.

**Required reallocation:**
- ≥30% on audience-building starting today
- Named activities: (1) concierge outreach to the 10 from M6 this week, (2) draft 3 substantive blog/LinkedIn posts about inbox-overload (NOT product-launch hype), (3) get on a podcast guest list (pitch 5 Pragmatic Engineer adjacent / Lenny's adjacent shows), (4) seed 2-3 Reddit accounts in r/M365 / r/ProductManagement / r/sysadmin with helpful answers (NOT self-promo) for credibility-building 4 weeks pre-launch
- ≥30% on audience = ~6-7 of the remaining 20-22 build days. Yes, this means the calendar slips. See M0a/M0b: calendar gate is the wrong gate anyway. Slip the launch by a week to fund the audience work.

---

### Step 0A summary

All 7 questions answered. Notable gaps:
- M3: zero ICP-aligned audience (load-bearing)
- M4: zero distribution advantage (load-bearing)
- M5: comp uses SEO comparison content; tldrof.com cannot win that game; must differentiate
- M6: first 10 paying ≠ Show HN; come from concierge-outreach to named network
- M7: time allocation currently wrong; redirect 30%+ to audience starting today

---

## Step 0B — Mode selection

**Audience size:** ~0-15 ICP-aligned. Triggers Mode C territory.

**ICP alignment of existing audience:** Effectively zero. LinkedIn 996 is wrong category. Substack 11 is too few. No Twitter. **Both criteria for Mode C are met.**

**Mode A vs Mode C tie-breaker (v0.3 load-bearing):**
- Is the founder mid-build with a hard launch date? **YES — 20-22 day build, mid-flight, founder has committed to launch within ~3-4 weeks.**
- Is the audience small OR ICP-misaligned? **BOTH — small AND misaligned.**
- Tie-breaker rule: **prefer Mode A with Section 4 elevated** (full plan PLUS embedded audience-build sprint) over Mode C alone.

Reason restated: Mode C alone would skip the launch playbook the founder still needs (because launch IS happening within 3-4 weeks). Mode A with elevated Section 4 produces BOTH the audience-build sprint AND the sequenced launch plan in one pass.

**MODE LOCKED: Mode A — Full Marketing Review, with Section 4 (Pre-launch audience-building) elevated as load-bearing.**

All 9 sections run in order. Sections 4 + 5 + 2 carry disproportionate weight given premise-audit findings.

---

# Section 1 — Competitive landscape

## 1a. Direct competitors

| Name | URL | Founded | Pricing | Apparent traffic sources | Public user complaints | Positioning vs tldrof | Honest read |
|---|---|---|---|---|---|---|---|
| **Readless.app** | readless.app | ~2024 | $4.90/mo (~$58.80/yr) | Heavy comparison-SEO (dozens of "Readless vs X" blog posts ranking on long-tail keywords). Some HN / Reddit / Product Hunt traffic likely. Solo founder per founder's pass-4 finding. [Source](https://www.readless.app/blog/best-newsletter-management-tools-2026) | "No instant magic moment (24h wait)", "no bulk-backlog flow", signup glitches per founder's trial | Same forwarding-address arch + AI summarization + dedup. Lower price ($4.90 vs $9). No magic moment. No bulk-backlog. Commodity-tier positioning. | **Apparent winner among direct comps** but on weak positioning. Beatable on (a) 60s magic moment, (b) bulk-backlog, (c) auto-forward UX, (d) M365/corporate-coverage IF tldrof actually ships it. |
| **Meco** | meco.app | ~2020 | Free + $35/yr ($3/mo) PRO | Mobile-first acquisition, App Store / Play Store organic, [Product Hunt launch](https://www.producthunt.com/products/meco), Gmail-OAuth integration as wedge | "Bugs", "paid wall for full features", Gmail-only structural limit | Dedicated newsletter inbox via Gmail OAuth. Mobile-first reader. Different model (you read inside Meco), not "one digest email." Has audio summaries. 4.77 stars / 660+ Play reviews. [Source](https://www.readless.app/blog/meco-pricing-2026) | **Different product shape** (reader vs digest) but same customer overlap. Has real user base. Gmail-OAuth structural limit blocks M365/corporate; that's the tldrof opening. |
| **Refind** | refind.com | ~2017 | Free + ~$5-10/mo Pro | Personal curation + sharing | Slow, opaque ranking | Different mechanic (curated highlights). Indirect competitor. | Lower threat. Don't anchor against. |
| **Mailbrew** | mailbrew.com | ~2020 | Free + ~$8/mo | Newsletter and feed digester | Acquired by Notion 2022; product appears dormant/maintenance | Was a direct comp; Notion acqui-hire and absorbed. | Effectively dead as standalone. Confirms market is real, exits happen. |
| **Notion Mail / Superhuman AI** | (varies) | 2025-26 | Bundled with Notion / $30+ | Existing user bases | OAuth-required, no corporate coverage | Premium-end of the market. Trust-led pricing. | **They prove the $30 price point works.** Coverage-moat narrative against them works. |

## 1b. Canonical-success comparables (load-bearing per M0b — design doc skipped this entirely)

| Name | Price | Founded | Scale | Primary acquisition channel | Onboarding model | Launch gate | Specific delta vs tldrof plan |
|---|---|---|---|---|---|---|---|
| **Superhuman** | $30/mo | 2017 | $700M ARR / $825M Grammarly acquisition Jul 2025 | [Mandatory 30-min concierge onboarding for every user. Word-of-mouth + invite-only waitlist.](https://review.firstround.com/superhuman-onboarding-playbook/) | Concierge (Vohra did first hundreds personally; peaked at ~20 onboarding specialists) | PMF-gate: 40% "very disappointed" Sean Ellis. [Went from 22% to 58% before unlocking growth.](https://saasclub.io/podcast/rahul-vohra-superhuman-342/) | tldrof plan: self-serve magic-link, no concierge, calendar gate. **Three deltas.** |
| **Readwise** | $9.99/mo (annual), $12.99/mo (monthly) | 2018 | $14M ARR, 4M users, 3M MAU, 82% YoY [Source](https://www.fueler.io/blog/readwise-usage-revenue-valuation-growth-statistics) | [Bootstrapped. EdTech partnerships, content-creator collabs, developer API ecosystem.](https://news.ycombinator.com/item?id=19530469) 30-day trial then paid; no freemium | Self-serve (but product is integration-heavy; integrations ARE concierge equivalent) | Product-led + retention-driven | tldrof plan: 7-day trial (vs 30-day), monthly-only at v1 (vs annual push), no content / partnerships / API plan. **Four deltas.** |
| **Morning Brew** | Free + $20-50/mo Premium | 2015 | $75M acquisition by Insider Inc 2020; ~2.5M subscribers at acquisition | Audience-first: built newsletter audience for ~5 yrs before monetizing premium. Referral program ("get N referrals, get swag"). | Self-serve | n/a (content business, not SaaS) | tldrof plan: audience-build is afterthought. Morning Brew built audience FIRST, then monetized. tldrof's order is inverted. |

## 1c. Pattern surface

**What canonical successes have in common that current plan lacks:**

1. **Concierge or concierge-equivalent onboarding.** Superhuman did literal 30-min sessions; Readwise's integration-heavy setup is concierge-equivalent labor; Morning Brew's referral program is concierge-via-existing-users. Current tldrof plan: self-serve magic-link with "operator-shape watch-item" actively excluding the concierge mechanic.

2. **PMF-signal launch gate, not calendar gate.** Superhuman is the canonical example. tldrof: calendar gate (day ~20-22).

3. **Audience built BEFORE product launch matters.** Morning Brew, even Readwise to a lesser degree, built distribution surface before the product was the headline. tldrof: zero audience, calendar-gated launch.

4. **Premium pricing held against commodity competition.** Superhuman $30 vs free Gmail. Readwise $10-13 vs free Pocket. Neither raced to the bottom. tldrof: anchored on Readless's $4.90.

5. **Content cadence as compounding distribution.** Readwise's blog + partnerships + API ecosystem. Morning Brew is content as product. tldrof: zero content plan.

**Where direct competitors diverge from canonical-success patterns:**

- Readless plays the COMPARISON-SEO game (different playbook entirely). It may win or lose; we'll see.
- Meco played the MOBILE-FIRST + ONBOARDING-VIA-OAUTH game (different playbook).
- Neither Readless nor Meco follow the Superhuman premium concierge playbook.

**Which pattern is current plan implicitly following:**

The current plan is implicitly following the **Readless playbook minus the SEO investment**. That is the worst possible mix: same commodity price, same self-serve mechanic, but without the comparison-SEO content moat Readless is building. tldrof will lose to Readless on this trajectory IF Readless's SEO investment compounds before tldrof builds an alternative.

**The right pattern to follow is the Superhuman + Readwise hybrid:**
- Premium price ($14-19 OR hold $9 with a different defense — see Section 6)
- Concierge intake for first 20-50 paying users
- Content cadence (founder writes, founder pitches podcasts, founder builds partnerships)
- Audience-build sprint pre-launch (Section 4)

**Founder action:** read [Superhuman's onboarding playbook](https://review.firstround.com/superhuman-onboarding-playbook/) (45 min) AND [Readwise's "Why we're bootstrapping" post](https://blog.readwise.io/why-were-bootstrapping-readwise/) (15 min) AND [Lenny's interview with Rahul Vohra](https://www.lennysnewsletter.com/p/superhumans-secret-to-success-rahul-vohra) (60 min). 2 hours total. Pre-launch homework, non-negotiable.

---

# Section 2 — ICP specification

Tightened from M1. Written to `icp.md` as separate artifact (see /icp.md). Inline summary here:

**Primary v1.0 ICP — "Priya":**

- 30-45, knowledge worker (PM, marketing, finance, consulting, ops, founder-equivalent)
- Gmail or M365 user (v1.0 ships Gmail-only auto-forward, so primary v1.0 = Gmail subset; M365 promoted to v1.0.5)
- ≥3 newsletter subscriptions, ≥1 from an industry/vertical publication (NOT just dev TLDRs)
- Inbox state: chronic 1,000-5,000 unread, "newsletter shame" pile
- Currently pays for: at least one premium content subscription ($10-30/mo range — Lenny's, Stratechery, The Information, NYT/WSJ, Notion personal, ChatGPT Plus)
- Hangs out: Lenny's Newsletter, podcast versions of Lenny / Acquired / Stratechery, LinkedIn for industry content, Reforge if PM/marketing
- Doesn't shop free trials of 10 productivity apps in a weekend (time-poor, trust-led)
- Triggers: "I declared inbox bankruptcy in Q1, want a system" OR "my coworker showed me their digest"

**Adjacent ICP (defer to v1.0.5+):**
- M365-only corporate-locked-out segment (lawyers, finance, healthcare, government, agency operators on custom-domain email). Same persona shape but corporate-email-locked. Requires v1.0.5 auto-forward-multi-client.

**Explicit exclusions for v1.0 (DO NOT target with launch copy):**
- Pure HN-cohort dev-newsletter readers — that's Readless's segment, $4.90 floor, comparison-shoppers
- "Indie hackers" as a category — too broad
- Power users wanting MCP/API — defer to v1.1 audience

**Conversion drivers:**
- "I've been telling myself I should fix this for months" (mental-load relief)
- "I want to read Lenny's and Stratechery in full, skip the rest" (signal-to-noise)
- "I can't add browser extensions to my work inbox" (forwarding architecture is the only viable option for corporate)

**Conversion objections:**
- "I tried Meco / Refind / similar; they didn't stick" → magic-moment + bulk-backlog is the differentiator
- "$9/mo for a newsletter aggregator?" → if priced at $9, need positioning that justifies; if priced $14-19, positioning emphasizes coverage + concierge
- "Privacy — you're reading my email?" → forwarding architecture story
- "I'll just unsubscribe instead" → bankruptcy framing pre-empts (you've TRIED that, didn't work)

See `./icp.md` for full version.

---

# Section 3 — Distribution channel-by-channel

Scoring scale: 1-5 (5 = strong).

| Channel | Reach (for Priya ICP) | Cost | Conversion | Founder fit | Effort to start | Leverage (R×C×F/$/E rough rank) |
|---|---|---|---|---|---|---|
| **Concierge outreach to founder's named network** | 1 (small N) | $0 | 5 (warm) | 5 | 2 (do this week) | **RANK 1** for first 10-20 paying. The Superhuman playbook. |
| **Vertical newsletter sponsorships (Lenny's, Morning Brew, Stratechery)** | 5 | 3 ($500-5000/placement) | 4 (in-context, trust-led) | 3 (no relationships yet) | 3 (4-8 wk lead times for premium placements) | **RANK 2** for scaled cohort, ~30-60 days post-launch |
| **LinkedIn organic (founder writes about inbox overload / building tldrof)** | 3 (founder has 996, wrong cat but some bleed) | $0 | 2 | 3 (founder doesn't write, can learn) | 4 (start today, compounds over months) | **RANK 3** — content engine, foundational |
| **Show HN** | 3 for dev-cohort subset of ICP; 1 for Priya overall | $0 | 1 (0.01-0.09% paying per HN consumer base rate) | 4 (founder knows HN) | 1 (single post) | **RANK 4** — one channel among several, NOT the launch |
| **Product Hunt** | 3 (different audience than HN, more consumer-friendly) | $0 (low if you can self-hunt) | 2 | 2 (no hunter relationships) | 3 (need warm-up) | RANK 5 |
| **r/productivity / r/M365 / r/sysadmin / r/Lenny's-adjacent communities (incl. r/ProductManagement)** | 2-3 | $0 | 3 (if compliant w/ community rules) | 2 (founder isn't known) | 4 (need 2-4 wks credibility building first) | RANK 6 |
| **IndieHackers launch + community engagement** | 2 (mostly indie devs, partial overlap) | $0 | 2 | 4 | 2 | RANK 7 |
| **Podcast guesting (Pragmatic Engineer adjacent / Lenny's adjacent)** | 4 (Priya listens to these) | $0 | 4 (trust-led) | 2 (no relationships, no PR rep) | 5 (12-24 wk lead) | RANK 8 long-term — slow but compounds |
| **Twitter/X organic** | 2 | $0 | 2 | 1 (zero following) | 4 | RANK 9 — don't bother organic; potentially use paid for retargeting only |
| **SEO (long-tail "inbox bankruptcy", "Outlook newsletter manager")** | 2 short term, 4 long term | 2 (content costs) | 3 | 2 (no SEO experience) | 5 (6-12 mo ramp) | RANK 10 long-term; do NOT compete with Readless's existing "X vs Y" SEO playbook directly |
| **Paid ads (Google / Meta / LinkedIn)** | varies | 1 (expensive) | varies | 1 | 3 | DEFER until ICP locked and conversion path proven |
| **Cold email outreach** | 3 | $0 | 2 (low warm rate) | 3 | 3 | RANK 11 — useful for podcast / partnership pitches, NOT for direct user acq |
| **Affiliate / referral program in-product** | 4 once cohort exists | 1 (rev share) | 3 | 4 | 3 | DEFER to v1.0.5 — needs user base first |

**Channels CUT (won't ship in v1):**

- TikTok / YouTube / Instagram organic — wrong content surface for Priya at this stage
- Reddit r/SideProject — wrong audience entirely (indie maker browsing, not Priya)
- Substack growth-hacks (founder's existing 11) — too small to matter and wrong audience
- Discord / Slack community presence — too slow for the 30-60 day window
- Influencer partnerships — premature

**Surviving channels for v1.0 launch (in priority order):**

1. **Concierge outreach** (RANK 1) — first 10-20 paying within 2-4 weeks
2. **Show HN** (RANK 4) — secondary launch event, dev-cohort subsegment, NOT the primary
3. **LinkedIn organic content** (RANK 3) — start today, 8-12 week compound
4. **One Lenny's / Stratechery / Morning Brew newsletter sponsorship** (RANK 2) — once first 10 paying validate concept, ~day 30+

Four-channel plan. NOT "do all 14." NOT "Show HN as the entire plan."

## Motion-class-specific channel notes

**Consumer subscription motion class** (per Section 3 motion-class rules):

- HN is wrong audience class for Priya. Reach score for HN reflects this. The dev-newsletter subsegment can be reached via HN; that's a small fraction of the target paying ICP.
- Specific vertical publications carry disproportionate weight: **Lenny's Newsletter, Stratechery, Morning Brew, Axios Pro Rata, The Information, Pragmatic Engineer**. Each has a known sponsorship rate ($1K-10K depending on placement). One placement = potentially 50-500 trial signups from a trust-led audience. Disproportionately better than HN for THIS ICP.

**Dev-tool motion-class rules do NOT apply** — this is not a dev tool. Founder must NOT apply dev-tool launch tonal patterns to launch copy. Specifically: copy needs to read as "someone like Priya wrote this for someone like Priya" — NOT engineer-to-engineer. (However, if a SECONDARY launch post targets HN, that post specifically should follow dev-tool tonal rules: technical specifics, honest comparisons including where Readless wins, link to GitHub if any. Two posts, two tonal registers — don't unify them.)

---

# Section 4 — Pre-launch audience-building plan (LOAD-BEARING per v0.3 elevation)

Founder starts from zero ICP-aligned audience. ~20-22 days of build remain. ≥30% reallocation to audience-building required per M7.

## Day 1-30 (i.e., from today through ~launch+10)

**Weekly cadence:**

- **2x per week:** LinkedIn long-form post (~600-1200 words) about (a) inbox overload as a problem, (b) how Priya-shaped knowledge workers cope, (c) building tldrof — NOT product hype, NOT "buy this" — building-in-public + thought-leadership. Topics: "Why your newsletter inbox is bankrupt", "The hidden cost of newsletter shame", "What Superhuman's onboarding teaches us about premium consumer SaaS", "Forwarding architecture: the privacy-first alternative to OAuth".
- **1x per week:** Concierge outreach. Email 5-10 named people from M6 list + 5-10 warm intros they suggested. Personal, no template. Offer concierge-intake (15-min Zoom, founder onboards them, $9/mo or free for 90 days for weekly feedback).
- **1x per week:** Engage in 2-3 relevant communities WITHOUT promoting. r/ProductManagement, r/M365, IndieHackers comments. Pure value-add answers to inbox-overload-related questions. Goal: become recognizable name 4-6 weeks pre-launch.
- **Daily:** Founder forwards corrected-ICP-aligned newsletter mix to test address (Morning Brew + Axios + Stratechery + Lenny's + 1 vertical). Tunes prompts against THIS mix per M0e pivot.

## Day 31-60 (post-launch month 1)

Scale based on day 1-30 signal:
- If LinkedIn posts averaging >100 reactions: continue cadence, add 1 weekly thought-leadership thread on X (founder builds X following from scratch with substantive content)
- If LinkedIn posts averaging <30 reactions: signal is weak; pivot content angle. Maybe focus on the "I built this and these 10 people are using it" build-in-public angle instead of thought-leadership
- Start podcast guest pitches: pitch 1 podcast per week (Lenny's adjacent, Acquired adjacent, Pragmatic Engineer adjacent, Indie Hackers podcast, MicroConf On Air, etc.). Realistic conversion: 1-2 yes per 10 pitches, 4-8 week scheduling lead.

## Day 61-90 (post-launch month 2-3)

- Newsletter sponsorship placement #1 (recommend: Lenny's Newsletter, ~$5K, requires 4-8 wk lead so book NOW at day 30 for day 60-90 placement)
- Continue concierge-intake outreach to expand from 10-20 paying → 30-50 paying
- Aim: SEO content has been compounding for 60 days; start measuring organic search traffic
- Apply for podcasts based on traction (4-8 week lead times from pitch → guest spot, so book NOW)

## Refused vague commitments

- "I'll post more on Twitter" — REJECTED. Replaced with: 2x weekly LinkedIn (named cadence, named topics)
- "Build in public" with no specifics — REJECTED. Replaced with: weekly LinkedIn post with named topic list
- "Network harder" — REJECTED. Replaced with: 5-10 named outreach contacts per week, concierge-intake offer specified

## Specific output target by launch day

- ≥6 published LinkedIn long-form posts (3 weeks × 2)
- ≥30 personal outreach emails sent (3 weeks × 10)
- ≥10 community comments / answers logged (3 weeks × 3-4)
- ≥1 podcast booked for post-launch (even if just confirmed lead time)
- ≥3 paying customers from concierge cohort BEFORE Show HN day, used as social proof in launch copy

This is the load-bearing work item. Without it, P5/P6 are math-impossible.

---

# Section 5 — Launch playbook (multi-channel, sequenced)

## 5a. Question the launch gate BEFORE the sequence

**Required question:** What is the gate that fires launch? Calendar (day ~20-22) or PMF signal?

**Current plan:** calendar (day ~20-22 per CEO review).

**Founder defense of calendar:** "I want to ship. I have founder-momentum. The build is done. Waiting kills me."

**Skill pushback:** tldrof is a RETENTION-DRIVEN consumer subscription (per P6 trial-conversion psychology, per Strategic Ladder Rung 1 retention thesis, per CEO review L5). For this class of product, calendar-gate is wrong per Vohra precedent (Superhuman went 22% → 58% before unlocking). [Source](https://saasclub.io/podcast/rahul-vohra-superhuman-342/)

**Proposed alternative: CONCIERGE-FIRST COHORT BEFORE PUBLIC LAUNCH.**

Replace the day-22 Show HN with:
- **Day 22-35:** Concierge cohort (10-20 paying, founder personally onboards each via 15-min Zoom, watches them set up their first filter, measures their actual retention for 2 weeks)
- **Day 35:** Run Vohra "very disappointed" survey on concierge cohort. If <30% "very disappointed" → product is not yet retention-strong, iterate before public launch (DON'T expand). If ≥30% (close to 40% bar) → proceed with public Show HN + LinkedIn + sponsorship launch.
- **Day 35-50:** Public launch sequence (see 5b below).

This costs 13 days of "launch delay" relative to the calendar plan. The 13 days are spent earning PMF evidence, NOT silence-after-launch. The expected value is dramatically higher.

**If founder REFUSES** to delay and insists on calendar launch on day ~22: acceptable ONLY with explicit acknowledgment of the Vohra precedent and a written-down plan for "what we do if day-30 cohort hits <10 paying" (which is the failure mode the calendar gate is most likely to produce). Document the risk; don't silently absorb it.

## 5b. Default sequence pattern (assumes calendar gate held OR PMF gate passed)

| Day relative to launch | Channel | Specific action |
|---|---|---|
| Launch -30 to -3 | Audience-build | Per Section 4 cadence |
| Launch -7 | Personal network email | Soft pre-announce to all 30-50 named contacts. "Launching publicly next week; I'd love your help amplifying if you've found it valuable." |
| Launch -3 | LinkedIn long-form | Build-in-public retrospective: "I've been quietly building tldrof for ~6 weeks; here's what I learned about inbox overload from my first 10 users." Include 1-2 named quotes from concierge cohort (with permission). |
| Launch -2 | Concierge cohort | Final ping: "Launching to public Tuesday. Could you (a) share with 2 people who'd benefit, (b) post a 1-line review on Twitter/LinkedIn day-of." |
| **Day 0, 8am PT** | **Show HN** | Show HN: "tldrof.com — Forward newsletters to clear inbox bankruptcy in 60s. Built it because Readless didn't have a magic moment." Honest comparison-table including where Readless wins (price, RSS). Code-first link if any open-source repo. Tonal register: builder-to-builders, NOT marketing-speak. (See dev-tool tonal rules from skill Section 3 for the Show HN post specifically.) |
| Day 0, 8am | **Direct LinkedIn post (parallel to HN, not after)** | LinkedIn long-form announcement targeted at Priya-cohort. Different tonal register from HN post. Lead with the inbox-overload problem; the product is the answer. Less code, more "I asked 10 PMs how they cope with newsletter overload, here's what I built." |
| Day 0, 10am | Twitter | Thread with HN link + LinkedIn link cross-reference. Founder's small X account is fine; the thread is for amplification by HN/LI traffic, not as primary channel. |
| Day 0, all day | Concierge cohort | Personally thank concierge users + ask for the share/review they pre-committed to. |
| Day 0 + 24h | IndieHackers | Cross-post (HN-first to avoid duplicate-content). Lean into the "indie founder shipped this" framing. |
| Day 0 + 48h | r/ProductManagement, r/M365 (if rules permit), r/productivity | Compliant cross-posts. CHECK community self-promo rules FIRST. Many subs forbid; respect that. |
| Day 0 + 5d | Product Hunt | Separate launch event. Different audience. Coordinate with PH hunter (need to source warmly 2-4 wks pre). |
| Day 0 + 14d | Newsletter sponsorship #1 (Lenny's or Morning Brew) | First sponsored placement runs. Book at launch -30. Budget ~$3-7K. |
| Day 0 + 14-21d | Podcast outreach | Pitch 10 podcasts in the Priya-cohort space (Lenny / Acquired / Pragmatic Engineer / Indie Hackers / MicroConf). 1-2 yeses realistic. |
| Day 0 + 30d | Substack | Retrospective with traction numbers (paying count, time-saved-aggregate, qualitative quotes). Doubles as case-study for next sponsorship pitch. |

## Risk callouts

- **HN miss = NOT the end of the world** because HN is one of four channels (concierge, LinkedIn, HN, sponsorship). Previous version of this plan would have died on HN miss; this version has multi-channel resilience.
- **All-on-LinkedIn risk** — algorithm shifts, organic reach varies. Mitigated by concierge + sponsorship + HN diversity.
- **Single Reddit subreddit ban** — minor risk, contained to 1 of 4 channels.
- **Concierge cohort negative signal (Vohra survey <30%)** — proceed to public anyway? NO. Hold launch, iterate product. This is the gate, not the calendar.
- **Sponsorship budget unavailable** — founder is bootstrapped; $3-7K for first sponsorship may be a real constraint. Acceptable substitute: 3 micro-sponsorships at $500-1000 each in smaller newsletters (e.g., Pragmatic Engineer's classifieds, ConvertKit's Creator Network, Beehiiv's recommendation network).

See `./launch_playbook.md` for hour-by-hour version of Day 0.

---

# Section 6 — Pricing & packaging

## 6a. Question the pricing BAND before the price point

**Required question:** Did the price band inherit from competitor anchoring or from ICP WTP evidence?

**Reality:** Pricing was anchored on Readless at $4.90 → "we'll be $9, premium-ish vs them." That's BAND-FROM-COMPETITORS thinking. NOT ICP-WTP-driven.

**ICP WTP evidence (what Priya actually pays for adjacent productivity / attention products):**

- ChatGPT Plus: $20/mo
- Notion Personal: $10-15/mo
- Lenny's Premium: $20/mo (annual) / ~$25/mo
- Stratechery: $15/mo
- The Information: ~$33/mo
- Superhuman: $30/mo
- Readwise: $10-13/mo
- Substack publication subs: $5-15/mo each (many)
- SaneBox: $5-7/mo

**Median in Priya's adjacent-category spend: $15-20/mo. Top quartile: $25-30/mo.**

**[RevenueCat data](https://www.revenuecat.com/state-of-subscription-apps/):**
- "Median high-priced apps convert downloads 2× better than low-priced apps. High-priced median: 2.8% (top quartile above 6.1%). Mid-priced median: 2.0%. Low-priced median: 1.4%."
- "Yearly plans renew at 83.4% overall, 4× weekly subs, ~2× monthly plans."
- "North America $32 median realized LTV per payer after Y1."

**Verdict:** $9/mo is at the LOW end of Priya's adjacent-spend band. Anchored on Readless rather than on what Priya actually pays for similar tools. There's room (and likely a conversion-rate benefit) to price at $14-19.

## 6b. Pricing recommendation

**OPTION 1: Hold $9, hold launch, defend differently.**

Hold $9 only if defense rests on:
- 60-second magic moment (Readless 24h delay)
- Bulk-backlog flow (Readless can't do)
- Auto-forward-helper covers more clients (NOT TRUE for v1.0 Gmail-only — must fix or kill this claim)

This is the CEO PC1 plan. It survives ONLY if the Gmail-only auto-forward contradiction (M0c) is resolved by either (a) shipping multi-client auto-forward in v1.0 (cuts CEO PC2) or (b) honestly admitting v1.0 is Gmail-only and dropping the corporate-coverage narrative until v1.0.5.

**OPTION 2 (RECOMMENDED): Move to $14/mo monthly OR $9/mo annual ($108/yr) — annual-first pricing.**

Rationale:
- $14 monthly anchors Priya properly (above Readless/Meco floor, in line with Lenny's premium / Stratechery / Notion Personal)
- $9/mo if billed annually (=$108/yr) is BOTH a discount narrative AND gets the [83.4% annual retention bump per RevenueCat](https://www.revenuecat.com/state-of-subscription-apps/) vs ~half on monthly
- Premium positioning: "Premium subscription for premium readers. We don't compete on price; Readless does."
- This is the Readwise playbook (annual-first, $9.99/mo annual / $12.99/mo monthly).

**OPTION 3: Move to $19/mo with explicit concierge-onboarding offering** for the corporate-locked-out segment ($19/mo with founder onboards you via 15-min Zoom call). This is the Superhuman-lite playbook. Risk: very small TAM until the founder can hire onboarding specialists; but the unit economics work well.

**My recommendation:** **OPTION 2 with annual-first pricing** ($14 monthly / $9 annual). Defensible, premium-anchored, doesn't race to Readless's floor, captures annual retention bump, easy to communicate.

## 6c. Trial mechanic revisit (M0d carry-forward)

Two-mode trial offering:

- **Self-serve mode (Gmail-cohort, Priya-ICP):** 7-day no-CC trial as currently designed. Validation = paying cohort for this segment.
- **Concierge mode (corporate-cohort once v1.0.5 ships, OR for the first 20-50 paying users in v1.0):** "Book a 15-min call with the founder. I'll set up your account, walk you through inbox-bankruptcy, and confirm forwarding works for your subscriptions. Charged $14/mo immediately after; cancel anytime."

The concierge mode IS the trial mechanic for trust-led segments. It selects FOR the right cohort and AGAINST comparison-shoppers.

## 6d. Annual discount strategy

- Annual price: $108/yr (=$9/mo billed annually, ~36% off monthly $14)
- Promote annual aggressively in onboarding (after first digest renders)
- [RevenueCat: yearly plans renew at 83.4% overall vs ~half for monthly](https://www.revenuecat.com/state-of-subscription-apps/) — annual is the retention move
- Once payment is annual, churn drops materially. Same playbook as Readwise.

## 6e. Per-seat / per-feature / per-usage

Per-feature (Pro tier) is a v1.0.5 thing. Don't fragment v1.0 by tier. Single price, single product.

---

# Section 7 — Post-launch growth loops

What compounds vs what's linear:

| Loop | Compounds? | Action in v1 |
|---|---|---|
| **Referral mechanics** | YES if implemented | v1.0.5: in-product "share your concierge address → get 1 month free" referral. Not v1.0 (premature). |
| **Content compounding (SEO)** | YES, 6-12 mo ramp | Start NOW (Section 4). DO NOT compete on Readless's "X vs Y" SEO terms; do compete on "inbox bankruptcy", "newsletter overload Outlook", "newsletter dedup for M365", "how to declare inbox bankruptcy on newsletters" long-tail. |
| **Network effects** | NO at v1.0 | Not network-effect product (single-user digest). v1.1+ might add "team digest" feature for orgs (would create network effect within orgs). Don't claim network effects in v1 pitch. |
| **Brand compounding** | YES, 12-36 mo | Consistent founder voice on LinkedIn / podcast guesting / Substack. Pay off in year 2. |
| **Retention as growth (WOM)** | YES IF retention strong | If concierge cohort hits Vohra 30-40% "very disappointed", word-of-mouth fires from that cohort. THIS is the loop that drives P5/P6 if it works. |

**Honest read:** v1 is NOT network-effect; growth-loop story rests on (a) retention-driven WOM, (b) SEO compounding, (c) content brand compounding. All three require 30/60/90-day work TODAY.

**Acquisition-treadmill risk:** if WOM doesn't fire (retention not strong enough), every new user requires new spend (newsletter sponsorships, paid ads in v1.0.5+). Solo bootstrapped founder cannot run acquisition treadmill at scale. The Vohra-gate cohort PMF survey is the load-bearing risk check.

---

# Section 8 — Metrics & instrumentation

## Track (with UTMs and per-channel attribution from day -7)

- **Acquisition by channel** (concierge / Show HN / LinkedIn / sponsorship / IndieHackers / etc.) — UTMs on every link
- **Activation** = user signed up AND forwarded ≥3 newsletters AND saw their first digest render in browser. Track activation rate per cohort.
- **filter_setup_rate_48h** (carried from CEO post-skill cleanup item 2) — % of users who set up auto-forwarding within 48h. **Interpretive bands: ≥60% = retention thesis intact; 30-60% = mixed; <30% = retention broken at auto-forward bottleneck. Investigate before optimizing anything else.**
- **Day-7 retention** = % of trial users who get day-7 digest
- **Day-30 retention** = % of paying users who haven't churned (subscription_status = active) at day 30
- **Trial-to-paid conversion** = % of trial users who become paying
- **Vohra "very disappointed" survey** — run on every paying user at day 14 of trial AND day 60 of paying. Bands: <30% = retention is broken; 30-40% = on track; ≥40% = strong.
- **LTV / CAC** — calculate at day 90+. For concierge cohort, CAC ≈ founder's time. For sponsorship cohort, CAC = $sponsorship / paying users sourced.
- **Per-segment metrics** (Gmail vs M365 vs other; Priya-ICP vs dev-newsletter subsegment) — segment all of the above by source-segment.

## DO NOT vanity-track

- LinkedIn follower count
- Substack subscriber count alone (unless converting to paid)
- Total signups without retention
- HN upvotes (correlation with revenue near-zero per [base-rate data](https://smollaunch.com/compare/product-hunt-vs-hacker-news))
- Total trial signups (cheap-trial mechanic per M0d makes this number misleading)

## Weekly review

Monday morning, 30 min:
- Vohra survey results (cumulative)
- Filter setup rate (rolling 14-day cohort)
- Trial → paid conversion (rolling 7-day)
- Day-30 retention (rolling 30-day cohort)
- Per-channel paying customer count

If filter_setup_rate_48h falls below 30% for two consecutive weeks → emergency UX review. If Vohra "very disappointed" stays under 25% past day 30 of public launch → halt expansion, iterate product. These are the trip-wires.

---

# Section 9 — Risk analysis

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| **Channel concentration on Show HN** | Already mitigated in this plan (HN is 1 of 4 channels) | High if it had been concentrated | Plan diversifies to concierge + LinkedIn + sponsorship. |
| **HN miss → public launch silence** | Medium | Medium | Concierge cohort + sponsorship cover. LinkedIn parallel post creates parallel discovery surface. |
| **Calendar-gate launch fires before retention proven (Vohra <30%)** | HIGH if founder insists on calendar | Catastrophic for retention-driven product | Adopt PMF-gate per 5a. If refused, document explicitly. |
| **CAC inflation in vertical newsletter sponsorships** | Medium 6-12mo out | Medium | Diversify across 3-5 publications; rotate; measure per-placement conversion |
| **Readless pivots to bankruptcy / multi-client / concierge BEFORE tldrof builds defense** | Medium (Readless is also solo, capability-parity) | High | Ship positioning fast (Edit 1 of Pass 4); ship multi-client v1.0.5 fast; build Strategic Ladder Rung 2 (Suite) as the longer-term defense Readless isn't building |
| **Algorithm risk on LinkedIn organic** | Low-Med | Medium | Diversify across LinkedIn + Substack + podcast guesting; don't bet on single platform |
| **Trust risk — early WOM hasn't compounded yet, brand unknown** | High first 60 days | Medium | Concierge cohort builds founder-trust transfer (each concierge user trusts founder personally). Sponsorship in known publication borrows trust. LinkedIn content builds slow trust over months. |
| **M0c/M0e — product calibrated wrong because dogfood was wrong** | High if no fix; mitigated if M0e pivots adopted | Catastrophic | M0e fix mandatory before launch: 2 weeks of Priya-mix dogfood with prompt re-tuning |
| **Macro: M365 corporate policy change blocking external forwarding** | Low | High for corporate segment | Already discussed in design doc; corporate IT often does block external forwarding. Validate with first 3-5 corporate users before claiming corporate-coverage in marketing |
| **Competitor counter-launch (Readless ships magic moment)** | Medium 60-180 days | High | Velocity advantage + Strategic Ladder depth; positioning narrative; brand compounding from content |
| **Pricing race-to-bottom pressure** | Medium | High | Premium-anchor narrative; resist matching $4.90; if must change, raise to $14 not lower to $4.90 |

---

## Outside voice — independent marketing critique (Claude subagent simulation)

Pretending to run an independent Claude subagent for critique. Below is what an outside reviewer would surface.

### Critique 1: Single biggest marketing risk the inside review missed

**The plan is correctly skeptical of Show HN but underestimates how hard "Lenny's Newsletter sponsorship" actually is to convert.** Lenny's sponsorship rates are ~$5-15K for newsletter placements with 200K+ subscribers. Even with great copy, conversion to $9-14/mo paying subscribers is plausibly 0.05-0.3% (much like HN base rate for consumer, just with better-targeted audience). That means $5K → 1000 signups → 30-150 paying. Cost per paying customer: $33-167. For a $108/yr LTV product with churn, that may not pay back in year one. **Sponsorship is a real channel but not the magic bullet the plan implies. Re-budget sponsorship as "marketing investment in brand/awareness, paid back in year 2" rather than as direct CAC.**

### Critique 2: Channel weaker than positioned

**Concierge outreach to "30-50 named contacts" is positioned as the load-bearing first-10-paying channel. Realistic conversion: 30 emails → 8-12 take the meeting → 3-6 convert to paying. That's enough for first 5-10 paying but NOT enough for first 20-30 paying.** The plan should make this explicit: concierge gets you to 5-10 paying in 2-4 weeks; getting to 25-50 paying requires the public launch + sponsorship + content cadence to compound. The plan correctly sequences these but understates the gap between "first 10" and "first 30."

### Critique 3: Audience-claim that lacks evidence

**The "M365 corporate-locked-out segment" is claimed as the structural moat but has ZERO validation in the design doc or this plan.** Founder has not interviewed a single lawyer, finance professional, healthcare admin, or government employee about whether they would (a) forward newsletters externally given corporate IT policies, (b) pay $9-19/mo personally for inbox cleanup, (c) be willing to deal with multi-client filter setup. The structural-coverage moat is an assumption, not a validated demand pattern. **Required before treating this as a real segment:** 5 interviews with corporate-locked-out professionals (one each: lawyer, finance, healthcare, government, agency). If even 2/5 say "my IT blocks external forwarding" → the moat is illusory for those verticals. This is a 1-week task that could invalidate or validate the v1.0.5 expansion direction.

### Critique 4: Provocative reframe

**What if tldrof is NOT a consumer subscription product but a B2B / team product?**

The strongest version: "Newsletter intelligence for product teams. Forward your team's newsletter pile (every PM's inbox accumulates 50-200 newsletters). One daily team digest covers what the whole team is reading, deduplicated. $99/mo per team of 5-10."

Pros:
- Higher ARPU ($99/mo team vs $14/mo individual)
- Slower churn (team subscriptions stickier than individual)
- Concierge mechanic FITS naturally (team onboard via founder Zoom call)
- Differentiation from Readless is stronger (Readless is individual; team-shape doesn't exist in the comp set)
- Distribution channel changes — pitching to heads of product / heads of marketing in 200-1000 person companies (Lenny's-like audience but as buyers, not users)

Cons:
- Different sales motion (B2B sales cycle 30-60 days vs consumer signup in seconds)
- "skill not_for" explicitly excludes B2B enterprise sales (note: B2B SMB / team-tier without enterprise sales motion may be acceptable per skill scope)
- Founder has zero B2B experience either; learning curve

**This is a real reframe worth at least 1 hour of consideration before locking the consumer subscription thesis.** Suggested action: 5 conversations with PM-leaders at 50-200 person companies asking "would you pay $99/mo for your team to share a newsletter digest?" If 2/5 yes → consider hybrid (consumer $14 + team $99) or pivot.

### Net summary from outside voice

- Sponsorship CAC is real and not in the plan — re-budget as brand investment
- Concierge gets you to 5-10 paying not 30 paying — sequencing gap
- M365 segment is unvalidated — 1 week of customer interviews required
- Team / B2B SMB reframe is worth 1 hour of consideration before locking individual-consumer thesis

---

## This week's 3 strongest action items (force the founder to commit)

1. **Pivot the dogfood subjects THIS WEEK.** Subscribe (via test forwarding address) to: Morning Brew, Axios AM, Stratechery, Lenny's, and 1 vertical newsletter the founder can credibly read for 2 weeks. Cut dev-only dogfood as the sole input. Tune dedup + summarization prompts against this mix. **Why this week:** Eng-review build window is mid-flight; product is being tuned RIGHT NOW. Every day of dev-only tuning entrenches the wrong audience signature. This is the M0e fix and the #1 action item.
2. **Email the M6 named-10-people list THIS WEEK with a concierge-intake offer.** Personal, no template. "I'm building tldrof.com, want to onboard you personally next week via Zoom, $14/mo or free for 90 days for weekly feedback." Goal: 3 say yes by end of week, 6-10 say yes by end of week 2. **Why this week:** First 10 paying must come from concierge per M6; if outreach doesn't start now, the launch ships to silence.
3. **Write LinkedIn long-form post #1 THIS WEEK.** Topic: "I built a system to deal with my newsletter inbox bankruptcy. Here's what I learned about why other people's solutions don't stick." NOT product hype. Builds founder credibility for the corrected Priya-cohort. Start cadence. **Why this week:** LinkedIn content compounds slowly; starting now means it has 3-6 weeks of compounding before launch. Starting at launch is too late.

---

## Schedule self-check

Re-run plan-cmo-review skill in 30 days. Evaluate:
- Did filter_setup_rate_48h beat 30%?
- Did concierge cohort hit 5+ paying?
- Did Vohra "very disappointed" hit 30%+?
- Did LinkedIn cadence sustain 2/week?
- Did dogfood pivot complete (Priya-mix forwarding for 2 weeks)?

If 4+/5: proceed to public launch sequence.
If <3/5: hold launch, address gaps.

## Recommended follow-up skills

- **`/office-hours`** if the Team-tier reframe from outside voice critique resonates and founder wants to consider pivoting before locking ICP
- **`/plan-ceo-review`** if pricing changes from $9 to $14 annual-first require business-model revision
- **`/plan-eng-review`** if marketing requires product changes (concierge-intake flow as separate signup path, referral mechanics for v1.0.5)
- **`/plan-design-review`** for the landing page — especially given the recommended segment-specific copy variants

## Artifacts written

- `marketing_plan.md` (this file)
- `icp.md` — full ICP specification
- `launch_playbook.md` — hour-by-hour Day-0 sequence
- `audience_build_journal.md` — weekly tracking template

## Web sources cited

- [Superhuman onboarding playbook (First Round Review)](https://review.firstround.com/superhuman-onboarding-playbook/)
- [Rahul Vohra on Superhuman: Lenny's Newsletter](https://www.lennysnewsletter.com/p/superhumans-secret-to-success-rahul-vohra)
- [Rahul Vohra finding PMF with data (SaaS Club)](https://saasclub.io/podcast/rahul-vohra-superhuman-342/)
- [Readwise pricing](https://readwise.io/pricing)
- [Readwise: Why We're Bootstrapping (HN)](https://news.ycombinator.com/item?id=19530469)
- [Readwise 2026 growth statistics](https://www.fueler.io/blog/readwise-usage-revenue-valuation-growth-statistics)
- [Readless.app pricing/feature comparison (their own blog)](https://www.readless.app/blog/best-newsletter-management-tools-2026)
- [Meco pricing 2026](https://www.readless.app/blog/meco-pricing-2026)
- [Meco app store listing](https://www.producthunt.com/products/meco)
- [Show HN vs Product Hunt (Smol Launch)](https://smollaunch.com/compare/product-hunt-vs-hacker-news)
- [Show HN front-page case study (IndieHackers)](https://www.indiehackers.com/post/my-show-hn-reached-hacker-news-front-page-here-is-how-you-can-do-it-44c73fbdc6)
- [RevenueCat State of Subscription Apps 2026](https://www.revenuecat.com/state-of-subscription-apps/)
- [First 100 paying customers (IndieHackers content strategy)](https://www.indiehackers.com/post/from-0-to-100-paying-users-the-exact-threads-content-strategy-i-used-to-launch-my-saas-e4c127ff30)

---

END marketing_plan.md
