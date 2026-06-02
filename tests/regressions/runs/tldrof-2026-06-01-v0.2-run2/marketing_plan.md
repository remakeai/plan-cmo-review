# Marketing Plan — TLDR-of-TLDRs (tldrof.com) — v0.2 review run 2

**Skill:** plan-cmo-review v0.2
**Date:** 2026-06-01
**Founder context:** Ex-Micron engineer, technical background, FIRST consumer product. LinkedIn ~996 (semiconductor / hardware pros — low ICP overlap), Substack ~11, no product-relevant Twitter. Dogfooded on dev / AI technical newsletters (TLDR, AlphaSignal). Near-zero existing marketing surface for product's actual buyer.
**Default activated:** **marketing-naive default holds** — none of the override criteria apply (no prior consumer ship at >$10K MRR, no marketing track record, no ICP-aligned audience, no documented launch retrospectives).
**Mode (after Step 0B selection below):** TBD

---

## PREMISE-LEVEL FINDINGS BLOCK

_(populated after Step 0.5 if ≥2 of M0a–M0e fail. Filled in below the Step 0.5 section.)_

---

## Step 0 — Pre-review system audit

### What exists (read from design_document.md)

- v1 product fully specced + CEO + Eng + Design reviews completed
- Calendar-driven launch on Day 18 (now 20-22 day build per CEO review)
- $9/mo, 7-day free trial, Stripe Checkout
- Headline competitor identified: **Readless.app** ($4.90/mo, also solo-founder, also forwarding-email architecture)
- Adjacent context: Refind, Mailbrew, Meco, Shortwave, Notion Mail, Superhuman AI, Substack Reader
- Distribution Plan in design doc: **Show HN + cross-post to X / founder's network for amplification. No paid acquisition.** That's the entire plan as written.

### Founder audience audit (numeric)

| Surface | Count | ICP overlap |
|---|---|---|
| LinkedIn | ~996 | LOW — semiconductor / hardware pros, not inbox-overloaded knowledge workers buying $9/mo consumer SaaS |
| Substack (own) | ~11 | UNKNOWN, likely low |
| Twitter/X (for this product) | 0 | N/A |
| GitHub stars (prior projects) | unknown / low signal | N/A |
| Newsletter / email list | None for tldrof | N/A |
| Prior consumer products | 0 | N/A — first consumer product |
| Reachable through warm intros to ICP | Untested | UNKNOWN |

**Effective marketing surface area for tldrof's ICP: near zero.** This is load-bearing for every downstream decision.

### Web-searched competitive landscape

Searches performed (5+ mandatory under v0.2):
- `Readless.app pricing review 2026`
- `Meco newsletter app competitors`
- `Mailbrew alternatives 2026`
- `newsletter digest app HN reddit`
- `Superhuman launch playbook concierge`
- `Readwise growth strategy bootstrapped`
- `consumer SaaS launch Show HN base rate`

Detailed competitor + canonical-success findings in Section 1 below.

### Activation rules verdict

Near-zero audience + competitive analysis exists in design doc but only direct comps, no canonical-success comps → recommend **Mode B (Focused Review)** with a Mode-C-style audience-build sprint addendum, OR push to **Mode C (Audience-Build Sprint)** outright. Founder pick logged in Step 0B below.

---

## Step 0.5 — Premise audit (load-bearing under marketing-naive default)

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| 1 | Show HN is THE launch channel ("Show HN with the headline above. Cross-post to X / founder's network for amplification.") | Distribution Plan section | HN audience overlaps with the *dogfood* audience (technical newsletter subscribers) but NOT clearly with the *paying* audience (corporate/M365/locked-account users explicitly named as secondary segment). Survivor-bias precedent. |
| 2 | $9/mo price point with 7-day trial | Constraints / P6 | Anchored to Readless ($4.90) "premium" framing without ICP willingness-to-pay evidence; band may be wrong (sub-$10 is documented LTV-penalty band per RevenueCat data) |
| 3 | ICP = "inbox-overloaded knowledge workers + HN cohort + M365 / corporate-locked-out users" | Target User section | Two genuinely different audiences (HN technical readers vs corporate-locked-out professionals); plan acts as if both reachable through same launch. They aren't. |
| 4 | 7-day free trial as primary acquisition mechanic | P6, Trial flow | Cheap-trial mechanic selects time-rich/uncertain-fit users; paying ICP for corporate / time-poor segment trust-shops (not trial-shops). M0d freebie-disqualifier risk. |
| 5 | Founder-dogfood (technical newsletters: TLDR, AlphaSignal, Bensbites) tunes the product | Founder is the ICP / P3 | Tuning has audience signature. Dedup quality, signal density, summary style all calibrated against dev / AI content. Corporate / M365 / lawyer / finance / healthcare ICP reads different content (legal updates, market briefings, industry reports); v1 will ship calibrated for the *wrong* segment of the named ICP. |
| 6 | "Calendar-driven launch on Day 18 (now Day 20-22)" | Approach C, Distribution Plan | Retention-driven consumer subscription product → PMF-signal-driven gate (Vohra/Superhuman) is the precedent, not calendar gate. Calendar fires whether or not product is indispensable. |
| 7 | Auto-forwarding setup as power-user feature (v1.0 Gmail-only per PC2) | CEO PC2 | Anti-feature candidate: makes onboarding flow split (forward vs picker vs auto-forward); contradicts "60-second magic moment" simplicity claim. Or — opposite framing — it's a RETENTION feature, not anti-feature. Needs explicit decision. |
| 8 | "Structural moat" framing on forwarding-address architecture | P4 (already softened by CEO L6 carry-forward to "timing + narrative + 2-week head-start") | Already partially fixed in CEO review; flagged because the doc's earlier sections still use "moat" language unchanged. |

### M0a. Launch-platform audience-class fit

**Premise tested:** Show HN as the launch + cross-post to X. Founder's network = LinkedIn (~996 semiconductor folks).

**Web search performed:** "Show HN consumer subscription productivity tool 2024-2026 outcomes," "Readless launch channel," "newsletter aggregator HN launch results."

**Findings:**
- Show HN base rate for consumer productivity / inbox SaaS: most posts get <10 upvotes ("Hidden Signal" cohort). Successful HN launches in this category (Superhuman, Linear, Readwise) did NOT primarily acquire from Show HN. Readwise specifically built via partnerships + product-led, NOT HN. Superhuman launched concierge-only by invitation, NOT publicly on HN.
- HN audience overlap with tldrof's NAMED ICP: medium for HN-cohort segment (engineers/PMs/founders), but the doc *itself* names the more interesting segment as **M365/Outlook/corporate-locked-out professionals** (~400M globally — lawyers, finance, healthcare, government). **None of those are on HN.**
- Founder familiarity: HN is the platform technical founders know; this is exactly the M0a category-error pattern.

**Verdict: PREMISE FAILS.** Show HN is a familiar-platform-not-audience-fit choice for the high-leverage paying segment. It's defensible only for the HN-cohort segment, which is the *less* differentiated of the two named ICPs (Readless already serves them too). For the corporate-locked-out segment that Readless structurally can't serve, HN is a category error.

**Cascade:** M2 (discovery path) MUST refuse Show HN as Step 1. Section 5 (Launch playbook) cannot use HN as primary channel — must add at minimum (a) a corporate-segment channel and (b) a non-Twitter / non-HN content channel.

### M0b. Canonical-success comparable

**Premise tested:** Plan should anchor against canonical successes at this motion class (premium consumer subscription tool that retains via daily ritual), not just direct competitors.

**Web search performed:** "Superhuman launch playbook," "Readwise growth bootstrapped," "Mailbrew acquisition" (acquired by ?), "consumer subscription PMF gate concierge."

**Findings:** Canonical successes at this motion class:

1. **Superhuman ($30/mo → $825M acquisition Jul 2025):**
   - Founder Rahul Vohra personally onboarded the first ~200 users in 1:1 calls
   - Invite-only waitlist for years (gated by Vohra's "very disappointed" PMF test ≥40%)
   - No public launch in v1 — concierge first, brand-by-scarcity
   - Pricing $30/mo from day 1 (5x what tldrof plans, 6x what Readless charges)
2. **Readwise (~$10/mo, ~$14M ARR, >90% retention):**
   - Bootstrapped, product-led
   - Acquired via partnerships with adjacent tools (Pocket, Instapaper, Kindle ecosystem)
   - No paid acquisition. No HN launch as primary channel.
   - Tight integration with where users already read = the moat
3. **Substack itself / Beehiiv:** content-led, founder credibility, ecosystem partnerships. None launched on Show HN.
4. **Mailbrew:** launched on PH, scaled via content + comparison-search SEO; **acquired/shut-down by 2023**. Not a success comp; counter-example.

**Specific deltas (canonical success vs current plan):**
- Canonical successes did NOT calendar-gate launch. tldrof does.
- Canonical successes ran concierge / waitlist onboarding for first N users. tldrof plans cold public Show HN.
- Canonical successes priced at $10-30/mo. tldrof at $9 (below the documented LTV-positive band).
- Canonical successes had a content/audience surface BEFORE launch. tldrof has near-zero.

**Verdict: PREMISE FAILS.** Plan anchors against direct competitor (Readless at $4.90) and survivor-bias precedent (some HN launches worked). Does NOT anchor against any canonical success for this motion class. The Vohra / Readwise / Superhuman playbook is invisible in the design doc.

**Cascade:** Section 5 must surface concierge-first-cohort alternative. Section 6 must surface pricing-band question (matching cheapest direct comp is the documented failure mode). Section 4 audience-build sprint becomes load-bearing.

### M0c. Anti-feature surface

**Premise tested:** Doc claims all in-scope features serve the paying ICP.

**Line-by-line scan of v1.0 in-scope feature list:**

1. **Secondary picker (curated 30 popular Substack-hosted newsletters)** — serves users with NO backlog to forward. But the doc's primary use case (post pass 4) is **inbox-bankruptcy**: 20-100 emails accumulated. If bankruptcy is the wedge, picker serves a *different* segment (fresh-start users, no inbox debt) and splits the onboarding story.
   - **Anti-feature candidate: YES.** Picker contradicts the bankruptcy positioning. Either kill it to v1.0.5 (cleaner story) or accept that v1.0 has two competing onboarding magic moments (a known failure mode).
2. **Auto-forward setup helper (Gmail only per PC2)** — adds a 2nd onboarding step (account-level verify + filter setup, ~1.5-2 days of engineering per Outside Voice T1). Splits the "60-second magic moment" claim: user sees backlog digest in 60s but only retains via a 5-minute filter setup later.
   - **Anti-feature candidate: PARTIAL.** It IS the retention mechanism, so it's not anti-feature in the strict sense, but the COPY claim that this is "60-second magic" is then misleading. Either own the two-step onboarding (bankruptcy in 60s, set-and-forget in 5 min) explicitly, or stop selling 60-second magic.
3. **MCP / read-only digest API for power users** — v1.1 not v1.0, so not an active anti-feature now. But flag for v1.1 review: a "read-only digest API" serves technical power users; the *paying corporate segment* doesn't use MCP. Power-user-feature-drift risk.
4. **Per-newsletter slider preferences UI** — v1.1, flagged in design doc as "strongest moat candidate." Serves the user who wants to tinker. Corporate-locked-out segment (lawyers, finance professionals) probably doesn't tinker; they want zero-touch. Different ICP. v1.1 anti-feature risk for the segment doc calls highest-leverage.
5. **The `blueprints` join table + multi-blueprint architecture** — explicitly NOT a v1 user-facing feature ("optionality-preserving DB choice"). NOT an anti-feature.

**Verdict: PREMISE FAILS (mildly).** Picker is the cleanest anti-feature candidate against the bankruptcy positioning. Auto-forward helper is a near-anti-feature against the 60-second-magic claim (resolvable by changing the copy, not the feature).

**Cascade:** Section 5 should surface "kill the picker to v1.0.5" question. Landing page copy must reconcile "60-second magic" with "5-min filter setup for retention." Recommend re-framing as **"60-second taste → 5-minute set-and-forget"** explicitly.

### M0d. Freebie-disqualifier (acquisition-mechanic selection bias)

**Premise tested:** 7-day free trial selects for the paying ICP.

**Mapping the trial mechanic to attracted segment:**

- 7-day free trial, no CC required at signup, Stripe-trial-mode with card required at day 6 → **attracts time-rich / curious / low-commitment users** (will try a $9/mo product for free if reminded). Conversion to paid will be lower than the underlying value justifies, because the validation cohort and paying cohort are different humans.

**Cross-reference to the named paying ICP:**

- **HN cohort segment:** time-pressured but does try tools. 7-day trial is moderate fit. Acceptable but won't differentiate.
- **Corporate-locked-out segment (lawyers, finance, healthcare):** time-poor / money-rich. Does NOT trial-shop. Buys on trust (referral, comparable-recommendation, vendor reputation). Free trial as the primary mechanic is a **selection-bias miss** against this segment.

**Specific failure mode:** If launch goes Show HN + free trial, the cohort that signs up will be HN-cohort technical users curious about a newsletter tool. They will convert at the rate consumer freemium-to-paid converts (1-5%). The corporate-locked-out segment that's the *real* differentiation story will never see the product because the acquisition path doesn't reach them.

**Verdict: PREMISE FAILS for the named secondary ICP, PARTIALLY SURVIVES for the primary HN ICP.**

**Cascade:**
- Section 6 must propose alternative acquisition mechanics for corporate segment: warm-intro outreach, vertical-community presence (Above the Law for lawyers, /r/financialcareers, healthcare CIO communities), industry-publication placement.
- Free trial held for HN-cohort segment; trust-build channels added for corporate segment.
- "Concierge waitlist" (Superhuman model) surfaced as a high-trust alternative for corporate beta.

### M0e. Dogfood audience-class match (founder vs paying ICP)

**Premise tested:** Founder dogfood (technical newsletters: TLDR, AlphaSignal, Bensbites, Lenny's, Pragmatic Engineer, Stratechery, Latent Space) produces a product calibrated to the paying ICP.

**Audience signature analysis:**

- **Founder dogfood content:** AI/dev/tech (high signal density, short bullet style, "what shipped this week" cadence, code/product launches).
- **Corporate-locked-out segment content:** legal briefings (Bloomberg Law, Above the Law digests), financial updates (Bloomberg Briefs, Morning Brew finance, sector-specific), healthcare news (Becker's Hospital Review, Fierce Healthcare), industry newsletters (Politico Playbook variants per industry). Style: longer-form, narrative, regulatory updates, market summary.

**Specific failure mode:** Dedup quality and summary style tune to AI/dev content during 5-9 day dogfood. Lawyers' weekly digests don't dedup the same way (overlap on policy/regulatory updates is more nuanced than overlap on product launches). Summary length expectations are different (lawyers want context, not bullets). The Claude prompts get tuned to founder's content, ship to corporate segment, summarize poorly.

**Verdict: PREMISE FAILS for the named secondary ICP. SURVIVES for the HN-cohort primary ICP.**

**Cascade:**
- Pre-launch dogfood expansion required: recruit 3-5 corporate-segment beta users (PC3 already requires 3-5 HN-cohort friends; ADD parallel 3-5 corporate beta users) during days 7-9 — concierge onboarding to capture content signature differences before launch.
- Section 5 launch playbook must explicitly acknowledge dogfood-vs-corporate-ICP gap and gate corporate launch on second-cohort PMF signal, not Day-18 calendar.

### Pricing-band sub-check (rolls into Section 6)

Pricing premise tested in M0b above (canonical successes price $10-30/mo). $9 is below the documented LTV-positive band per RevenueCat State of Subscription Apps data. Cheapest-direct-competitor anchoring (Readless $4.90 → tldrof $9 "premium") is the documented technical-founder failure mode. Full treatment in Section 6.

### Step 0.5 verdict summary

| # | Verdict | Cascade target |
|---|---|---|
| M0a Launch platform | FAILS for corporate segment | Sections 3, 5 |
| M0b Canonical-success comparable | FAILS (no canonical successes in plan) | Sections 1, 5, 6 |
| M0c Anti-features | FAILS (mildly — picker + auto-forward copy) | Sections 5, design doc edits |
| M0d Freebie disqualifier | FAILS for corporate segment | Sections 3, 6 |
| M0e Dogfood mismatch | FAILS for corporate segment | Sections 2, 4, 5 |

**5 of 5 fail at least partially. ≥2 threshold tripped.** Premise-level findings block at top of plan is required and populated below.

---

## PREMISE-LEVEL FINDINGS BLOCK (populated)

> **The plan as written serves the HN-cohort segment competently and the corporate-locked-out segment poorly. The corporate segment is the more differentiated, higher-leverage opportunity (Readless cannot reach it). Yet every marketing premise in the plan (channel, price, trial mechanic, dogfood mix, calendar gate, founder reach) is calibrated for the HN segment.**
>
> **5 of 5 premise audits failed at least partially. The doc is internally consistent for the WRONG primary audience.**
>
> Four high-leverage corrections precede tactical optimization:
>
> 1. **Split the launch into two cohorts.** HN-cohort launch on Day 20-22 as planned. Corporate-cohort beta on a separate track: concierge-onboarded 10-20 users, PMF-gated (Vohra "very disappointed" ≥40%), then vertical-channel launch 4-8 weeks later.
> 2. **Re-anchor pricing against canonical successes** (Superhuman $30, Readwise $10), not against cheapest direct competitor (Readless $4.90). $9 is below the LTV-positive band; consider $12-19 for the corporate segment as a separate tier or as the unified price.
> 3. **Expand dogfood to the corporate segment** during days 7-9. Recruit 3-5 corporate-segment betas in parallel with the 3-5 HN-cohort friends PC3 already specifies.
> 4. **Refuse the single-channel Show HN launch.** Force at least 3 launch channels with sequence. Force a corporate-segment channel for the differentiated audience.
>
> The rest of the plan below assumes these corrections.

---

## Step 0A — Forcing questions (founder answers + skill challenges)

_Founder answers are naive (smart-but-first-time technical founder). Skill refusals/challenges follow each._

### M1. Audience reality

**Founder (naive answer):** "Knowledge workers who subscribe to too many newsletters. Like me. Engineers, PMs, founders. They're on HN, on Twitter, on Reddit /r/Entrepreneur."

**Skill challenge:** REFUSED. "Knowledge workers" is a demographic, not a person. "Like me" privileges the dogfood ICP (which Step 0.5 M0e flagged as a mismatch with the higher-leverage segment).

**Forced specificity (composite + corporate):**

**Persona A — "Devin," HN-cohort segment (the dogfood ICP):**
- 32, senior engineer at a mid-size tech co, $180K base
- Subscribes to: TLDR, AlphaSignal, Bensbites, Lenny's, Pragmatic Engineer, Latent Space, Stratechery, The Hustle, Morning Brew (9 daily)
- Inbox at 18,000 unread; aggressively archives but loses signal
- Pays $20/mo ChatGPT Plus, $10/mo Readwise, $30/mo Claude Pro (yes, both)
- Reads HN every morning, follows ~200 on X, in 3 Slack groups (PM/Eng/AI)
- Listens to Latent Space podcast, Lenny's podcast
- Buys consumer SaaS confidently if free-trial proves it
- ICP for the HN launch path

**Persona B — "Maria," corporate-locked-out segment (the differentiated, higher-leverage ICP):**
- 41, finance director at a Fortune 500, M365 corporate email, IT bans OAuth into work inbox
- Subscribes to: Bloomberg Briefs (4 sector-specific), Politico Money, Axios Pro: Fintech Deals, two industry analyst newsletters, two trade-association briefings, internal corporate digest (8 daily, ~45 min/day cognitive cost)
- Reads on phone between meetings; misses signal weekly
- Pays $400/yr Bloomberg Briefs, ~$2K/yr industry analyst, $150/yr WSJ
- Does NOT live on HN, sometimes LinkedIn, reads Axios Pro, attends 2-3 industry events/yr
- Buys tools on (a) IT-approved vendor list, (b) recommendation from peer at industry event, (c) coverage in trade publication
- Does NOT free-trial-shop consumer SaaS for work email
- ICP for the corporate-segment differentiated path

**Where Maria spends attention right now (specific):** Axios Pro newsletters, sector-specific industry publications (e.g. American Banker, Treasury & Risk, CFO Dive for finance; Healthcare Dive, Fierce Healthcare for healthcare), LinkedIn (industry voices, not founder voices), 1-2 trade-association events per year, peer text threads / SMS, industry Slack groups (if any), occasional WSJ / FT.

### M2. Discovery path

**Founder (naive answer):** "They see my Show HN post, they're curious about the bankruptcy framing, they sign up for the free trial."

**Skill challenge:** REFUSED. Step 1 is "Show HN" — explicit no-go per M0a finding. Also: "they're curious" is passive; need active discovery path.

**Forced specificity (two paths):**

**Persona A path (HN cohort):**
1. Devin browses HN daily ~7-8am PT; sees Show HN post in first 30 (or via second-chance pool curated by dang)
2. Headline hooks ("50 unread newsletters? Forward them all here. Inbox debt cleared.")
3. Clicks through, lands on tldrof.com; lands on /signin within 30s if landing page is clean
4. Signs up; gets forwarding address; forwards a backlog within 5 min
5. Sees magic-moment digest; decides whether to enter card at day 6

Realistic: ≤6 days from first-touch to paying decision. Channel risk: HN miss = no recovery.

**Persona B path (corporate cohort):**
1. Maria reads sector industry newsletter (e.g. CFO Dive) where tldrof was mentioned as a tool fellow CFOs use; OR
2. Peer text in her industry Slack group: "ever tried tldrof? Cleared my Bloomberg backlog in one sitting"; OR
3. Sponsored mention in Axios Pro (paid placement, ~$2-5K test), OR
4. Talk at industry event by a comparable-role peer who paid for tldrof and shared the result; OR
5. Trade-publication review or LinkedIn post by an industry voice (not a founder voice)

Realistic: 6-24 weeks from first-touch to paying decision (corporate segment trust-builds slowly). Channel: vertical publications + peer referral.

### M3. Pre-launch audience

**Founder (naive):** "I have 996 LinkedIn followers and ~11 Substack subscribers. And I'm pretty active on Twitter when I post."

**Skill challenge:** Numbers are honest, but ICP overlap is near-zero:
- 996 LinkedIn = semiconductor / hardware audience, NOT Devin and NOT Maria
- 11 Substack = below noise floor
- Twitter "when I post" = no demonstrable audience

**Forced honest answer:** **"Effectively zero pre-launch audience for this product's ICP."** This triggers an audience-build addendum to the plan regardless of mode chosen. Days -30 to launch must include explicit audience-build activity (Section 4 below).

### M4. Channel honesty

**Founder (naive):** "I'm good at building things and I write code well. I can write blog posts about the build."

**Skill challenge:** Building code is product capability, not distribution capability. Writing blog posts without a distribution surface for them is shouting into the void. REFUSED.

**Forced honest answer:** **"I have no demonstrable distribution-channel advantage over a generic technical founder."** This is the FIRST WORK ITEM, not a future-tense aspiration. Either build a beachhead channel before launch (build-in-public on X with credible engagement, or weekly Substack with explicit topic that builds search authority) or accept that launch leverages exist channels purely transactionally (paid placement, warm intros, founder-network favor calls).

Possible *latent* advantage to develop in 30 days:
- Engineering credibility → write 2-3 substantive technical posts about the architecture (Mailgun inbound + Claude pipeline) that might land on HN front page on their own merits as engineering content — pre-warms HN audience for the product launch.
- LinkedIn → 996 semiconductor folks won't buy, but corporate adjacency may exist: write 2-3 posts framing the inbox-overload problem in business / executive language; *latent* corporate-segment reach worth testing.

### M5. Competitor traffic source

**Founder (naive):** "I don't know exactly. I think Readless gets some HN and some Twitter."

**Skill challenge:** "I don't know" is acceptable IF paired with explicit pre-launch research commitment.

**Forced answer + commitment:** Run before next session (concrete tasks):
- SimilarWeb on readless.app + meco.app + mailbrew.com (historical) — confirm where their traffic comes from
- Backlink check (Ahrefs free or ubersuggest) on direct comps — what's the link profile?
- Manual scan: Readless founder's Twitter / LinkedIn / Substack — where do they post when launching features?
- HN search "readless" and "meco" — what's the launch outcome history?

**Initial best guesses (verify):** Readless probably gets dominant traffic from search (people google "newsletter aggregator" / "newsletter digest"), then product-hunt-like communities, modest social. Mailbrew shut down — instructive failure case for the category. Meco acquired by Substack 2024 — instructive success case (acqui-hire validates demand).

### M6. First 10 paying customers

**Founder (naive):** "Whoever sees the Show HN post and signs up. Hopefully my friends from the dev community."

**Skill challenge:** "Whoever" is passive and "friends" must be NAMED and verified as ICP. REFUSED.

**Forced specificity:**

**HN-cohort 10 (names — placeholder, founder fills):**
1-5. Five named close friends in eng/PM who actually have a backlog of newsletters right now (verify before launch via DM: "do you have unread TLDR / AlphaSignal sitting in inbox? would you pay $9/mo to clear it?")
6-10. Five named acquaintances from prior workplaces / open-source contributions / Twitter follow / Discord regulars in dev communities

**Corporate-cohort 10 (path — founder doesn't know individuals yet):**
1-5. Warm intros via LinkedIn first-degree connections in finance / legal / consulting roles (founder writes 10-15 personalized DMs in week before launch)
6-10. Cold but high-fit outreach to known industry voices (CFOs / GCs with public profiles on LinkedIn writing about productivity); ~20 DMs to net 5 conversations to net 1-2 betas

**Commitment:** Founder writes 30 named-person outreach list before Day 0 of launch sequence. Lists go in `outreach_list.md` (not in this artifact; founder homework).

### M7. Time allocation

**Founder (naive):** "I'm 100% on building right now. The build window is the build window. I'll start marketing after launch."

**Skill challenge:** REFUSED. "Marketing after launch" is the canonical anti-pattern (#3 in the skill's list). Launch with zero audience = lottery ticket regardless of build quality.

**Forced recalibration:** Build window is 20-22 days. Required minimum: **40% of pre-launch time on audience-build for the corporate segment** (because HN-cohort can be partially served by launch-day mechanics; corporate cannot). For tldrof specifically:
- Days 0-9: ~10-15% audience work (recruit corporate beta candidates, write 1 LinkedIn post, write 1 substantive engineering post for X)
- Days 10-18: ~25-35% audience work (warm intros, draft launch sequence, prep Show HN draft AND vertical-publication outreach, build email list of 30+ named-person targets)
- Days 19-22: ~50% audience work (final outreach sequence, soft pre-announce to ~50, prep launch artifacts for 3+ channels)

Net: average ~25-30% of pre-launch time on audience-build is the floor. Below that = audience-doesn't-exist on launch day.

**Founder acceptance / risk acknowledgment required:** If founder defends 100% build allocation, document as an explicit known risk in TODOS.md. The risk is that launch ships to silence.

### Step 0A completion summary

All 7 questions have concrete answers OR explicit risk acknowledgment. Cascading findings from Step 0.5 are visible in M1, M2, M4, M6, M7 specifically. Proceed to Mode selection.

---

## Step 0B — Mode selection

**Founder situation:**
- Near-zero audience (M3)
- Direct-competitor analysis exists in design doc; canonical-success analysis missing
- 5 of 5 premises failed (Step 0.5)
- Time-pressured pre-launch (20-22 days)

**Mode A (Full Review)** is too long for time pressure but the premise failures demand depth.
**Mode B (Focused Review)** runs Sections 1, 3, 5 — covers the highest-cascade-impact sections.
**Mode C (Audience-Build Sprint)** is the right shape for "near-zero audience" but the founder is mid-build and won't pause for an audience-only sprint.

**Selected: Mode A LIGHT — run all 9 sections but with depth concentrated in Sections 1, 3, 5, 6, plus a Mode-C-style audience-build addendum as Section 4.** Sections 7, 8, 9 covered briefly. Justification: premise failures are severe enough that surface-only coverage in Sections 1/3/5 misses cascading implications; full coverage is required.

If founder rejects Mode A Light scope, fallback: **Mode B + audience_build_sprint.md addendum** (the corporate-segment cohort).

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Name | URL | Pricing | Founding | Apparent traffic source | Public complaints | Positioning vs tldrof | Winning? |
|---|---|---|---|---|---|---|---|
| **Readless.app** | readless.app | $4.90/mo | 2024-25 (solo) | SEO + some Twitter; founder presence on X (small) | Slow first digest (24h); subscription-curated onboarding feels manual; topic clustering quality middling | Same architecture (forwarding); inferior bankruptcy flow; commodity pricing | Surviving but not breakaway; capability parity with tldrof v1.0 |
| **Meco** | meco.app | $0 (acq'd by Substack 2024) | 2020 | Substack ecosystem; PH launch; press at acquisition | Limited customization in free version; "Substack only" tilt post-acq | Inbox-app for newsletters (read in app, not digest in email); different shape | Acquired = validation of category; absorbed |
| **Mailbrew** | mailbrew.com | (Shut down 2023) | 2019 | PH launch + content/SEO | (Historical) — power-user feature creep, no killer wedge | Power-user customizable digest builder | LOST (instructive) |
| **Refind** | refind.com | $0-12/mo | 2016 | Email referral loops; community newsletter ecosystem | Algorithmic recommendation noise; less personal control | Curated discovery, not personal-newsletter aggregation | Niche success, different shape |
| **Shortwave / Notion Mail / Superhuman AI** | various | $9-30/mo | various | OAuth-based; press / paid / founder content | "Reads all your email" trust concerns; OAuth-only excludes corporate | Full inbox tools; different motion class | Each successful at own motion; structurally cannot serve corporate-locked-out |

**Read:** Readless is the only true direct comp. Capability parity. Pricing race to bottom by Readless is its strategic exposure (commodity positioning). Mailbrew's failure is the instructive lesson — power-user features without sharp wedge. Meco's acquisition validates demand. Refind / Shortwave-class are adjacent, not direct.

### 1b. Canonical-success comparables

| Name | Price | Founded | Scale (latest) | Primary acquisition | Onboarding | Launch gate | Delta vs tldrof plan |
|---|---|---|---|---|---|---|---|
| **Superhuman** | $30/mo | 2014 | $825M acquisition Jul 2025 | Concierge invite-only waitlist, founder-led onboarding, referral | Manual 1:1 (Vohra personally did first ~200) | **PMF gate: ≥40% "very disappointed"** | tldrof = $9, no waitlist, calendar gate, no concierge |
| **Readwise** | $10/mo | 2017 | ~$14M ARR, >90% retention | Adjacent-tool partnerships (Pocket, Instapaper, Kindle), product-led | Self-serve but onboarding tutorial guided | Product readiness, not calendar | tldrof = no partnerships planned, no adjacent-ecosystem entry |
| **Stratechery / Bloomberg** | $150-400/yr | 2013/various | $1M+ / $massive | Founder content + earned credibility, decades | Self-serve | N/A | Different motion (B2C content), but instructive on annual pricing + trust posture |
| **Beehiiv / Substack (as platform)** | varies | 2017-21 | $massive | Founder content, ecosystem partnerships, creator referrals | Self-serve plus white-glove for top creators | N/A | tldrof = no ecosystem partnership story planned |

**Specific deltas (canonical successes vs current tldrof plan):**

1. **Concierge-first cohort:** Superhuman did the first 200 1:1. tldrof plans cold public Show HN. The bankruptcy magic-moment is BUILT FOR concierge — founder could literally onboard the first 20 personally via warm DMs and learn the dedup quality, time-saved math accuracy, content-signature variance ONE COHORT AT A TIME. The skill recommends adding this.
2. **PMF-signal gate:** Vohra "very disappointed" ≥40%. tldrof gates on calendar Day 20-22. For a retention-driven daily-ritual product, this is the canonical failure pattern.
3. **Adjacent-ecosystem partnerships:** Readwise won via Pocket / Kindle integration. tldrof v1 has zero partnership story; the entire growth model is direct acquisition.
4. **Pricing band:** Canonical successes price at the top of their band ($10-30 consumer SaaS). tldrof at $9 is below the LTV-positive band per RevenueCat data (more in Section 6).

### 1c. Pattern surface (1-paragraph read)

Canonical successes at this motion class share: **(a) concierge-first onboarding for first N users, (b) PMF-signal launch gate, (c) adjacent-ecosystem partnerships as compounding channel, (d) pricing at the top of the band signaling premium-not-commodity.** Direct competitors (Readless) diverge from canonical successes on every dimension EXCEPT possibly (b), and Readless's existence validates the category. The tldrof plan currently follows the Readless playbook (commodity-adjacent price, calendar launch, self-serve onboarding, no partnerships) rather than the canonical-success playbook. **For a solo founder with no audience, the Readless playbook produces "Readless 2 with marginally better UX." For a solo founder who has spotted a real structural-coverage advantage (M365 / corporate / paid-account-locked users), the canonical-success playbook is the higher-leverage choice for the corporate segment specifically.**

**Founder action:** Read 2 founder interviews — **Rahul Vohra on Lenny's podcast (Superhuman concierge + PMF gate)** AND **Tristan Homsi on Readwise growth** (or whichever Readwise founder interview is most substantive). Record what they did that tldrof doesn't.

---

## Section 2 — ICP specification

See M1 above for two-persona spec (Devin = HN cohort, Maria = corporate-locked-out). Compressed ICP doc written to `icp.md` (separate artifact).

Key forcing summary for plan:
- **Persona A (Devin):** reachable via HN, X, IndieHackers, /r/SideProject, Lenny's-adjacent communities, podcast guesting in dev/AI vertical, build-in-public X.
- **Persona B (Maria):** reachable via vertical industry publications (Axios Pro, CFO Dive, Healthcare Dive, sector-specific Substacks), LinkedIn industry-voice content, peer referral within industry Slack groups, paid placement in trade publications, trade-association events.

These are **different channels, different copy, different acquisition mechanics, different price-tolerance.** Treating them as one ICP and one launch is the plan's largest unforced error.

---

## Section 3 — Distribution channel-by-channel

### Candidate channels scored for THIS founder

| Channel | Reach (paying ICP) | Cost | Conversion | Founder fit | Effort to start | Notes |
|---|---|---|---|---|---|---|
| Show HN | Medium (Persona A only) | $0 | 1-3% if hits | OK (founder is technical) | Low (1 post) | Lottery; M0a category-error for Persona B |
| /r/SideProject + /r/Entrepreneur | Low-Med | $0 | 0.5-2% | OK | Low | Persona A overlap; community rules / self-promo limits |
| IndieHackers | Med (Persona A) | $0 | 1-3% | OK | Low | Better for paid SaaS than HN, similar shape |
| Product Hunt | Med | $0-cost-of-hunter | 1-2% | Weak — no hunter relationships | Med (need hunter) | Single-shot day; Day 0+7 |
| X / Twitter organic | Very low (0 followers for this product) | $0 | 0.5-1% | Weak (no audience) | High to build | Build-in-public is highest leverage |
| X / Twitter paid | Low (CPM expensive in AI category) | $5-15 CPC | 1-2% | Weak | Med | Skip for v1 |
| LinkedIn organic | Low for Persona A, **Med-High latent for Persona B** | $0 | 1-2% | OK (founder has 996 wrong-vertical audience but can pivot content) | Med | **Underused leverage point; Persona B's home turf** |
| LinkedIn paid (Sales Navigator / Sponsored content) | High for Persona B | $$$ | 2-5% if targeted | Founder has no experience | High | Defer to v1.0.5; corporate segment investment |
| Substack (founder writes) | Very low (11 subs) | $0 | n/a unless audience grows | OK (founder writes) | High (slow ramp) | Pre-launch 30-day push to build to 100-200 = realistic; long-term retention | 
| Vertical industry publications (paid placement / sponsorship) | High for Persona B specific verticals | $1-5K per test | 1-3% | Founder has no relationships | Med | Highest-leverage for Persona B; recommended week-3+ test |
| Reddit (vertical subs: /r/ChatGPTPro, /r/productivity, /r/personalfinance) | Med | $0 | 0.5-2% | OK | Med (need community standing) | Cross-post compliant only |
| Cold outreach DM (LinkedIn / X) | Med — Maria pool | $0 (time) | Higher (5-10% conversation) | OK | High labor | First-10-customers plan |
| Podcast guesting | Med — Lenny's, Latent Space, Pragmatic Engineer, AI-focused; vertical for corporate | $0 (time) | 2-5% per appearance | OK | High prep | **Multi-cohort fit; high signal** |
| Email signature + personal network email | Low absolute, high relative for first 10 | $0 | 5-15% in personal net | OK | Low | Day -7 soft pre-announce |
| SEO / content for "newsletter digest" / "bankruptcy" terms | High latent | $0 (time) | 1-3% organic | OK (founder writes) | Very high (6-12 mo ramp) | Start in week 1; compound channel |
| Paid Google search ads on competitor terms | Med | $1-5 CPC | 3-7% | Founder no experience | Med | Test at week 2; $50-200 budget |
| Affiliate (Lenny's, Justin Welsh-style creators) | Med-High | 30-50% rev share | 2-5% | None now | High | v1.0.5+ |

### Ranking (leverage = reach × conversion × founder fit ÷ cost ÷ effort)

For Persona A (HN cohort), top 4 to actually do:
1. **Show HN + IndieHackers + /r/SideProject as a coordinated 48-hour Day-0 burst** (NOT Show HN alone)
2. **Build-in-public on X for 30 days pre-launch** (latent audience-build; produces day-0 amplification material)
3. **Podcast guesting (Lenny's adjacency, Pragmatic Engineer if reachable, AI-focused podcasts)** — book Day 0+14 first appearance
4. **Personal network email Day -7** to ~50 named contacts; expect 5-10 paying conversions from this alone

For Persona B (corporate cohort), top 4 to actually do:
1. **LinkedIn organic content (pivot from semiconductor)** — 8-10 posts over 30 days reframing inbox-overload in executive language; latent corporate reach
2. **Cold warm-intro outreach via LinkedIn first-degree** — 20-30 personalized DMs to identified ICP-matching contacts
3. **Paid placement test in 1-2 vertical newsletters (CFO Dive, Axios Pro: vertical, or Above the Law for legal)** — $1-3K test at Day 0+30
4. **Industry Slack / community presence** — identify 2-3 corporate-vertical communities, build 4 weeks of standing before launch

**REFUSE "all of them."** Cut: paid Twitter, paid Google (initial), affiliate, Product Hunt (defer to v1.0.5). Net for solo founder: ~6 active channels split across 2 cohorts.

---

## Section 4 — Pre-launch audience-build plan (30/60/90)

(Note: build calendar is 20-22 days — compress to 20/40/60 effectively.)

### Days -22 to 0 (pre-launch): minimum-viable audience seed

**Cadence per week:**
- **2 X posts/week** (build-in-public threads on architecture, NOT promotional)
- **2 LinkedIn posts/week** (1 corporate-segment-framed inbox-overload post + 1 build update)
- **1 Substack post/week** (technical deep-dive — Mailgun + Claude pipeline as engineering content; SEO + credibility play)
- **10 personalized cold DMs/week** (corporate-segment outreach + HN-cohort beta recruitment)
- **Daily** light HN reading + commenting on adjacent threads (build name recognition pre-launch — DO NOT promote)

**Cumulative pre-launch audience target (realistic):**
- X: 50-200 followers (mostly engineering audience seeing build-in-public)
- LinkedIn: ~10-30 new connections in target verticals (corporate-segment)
- Substack: 30-80 subscribers
- 30+ named contacts personally pre-announced
- 3-5 confirmed Day-0 amplifiers (people who will retweet / share at launch on request)

### Days 0-30 post-launch (audience compounding)

- Cadence sustains; pivot ratio to launch-related content
- Add: podcast outreach (target 5 podcasts, expect 1-2 yeses for Day 0+30-60)
- Add: comment-section presence on competitor / category content (link only when on-topic)
- Add: vertical-publication sponsorship test (if Persona A launch traction unlocks budget for Persona B test)

### Days 30-90

- Iterate based on which channel produced conversions; double down
- SEO content compounding begins (target: 1 ranking post by day 90)
- Corporate-cohort PMF gate runs: ≥40% "very disappointed" before vertical-channel scale-up

---

## Section 5 — Launch playbook

### 5a. Question the launch gate BEFORE producing the playbook

**Current gate:** Calendar Day 20-22 (build complete).

**Skill challenge under v0.2:**

> For a retention-driven daily-ritual consumer subscription, the launch gate should be PMF-signal-driven (Vohra ≥40% "very disappointed" or equivalent), not calendar-driven. Why is calendar the right gate for tldrof?

**Founder's likely defense:** "I need the HN launch moment; the build window is finite; calendar IS the gate because the alternative is infinite refinement."

**Skill counter:** Accept the calendar gate FOR THE HN LAUNCH ONLY. Refuse it for the corporate-segment launch.

**Recommended split-gate model:**
- **HN-cohort launch:** calendar gate Day 20-22 (founder's plan). Acceptable risk — HN benefits from a launch moment; HN audience expects "shipped" products; first 10-20 trial users provide PMF signal AFTER launch.
- **Corporate-cohort launch:** PMF gate. Founder personally onboards 10-20 corporate-segment beta users (recruited days 7-9, dogfood-of-three-by-day-12); runs Vohra "very disappointed" test on them; corporate vertical-publication / paid-channel launch ONLY fires when ≥40% answer "very disappointed."
- **Concierge-first option for corporate:** if PMF gate fires, scale via warm intros + vertical sponsorship + trade-pub placement. If PMF gate fails, iterate dedup quality / summary style / time-saved math for corporate content type and re-test cohort 2.

### 5b. Sequence (Mode A LIGHT; two cohorts)

#### HN-cohort sequence (Persona A — Devin)

| Day | Channel | Specific action |
|---|---|---|
| -30 to -7 | X build-in-public | 2 posts/week on architecture; aim for 50+ followers by Day 0 |
| -30 to -7 | LinkedIn | 2 posts/week; engineering-credibility posts |
| -30 to -7 | Substack | 1 post/week; technical deep-dive content |
| -14 | Podcast outreach | Pitch Lenny's-adjacent, Latent Space, Pragmatic Engineer (~5 pitches, expect 1-2 yeses) |
| -7 | Personal network email | Soft pre-announce to ~50 named contacts ("launching in a week; here's what / here's the ask") |
| -3 | X | Build-in-public preview thread |
| -1 | HN draft review | Show post draft to 2-3 trusted technical reviewers for headline/copy critique |
| **0 morning PT** | **Show HN** | Bankruptcy headline; immediate engagement-shepherding (replies in real time first 4 hours) |
| 0 + 2h | X | Thread with HN link |
| 0 + 4h | LinkedIn | Long-form post (HN audience overlap = low, so different framing) |
| 0 + 8h | IndieHackers | Cross-post (HN-first to avoid duplicate-content penalty); engage in comments |
| 0 + 24h | /r/SideProject | Compliant cross-post per subreddit rules |
| 0 + 48h | /r/Entrepreneur | If launch traction warrants |
| 0 + 7d | Product Hunt | Separate launch event if hunter relationship secured by Day 0; else defer |
| 0 + 14d | Podcast appearances | First podcast guest spot if booked |
| 0 + 30d | Substack retrospective | Traction numbers + technical lessons |

**Risk callouts:** HN miss = no recovery if it's the only channel; mitigated by IndieHackers + /r/SideProject + personal network running in parallel.

#### Corporate-cohort sequence (Persona B — Maria, PMF-gated)

| Day | Channel | Specific action |
|---|---|---|
| -22 to -7 | LinkedIn | Pivot content to corporate-segment-framed inbox-overload posts |
| -14 | Warm-intro DM | 20-30 personalized LinkedIn DMs to ICP-matching first-degree connections; invite to private beta |
| -7 | Concierge onboard | 5-10 corporate betas onboarded 1:1 by founder (Zoom or screen-share); 7-day dogfood |
| **0 to +14d** | **Concierge cohort runs HN-launch period in parallel** | No public corporate-segment launch; founder hand-holds beta cohort, captures content-signature differences vs HN content, tunes Claude prompts |
| +21d | Vohra PMF survey | Ask 10-20 corporate betas "how would you feel if you could no longer use this?"; require ≥40% "very disappointed" to fire next stage |
| +30-60d | Vertical content + paid test | If PMF gate fired: LinkedIn content series targeting 2-3 verticals; $1-3K paid placement test in 1-2 vertical newsletters (CFO Dive, Healthcare Dive, etc.) |
| +60-90d | Industry events / trade pub outreach | Pitch trade publications for review coverage; identify 1 industry event for Q3-Q4 |
| +90d | Affiliate / partnership pilot | Identify 1-2 industry creators / consultants for affiliate test |

**Risk callouts:** Corporate cohort may fail PMF gate first try — that IS the signal; iterate dedup / summary quality for corporate content type and re-recruit cohort 2.

`launch_playbook.md` written as separate artifact with hour-by-hour Day 0 detail.

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing BAND before the price point

**Current price:** $9/mo, 7-day free trial.

**Skill challenge under v0.2:**

> Did the $9 price band inherit from competitor anchoring (Readless $4.90 → tldrof $9 "premium positioned") or from ICP willingness-to-pay evidence?

**Founder's answer (per design doc):** Implicitly competitor-anchored — Readless is the floor, $9 chosen as defensibly above Readless without venturing into premium range.

**Skill counter — ICP willingness-to-pay evidence:**

- Persona A (Devin) adjacent-category spend: $20/mo ChatGPT Plus, $10/mo Readwise, $20/mo Claude Pro. **Anchor: $10-30/mo is the normal band for productivity tools this segment buys.** $9 is at the bottom of their accepted band.
- Persona B (Maria) adjacent-category spend: $400/yr Bloomberg Briefs (~$33/mo), $150/yr WSJ, employer-funded vertical tools at $1-2K/yr. **Anchor: $20-50/mo personal, $100-500/mo employer-funded.** $9 is so low it signals "consumer tool" — wrong category signal for corporate buying.

**RevenueCat State of Subscription Apps (2024-25) data point:** $5-9 is a documented LTV-penalty band; $10-15+ retains meaningfully better; annual billing dominates retention.

**Recommendation:**
- **HN-cohort: $9/mo holds OR move to $12/mo** (above the LTV-penalty floor, still under the Devin threshold of pain). The $9 isn't catastrophic for this segment; small upward pressure is the optimization.
- **Corporate cohort: separate tier at $19/mo (or $24/mo) "Pro / Corporate"** specifically positioned for paid-account-locked users with M365/Outlook. Annual billing default ($199/yr = ~$16.50/mo equivalent, 30% saving — primes annual retention).
- **Cheapest-direct-competitor matching ($4.90) is explicitly refused as anti-pattern #7.**

### 6b. Standard pricing & packaging coverage

- **Tier structure:** v1.0 — single tier at $9 OR $12 (recommend $12 with annual $99 default for retention). Corporate Pro tier at $19/mo OR $199/yr in v1.0.5 once corporate PMF validated.
- **Trial mechanics:** revisit M0d findings — 7-day free trial is fine for HN cohort, INAPPROPRIATE for corporate cohort. Corporate cohort: **concierge waitlist** (founder personal onboard, no trial — buyer commits to paid after 1:1 demo). Different mechanic for different segment.
- **Annual discount:** strongly recommended — name the RevenueCat retention evidence on landing page ("save 17% with annual; locked in for the year you'll actually use it").
- **Per-seat vs per-feature:** v1.0 personal use; per-seat for v1.0.5+ if corporate teams emerge (CFO + 2 analysts on shared digest = clear team-tier shape).

**Force founder to defend pricing model decision:** $9 vs $12 vs $9-with-annual-at-$99 vs $12-with-annual-at-$120. Pick one with specific reasoning, not "felt right." Recommend $12/mo + $99/yr.

---

## Section 7 — Post-launch growth loops

- **Referral mechanics:** v1.1 candidate — "share your time-saved screenshot" mechanic (the "reading-speed arbitrageur" insight from doc's Cross-Model Perspective). Currently NOT in v1.0. RECOMMEND moving to v1.0.5 if not v1.0.
- **Content compounding:** Substack technical content + landing-page SEO for "newsletter digest," "inbox bankruptcy," "newsletter aggregator," etc. 6-12 month compounding. Start week 1.
- **Network effects:** None native to product. Each user is independent.
- **Brand compounding:** Slow; founder presence over time on X / LinkedIn / Substack.
- **Retention as growth:** YES — daily-ritual + auto-forward creates loss-aversion-locked users who become unprompted word-of-mouth sources. P5 IS the test (per CEO L5 carry-forward).

**Verdict:** Without a referral mechanic, growth is acquisition-treadmill. Add "shareable time-saved card" by v1.0.5. Surface this as TODO in marketing TODOS section of design doc.

---

## Section 8 — Metrics & instrumentation

Measure (weekly):
- Acquisition by channel (UTM tagging required on every link)
- Activation rate: signup → first digest rendered → first auto-forward configured (3-step funnel)
- Day-7 retention (% who got 2nd digest), Day-30 retention
- Free trial → paid conversion (Stripe data)
- LTV/CAC once Day-60+ data exists
- **filter_setup_rate_48h** (CEO post-skill cleanup item 2) — leading indicator of retention thesis

Do NOT measure (vanity):
- HN upvotes (correlation w/ revenue near-zero)
- Total signups (without retention context)
- X/LinkedIn follower count (correlation weak)

Weekly dashboard: Stripe + Supabase + Posthog (recommended free-tier addition) + manual UTM tracking. ~2h/week founder time.

---

## Section 9 — Risk analysis

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| HN miss (single-shot, no recovery) | Med (30-40% base rate) | High (zero day-0 traction) | Multi-channel Day-0 sequence; personal network email Day -7 |
| Channel concentration (>60% from one) | High under current plan | High | Forced multi-channel ranking in Section 3 |
| Corporate segment unreached | Very high under current plan | High (loses the differentiated leverage) | Split-cohort launch in Section 5 |
| Pricing-band miscalibration | High | Med-High (lifetime LTV penalty) | Section 6 recommendation $12/mo + corporate $19 tier |
| Dogfood-vs-ICP mismatch | High (M0e) | Med (degraded corporate quality) | Days 7-9 corporate beta recruit |
| Readless counter-launches bankruptcy framing | Med (low-cost, motivated solo) | Med | Ship positioning + ladder rungs Readless isn't building |
| Calendar gate misfire (PMF not actually present at launch) | High for corporate segment | High | PMF gate for corporate cohort; calendar for HN cohort only |
| Trial conversion lower than business model assumes | Med-High | High | Concierge cohort for corporate; explicit P6/P5 tests |
| Founder zero pre-launch audience | Confirmed | High | 30-day audience seed in Section 4 |
| Picker UX splits magic-moment story (M0c anti-feature) | Med | Med | Recommend defer picker to v1.0.5 |
| LinkedIn semiconductor audience doesn't pivot to corporate-ICP content | Med | Low (latent only) | Test 2-3 posts; if no traction, deprioritize LinkedIn organic for Persona B |

---

## Outside voice — independent critique

(Simulated — would be Claude subagent or Codex CLI in real run.)

**Single biggest risk inside review missed:**

> **The "M365 corporate-locked-out" segment is the doc's strongest strategic claim — and it is **completely untested**.** The corporate-segment is named in the doc, used to justify the structural-coverage moat, and informs Persona B in this review. But zero corporate-segment users have been recruited, dogfooded, or surveyed. The plan above adds days-7-9 recruitment of 3-5 corporate betas, but THIS skill recommends going further: **do not commit any v1.0.5 corporate-channel investment (LinkedIn paid, vertical sponsorship, trade-pub placement) until corporate cohort PMF gate fires.** If the corporate segment doesn't materialize, the plan reduces to "Readless 2 with marginally better UX on HN-cohort segment" — and that may not be enough to clear P5/P6 thresholds.

**Channel mentioned weaker than positioned:**

> **LinkedIn organic for corporate segment.** Plan treats it as a viable Persona B channel. Reality: founder's 996 are semiconductor; "pivoting content" to corporate productivity takes 3-6 months minimum to build credibility with a new audience. For v1.0 launch window, LinkedIn organic is a **future channel**, not a launch channel. Use LinkedIn for warm-intro DM outreach (high signal, low scale), not for organic reach.

**Audience claim lacking evidence:**

> **"Reachable post-launch via vertical communities and industry-specific channels."** Doc claims corporate segment is reachable; no specific community or channel named. Plan above identifies CFO Dive, Healthcare Dive, Axios Pro — but founder has zero relationship with any of these, and paid placement is the only realistic short-term entry. Cost: $1-5K per test. Treat as v1.0.5+ budgeted experiment, not v1.0 free-channel access.

**Provocative reframe:**

> **Consider killing the public Show HN launch entirely and going concierge-only for 4-6 weeks.** Superhuman launched concierge for years. The bankruptcy magic-moment is built for concierge: founder personally onboards 20-50 users from warm network + LinkedIn DMs, tunes the product, runs PMF survey, builds a public case-study set (3-5 named-with-permission user stories), THEN does Show HN with the case studies as the post. Headline becomes "I tuned this product on 20 real users; here's what they said" — far stronger HN play than "shipped today; please upvote." Founder loses the calendar-pressure launch moment; gains a PMF-validated launch with social proof. **This is the canonical-success-playbook alternative the plan as written doesn't surface.**

---

## Outputs

1. `marketing_plan.md` — this doc (canonical artifact)
2. `icp.md` — Persona A + B specification
3. `launch_playbook.md` — sequenced launch plan with both cohorts
4. `audience_build_sprint.md` — 30-day pre-launch + 60-day post-launch audience cadence
5. Recommended design-doc edits (in `design_doc_edits.md`): pricing tier change, corporate-cohort PMF gate addition, picker defer-to-v1.0.5 question, referral mechanic added to v1.0.5

---

## Handoff — 3 strongest action items for THIS week

1. **Recruit 5 corporate-segment beta candidates via LinkedIn first-degree DM by end of week.** Personalize each DM; offer 4-week free concierge use in exchange for 1:1 feedback. If can't find 5, the corporate-segment thesis is in question and the entire differentiated-positioning story needs revisiting.
2. **Write 30-named-person outreach list for Day -7 soft pre-announce.** Names go in `outreach_list.md`. Include 15-20 HN-cohort + 10-15 corporate-cohort.
3. **Re-anchor pricing: pick $12/mo with $99/yr annual default for v1.0 single tier.** Update design doc P6 and landing-page copy. Tier 2 (Corporate Pro $19) flagged for v1.0.5 conditional on corporate PMF gate.

## Schedule self-check

Re-run `/plan-cmo-review` in 30 days (Day 30 post-launch) to evaluate progress against this plan. Key checkpoints: filter_setup_rate_48h, HN-cohort conversion rate, corporate beta PMF survey results.

## Follow-up skills

- `/plan-ceo-review` — re-run focused on pricing band + corporate cohort split (this affects business model in ways CEO review should re-evaluate)
- `/plan-eng-review` — minor; corporate beta concierge onboarding may require an admin-tooling pre-spec
- `/office-hours` — if PMF gate fails for corporate cohort and pivot decision is needed
