# Marketing Plan — tldrof.com (TLDR-of-TLDRs)

**Skill:** `/plan-cmo-review` v0.2.0
**Run date:** 2026-06-01
**Mode selected:** Mode C (Audience-Build Sprint) — primary; companion Mode-B-style marketing plan + launch playbook produced because founder is mid-build with hard ship date and needs both artifacts.
**Founder operating assumption:** marketing-naive default (technically strong ex-Micron engineer, first consumer product, near-zero ICP-relevant audience). Working under marketing-naive default; premise-challenge is load-bearing.

---

## PREMISE-LEVEL FINDINGS BLOCK

The v0.2 skill's load-bearing addition is the Step 0.5 Premise Audit. Run against the tldrof design doc, **four of five premise challenges failed and one is inconclusive.** This is the single highest-value output of this review.

The tldrof design doc has been through five founder editorial passes plus CEO and Eng review. Those reviews sharpened **architecture, positioning copy, and engineering risk**. None of them attacked the marketing premises, because none were CMO-shaped. Under the marketing-naive default, those premises were inherited from the founder's intuition and never tested.

### Findings summary

| # | Premise | Verdict | Severity |
|---|---|---|---|
| **M0a** | Show HN is the right launch platform for this product | **FAIL** | High |
| **M0b** | "Bankruptcy & bouncer positioning is the differentiator" sufficient without canonical-success comparable | **FAIL** | High |
| **M0c** | All v1.0 in-scope features serve the paying ICP | **FAIL** | Medium |
| **M0d** | 7-day free trial is the right acquisition mechanic for the paying ICP | **FAIL** | High |
| **M0e** | Dogfooding on technical TLDRs (AlphaSignal, etc.) tunes the product for the paying ICP | **INCONCLUSIVE leaning FAIL** | Medium-High |

**Cascading implication:** the tactical Step 0A and downstream sections (channels, pricing, launch sequence) all inherit corrections from these findings. The most consequential are:

1. The launch is currently a single-channel calendar-gated Show HN lottery ticket with no audience runway — replace with a multi-channel PMF-signal-gated rollout (M0a + M0d corrections combine).
2. Pricing band ($4.90–$9) is anchored to a near-mirror competitor (Readless); canonical-success comparables (Superhuman $30, Readwise $10–12, Substack-paid $5–50) sit higher than the planned $9. The band itself, not just the point, deserves re-examination (M0b correction).
3. The 7-day free trial selects for the wrong segment for a time-poor/money-rich corporate ICP — and corporate is the founder's strongest stated structural moat (M0d correction).
4. Dogfooding on technical-developer TLDRs may have tuned the product for a segment that is BOTH not the highest-LTV buyer AND maximally saturated with Readless awareness (M0e correction).

The rest of the marketing plan is written DOWNSTREAM of these findings. Read this block first.

---

## Step 0 — Pre-review system audit

### Existing artifacts read
- `design_document.md` (1,535 lines, APPROVED after 5 founder editorial passes + 2 adversarial spec reviews + CEO review HOLD SCOPE + Eng review)
- Marketing artifacts existing: domain registered, no landing page live, no social presence for the product, no newsletter for the product, no content history

### Founder audience audit
- LinkedIn: **~996 followers** (predominantly semiconductor / hardware professionals from ex-Micron career; low ICP overlap with consumer TLDR-overloaded knowledge workers)
- Substack: **~11 subscribers**
- Twitter/X: **0 followers** (no account presence to speak of)
- GitHub stars on prior projects: not material for consumer ICP
- Prior shipped consumer products: 0 (Micron engineer, OSS projects, makerspet store, small newsletter — none are consumer SaaS at scale)

**Verdict:** ICP-relevant audience surface area for tldrof is effectively zero. The 996 LinkedIn followers are a hardware-engineering audience — they are not the inbox-overloaded knowledge-worker / corporate-locked-out segment the product is designed for. Treat as zero for planning purposes.

### Competitive landscape web search (this run)
- Direct competitor: **Readless.app** ($4.90/mo, near-mirror architecture, content-marketing-led — their blog dominates SERPs for "best newsletter summarizers 2026", "Mailbrew alternatives", "Readwise pricing", etc.)
- Adjacent competitor: **Meco** ($0 free / $35/yr, Product Hunt launch + affiliate program with newsletter creators)
- Graveyard: **Mailbrew** ($8–10/mo, acquired by Readwise 2023, discontinued; users migrated to Readwise Reader)
- Adjacent: **Readwise Reader** (~$10–12/mo, broader read-later + newsletter + RSS, bootstrapped, partnerships-led)
- Canonical premium-concierge consumer subscription: **Superhuman** ($30/mo, concierge onboarding by Vohra personally for first 200, 450K+ waitlist, $825M acquisition Jul 2025)
- Canonical niche-indispensable consumer subscription: **Readwise** (~$10/mo, bootstrapped, paid-only after free trial, partnerships + creator collabs + API ecosystem)

### Mode selection trigger
Founder has:
- Zero ICP-relevant audience (M3 = 0)
- Direct competitor identified (Readless, with structural read)
- No canonical-success comparable named in design doc
- Hard build calendar (20–22 days, mid-build right now)

The skill's activation rule says zero-audience + zero-competitors → Mode C. Founder has a competitor identified, but the audience condition dominates. **Mode C selected.** Companion Mode-B-style marketing plan + launch playbook produced because the build is already underway and the founder needs an actionable launch sequence in addition to the audience-build sprint.

---

## Step 0.5 — Premise Audit (full)

### Premise extraction table

| # | Accepted premise | Where in doc | Hypothesis: likely-wrong because |
|---|---|---|---|
| 1 | Show HN is the launch | "Distribution Plan" + P2 HN headline | HN is dev-tools-native; the product's stronger ICPs (M365 corporate, inbox-bankruptcy non-devs) don't live on HN |
| 2 | Bankruptcy + bouncer positioning differentiates against Readless | P2, pass 4 | Differentiation copy ≠ acquisition; Readless owns SEO ("Readless vs X" pages everywhere) — positioning has to clear the discovery moat too |
| 3 | $9/mo is the right price | P5, P6, CEO PC1 | Anchored on Readless ($4.90); never tested against ICP willingness-to-pay; canonical comparables sit at $10–30 |
| 4 | 7-day free trial gates conversion via loss-aversion | P6 | Free trial mechanism selects for time-rich/money-poor; the stated corporate ICP is the opposite profile |
| 5 | Dogfooding on AlphaSignal/Bensbites/Lenny tunes the product for the paying ICP | "Target User" section | The HN-cohort technical-newsletter dogfood audience overlaps poorly with the M365/corporate-locked-out moat ICP |
| 6 | Auto-forward filter helper (Gmail only at v1.0) is enough to clear the bankruptcy-to-retention bridge | CEO PC2, P3 | Bankruptcy is one-and-done; if filter setup fails, no recurring inflow → churn inevitable; Outlook/Proton deferral leaves the corporate ICP unsupported on day 1 |
| 7 | "Structural moat" against Readless is real and durable | P4, pass 4 | CEO review L6 already softened this to "~2-week head start"; surface that softening in the marketing plan |
| 8 | 25 paying / day 30 is achievable on a single Show HN + cross-post to X (founder has no X following) launch | P5, Distribution Plan | Cross-post-to-X requires X audience; founder has none |

Premises 1, 3, 4, 5 map to M0a–M0e. Premises 2, 6, 7, 8 fold into Section 1, 3, 5 downstream.

---

### M0a — Launch-platform audience-class fit

**Question:** Is Show HN the right *audience class* for tldrof, or just the platform the founder is familiar with?

**Founder's naive answer (simulated):** *"I think so — HN is where I read about new tools, and the design doc's target user includes 'Engineers, PMs, founders, and AI-adjacent professionals who already subscribe to multiple daily TLDR-style newsletters: AlphaSignal, Bensbites, Lenny's, Pragmatic Engineer, Stratechery...' That's an HN-overlapping audience."*

**Web-search check:** Show HN base rate in 2026 — ~200 posts/day, ~24-hour upvote window, comment volume does not predict signups, and Show HN volume has tripled since 2019. Daniel King's 2026 data (14 years, 188,000 posts) shows the median Show HN gets <5 upvotes; the long tail is what makes it look like a viable channel via survivor bias.

For NEWSLETTER-AGGREGATOR specifically, recent Show HNs (search results above) show no clear winners in 2025–2026. Meco grew via Product Hunt + creator affiliate, not HN. Readless grew via SEO (blog content), not HN. **There is no canonical Show HN newsletter-aggregator success to point to.**

For the **product's strongest stated ICP** — M365 / corporate-locked-out users (lawyers, finance, healthcare, government) — HN audience overlap is near zero. HN is dev-and-startup-heavy; corporate lawyers are not the HN audience.

**Verdict: PREMISE FAILS.**

Show HN is the right platform for the *founder-dogfood-audience class* (HN-reading engineers who already subscribe to AlphaSignal). It is the wrong platform for the *positioned-moat audience class* (M365/corporate, time-poor/money-rich, regulated industries). The founder optimized launch platform for the audience they share an identity with, not for the audience the design doc claims as the strongest structural moat.

**Cascading implications:**
- M2 (discovery path) cannot have "Show HN" as step 1 for the corporate ICP — it doesn't reach them
- The actual ICP-platform map needs splitting: HN-cohort for the technical-bankruptcy segment, *other* channels (LinkedIn long-form, vertical-industry communities, paid placements in industry newsletters) for the corporate segment
- Section 5 launch playbook must NOT be Show-HN-first. Show HN can be ONE channel of three (per skill anti-pattern #2), but it is not the lead channel for the highest-LTV ICP

---

### M0b — Canonical-success comparable

**Question:** Name the most successful product in this category at this motion class. What did they do that the current plan does NOT?

**Founder's naive answer (simulated):** *"Readless is the closest comp at $4.90/mo, and Mailbrew was the previous one before they got acquired. I guess Substack and Beehiiv at the publication-side, but they're not really comparable. There's no real direct success at $9/mo for the digest-of-digests motion specifically."*

**Web-search verdict (mandatory — skill refuses "no real comparable"):** the founder is right that there's no direct-competitor canonical success at exactly this motion. That is the WRONG question. The right question is **canonical-success comparable for the motion CLASS** — *premium-concierge consumer subscription* and *niche-indispensable consumer subscription*. Both have named, documented, well-known successes.

| Canonical success | Price | Motion class | Primary acquisition | Onboarding | Launch gate |
|---|---|---|---|---|---|
| **Superhuman** | $30/mo | Premium-concierge consumer SaaS | Waitlist (450K) + referrals + concierge | Vohra personally onboarded first 200; 14-person concierge team at scale | PMF-signal (Vohra "very disappointed" test ≥40%) — NOT calendar |
| **Readwise** | ~$10/mo | Niche-indispensable consumer SaaS | Bootstrapped product-led + partnerships + creator collabs + dev API ecosystem | Self-serve + freemium-to-paid (later paid-only after free trial) | Product-led; no big-bang launch |
| **Substack (subscriber-side)** | varies, $5–50/mo per publication | Niche-indispensable consumer subscription | Creator-led; existing audience of writer is the entire funnel | Writer-owned onboarding | Continuous |
| **The Browser (newsletter)** | $5/mo | Curation-as-product consumer subscription | Editor's personal network + word-of-mouth + slow Twitter compounding | Trial-free model | Slow burn, no big-bang |

**Specific deltas between canonical successes and tldrof's current plan:**

1. **Superhuman delta:** Superhuman's launch gate was PMF-signal (Vohra Score ≥40% "very disappointed"). tldrof's gate is **calendar (day 18 → 20–22)**. For a retention-driven $9/mo consumer subscription, calendar gating is the wrong choice (skill anti-pattern #8).
2. **Superhuman delta:** Superhuman manually onboarded 200 users before scaling. tldrof plans to ship straight to public Show HN. The "5 HN-cohort friends as private-beta users" in CEO PC3 is the right INSTINCT but the wrong SCALE — should be 20–50 manually-onboarded users before any public launch, not 5.
3. **Readwise delta:** Readwise was bootstrapped via partnerships + creators + API ecosystem. tldrof has none of these channels in v1.0 launch plan. The Strategic Ladder Rung 2 (Suite) hints at API/blueprint extensibility, but launch sequence ignores it.
4. **The Browser delta:** Editorial-curated-newsletter products win by having a known curator. tldrof's curator (the founder) has 11 Substack subscribers. The curator-led path is not available without 6–12 months of audience-building first.

**Verdict: PREMISE FAILS.**

The plan anchors against Readless (direct competitor, possibly losing — content marketing has not hit escape velocity per traffic signals) and ignores the canonical successes whose playbooks would actually transfer. **The single biggest plan-shape correction:** copy the Superhuman concierge-onboarding pattern at smaller scale for the first 20–50 users; gate the public launch on a Vohra-style PMF signal, not a calendar day.

---

### M0c — Anti-feature surface

**Question:** Name 2+ in-scope features that contradict positioning, trust model, or business model.

**Founder's naive answer (simulated):** *"Honestly I don't think any of the v1.0 features contradict positioning. We trimmed pretty aggressively in CEO review — killed feature flags, deferred Playwright automation, etc. The picker is small but it's a fallback."*

**Line-by-line check of v1.0 in-scope features:**

| # | Feature | Stated positioning it could contradict | Verdict |
|---|---|---|---|
| 1 | **Secondary curated picker (~30 newsletters)** | "Forward-from-inbox bankruptcy" is the primary frame; picker serves users with EMPTY inboxes — opposite segment from inbox-bankrupt | **ANTI-FEATURE candidate.** Picker users are time-rich starting-fresh users; bankruptcy users are time-poor backlog-clearers. Two products, one app. |
| 2 | **7-day free trial, no CC required at signup** (CEO review allows trial with Stripe Checkout post-trial) | Positioning targets corporate/M365 segment as moat; corporate buyers are TRUST-LED, not TRIAL-LED | **ANTI-FEATURE.** See M0d full treatment. |
| 3 | **Read-only digest API + MCP wrapper** (v1.1, but design doc surfaces it as "for power users / OpenClaw / personal-agent integration") | Positioning is "zero-effort consumer SaaS for the inbox-overwhelmed"; API + MCP serves the technical-DIY segment that builds its own digests with Cron + Claude API | Soft anti-feature. Power-user-API audience is the LOWEST-LTV segment for a $9/mo subscription — they have the alternative of building it themselves. |
| 4 | **5-option delivery dropdown (6am, 8am, 12pm, 5pm, 8pm) + auto-detected mode** | Positioning is "we figured it out for you, zero questions asked" | Mild contradiction — the dropdown undermines the "auto-detected" magic. Most users will never touch it; keeping it is fine, but if it ships visibly it dilutes the positioning. Default the UI to "Auto" and hide the override behind one click. |
| 5 | **Per-newsletter / per-item summarization slider (v1.1)** | Positioning is "set and forget"; sliders are power-user UX | This is flagged in the design doc as "strongest moat candidate" but it serves a different segment (engaged tweakers) than the bankruptcy framing serves (set-and-forget). Worth keeping as a Rung 2 wedge, NOT as a v1.0/v1.1 positioning anchor. |
| 6 | **Strategic Ladder Rung 2 → Rung 4 ambition** baked into landing-page copy / pitch | v1 positioning is "consumer SaaS for inbox overload"; the platform/concierge/spawn-a-business rungs are b2b/operator-shaped | Not a v1.0 product feature, but DO NOT mention rungs 2–4 in v1 marketing copy. The Strategic Ladder is fundraising/internal-strategy framing; users want to know what the product does TODAY. |

**Verdict: PREMISE FAILS — 2 clear anti-features (picker, free trial), 2 soft ones (API/MCP, delivery dropdown), 1 future drift risk (slider in v1.1), 1 marketing-discipline note (don't talk Rungs 2–4 in v1 copy).**

**Recommended decisions:**
- **Picker:** kill from v1.0 (already a "stretch goal per CEO review packing"); ship to v1.0.5 ONLY if launch data shows >15% of signups have empty-inbox onboarding. The bankruptcy framing IS the positioning; protect it.
- **Free trial:** see M0d. Strongly consider concierge-first cohort instead.
- **API/MCP:** keep in v1.1 backlog but de-emphasize in launch messaging.
- **Delivery dropdown:** hide behind one extra click; default UI is just "Auto-detected."
- **v1.1 slider:** valid but communicate it as advanced feature for retained users, not as launch positioning.
- **Strategic Ladder:** keep internal; v1 marketing copy is the bankruptcy/bouncer story only.

---

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the 7-day free trial select for the wrong segment?

**Founder's naive answer (simulated):** *"The 7-day free trial is load-bearing — by trial end the user has reallocated the saved 45 minutes, so canceling means giving the time back. That's the loss-aversion gate from P6. Industry standard for $9/mo SaaS is 7-day trial. Stripe Checkout post-trial means cards on file before charge."*

**Diagnostic — map the acquisition mechanic to attracted segment:**

| Mechanic | Attracted segment |
|---|---|
| 7-day free trial, no CC at signup | Time-rich, low-commitment — trial-shoppers who churn on cancel-by-trial-end |
| 7-day free trial, **CC required** at signup | Higher-intent than no-CC, but still trial-shoppers |
| **Concierge onboarding waitlist** | Committed prospects willing to wait — serious intent signal |
| **Referral from trusted source (HN-cohort friend, industry comp)** | Trust-led, often time-poor/money-rich (the design doc's stated moat ICP!) |
| **Paid placement in industry-vertical newsletter** | Audience of that publication — directly the time-poor professional segment |
| **Free tier (Meco's path)** | Mass-volume top-of-funnel; commodity perception |

**The doc's stated highest-leverage ICP** (per P4 + Founder Editorial Pass 1 expanding the secondary segment): "M365 / Outlook users (~400M globally) and corporate-email users locked out of OAuth-based AI inbox tools by security policy: lawyers, finance, healthcare, government, agency operators with custom-domain email."

**This is a time-poor / money-rich / trust-led segment.** A managing partner at a law firm does not trial-shop $9/mo productivity tools. They either:
1. Get recommended the tool by a peer they trust → signs up because of social proof
2. See it in an industry trade publication / community → signs up because trusted publication endorsed
3. Get pitched by their IT department or assistant → signs up because someone they delegate to handled it

**Free trial with no CC sends the WRONG signals to this segment:**
- Signals "we're early / unproven / commodity"
- Forces them to remember to cancel (low-priority task for high-throughput professionals)
- Selects FOR engineers/founders who DO trial-shop (time-rich segment, low LTV)
- Selects AGAINST the corporate moat ICP

**Industry-standard counter-argument** (the founder might raise): "Stripe Checkout post-trial is standard for $9/mo SaaS, Superhuman / Readwise / Notion all do trial-then-pay." That's true for the **consumer-prosumer segment**. It's NOT how Superhuman ran its early growth — Superhuman had no public free trial for the first ~3 years; they had a waitlist + concierge onboarding + invite-only model precisely because they were targeting a trust-led segment.

**Verdict: PREMISE FAILS.**

7-day free trial is right for the HN-cohort technical buyer. It is wrong for the corporate moat ICP. Two options:

**Option A (recommended, structural):** Run TWO acquisition paths for two ICPs:
- HN-cohort segment: 7-day free trial as designed, Show HN as one of several launch channels, $9/mo
- Corporate/M365 segment: concierge waitlist, manual founder onboarding for first 20–50 users, $19–29/mo (premium positioning consistent with the segment's WTP), invite-only beta

**Option B (simpler, cheaper):** Drop the corporate moat framing entirely from v1 marketing, ship only the HN-cohort path, and revisit corporate as v1.0.5 once you have HN-cohort traction. **This is the more honest answer for a solo-founder, 20-22 day v1.0 build.** Cycle time on corporate-segment customer-development would consume a quarter on its own.

**Recommended decision:** Option B for v1.0 launch. Drop M365/corporate moat marketing claims from v1.0 launch copy. Capture them as v1.0.5 motion. Specifically:
- Remove "Works with Gmail, Outlook, Proton, anything" from primary landing copy; keep technically true but de-emphasize
- Drop the "400M+ M365 / corporate-locked-out users" claim from any pitch deck
- Ship v1.0 to the HN-cohort segment with 7-day trial, then validate the corporate path separately as v1.0.5 with a concierge-waitlist treatment

If the founder wants to pursue both segments simultaneously (Option A), this becomes a 2-month launch program, not a 20-22 day build → ship. **Be honest about which trade.**

---

### M0e — Dogfood audience-class match (founder vs paying ICP)

**Question:** Is the dogfood audience the same as the paying ICP?

**Founder's naive answer (simulated):** *"I'm the ICP. I subscribe to AlphaSignal, TLDR Tech, Bensbites, Lenny's, Pragmatic Engineer — those are the same newsletters the HN-cohort reads. Dogfooding on these tunes the product for the launch audience."*

**Analysis:** The founder is correctly identifying that they are A user. The question is whether they are the BUYING user.

Two issues:

**1. Dogfood-audience-newsletter-MIX is technical-developer-heavy.** AlphaSignal, TLDR Tech, Bensbites, Pragmatic Engineer, Latent Space — these are AI/dev newsletters where dedup is HIGH (every major AI release gets covered everywhere). The product will appear to work very well on this mix because the dedup pass has lots of obvious duplicates to merge. But for the **corporate moat ICP** — lawyers reading Law360 + ABA Journal + Bloomberg Law, finance pros reading Axios Pro Rata + Term Sheet + The Information — the newsletter mix has LOW cross-source overlap (legal/finance verticals don't cover the same stories the same way). The product's flagship "you saved N minutes from deduplication" math will look different (worse) on those mixes than it does on the founder's dogfood mix.

**2. The HN-cohort dogfood audience is precisely the segment most likely to ALREADY KNOW Readless.app** ($4.90/mo, same architecture, exists for 1+ year, content marketing engine running hot — their blog occupies multiple SERP positions for "newsletter summarizer" queries). The founder's "the launch IS the test" plan assumes a cold HN audience; in reality, a meaningful share of HN-cohort technical readers will Google "tldrof vs readless" within 5 minutes of seeing the Show HN post.

**Verdict: PREMISE INCONCLUSIVE LEANING FAIL.**

The dogfood-audience-match is correct in the narrow sense (founder is in the HN-cohort segment). But:
- The dogfood newsletter MIX is biased toward high-dedup verticals; product may underperform on low-dedup verticals (which is where the corporate moat segment lives)
- The dogfood audience is the segment most exposed to Readless competition, making the "first impression in 60 seconds" claim harder to make stick

**Recommended action:**
- During days 7–9 of remaining build, add 3–5 dogfood subjects whose newsletter MIX is NOT AI/dev (e.g., one professional reading Axios + Punchbowl + The Information; one in healthcare reading STAT + Endpoints + Fierce Healthcare). Verify dedup quality on those mixes BEFORE shipping. This is the cheapest premise-correction available.
- If dedup quality on low-overlap verticals is meaningfully worse, surface this honestly in onboarding ("works best for users with 5+ newsletters in the same vertical") rather than overclaiming.

---

### Pricing-band sub-check (M0b-adjacent, also feeds Section 6)

The design doc treats $9/mo as locked from Premise P5/P6 with no ICP-WTP evidence cited. CEO PC1 confirmed "Hold $9/mo" but did so based on competitive positioning rationale (don't race to Readless's $4.90 floor), not ICP-WTP evidence.

**Pricing band evidence from web search:**
- Readless: $4.90/mo (the floor; widely cited)
- Meco: $34.99/yr ($2.92/mo equivalent — free tier dominant)
- Mailbrew (historical): $8–10/mo (acquired & discontinued — not a survival proof)
- Readwise: ~$10/mo (paid-only after free trial)
- Readwise Reader: $10–12/mo bundled
- Superhuman: $30/mo
- Substack-paid: typically $5–50/mo PER publication (subscribers stack multiple)
- ChatGPT Plus: $20/mo (the consumer-AI anchor)
- News-subscriptions benchmark: average monthly churn 5.3%; >25% first-term churn is "normal"

**Implication:** the $9/mo point is **the middle of a band that goes from $5 to $30**. The CEO review locked $9 against Readless's $4.90 — that's a defense against the floor, not an investigation of the ceiling. For the HN-cohort segment $9 is fine. For the corporate segment (if pursued — see M0d) $19–29 is the more honest positioning. Section 6 expands.

---

### Step 0.5 completion summary

**4 of 5 premise challenges failed; 1 inconclusive-leaning-fail. 8 of 8 extracted marketing premises are downstream-affected.** Under the v0.2 skill's default refusal posture, this is exactly the situation where premise-challenge is load-bearing.

Cascading into Step 0A:
- **M1** answers cannot accept the HN-cohort persona as the only ICP; need to either pick one ICP and ship clean, or run a two-track plan honestly
- **M2** answers cannot have Show HN as step 1
- **M3** answer is brutal: founder has effectively zero ICP-relevant audience; this triggers Mode C
- **M4** answer needs to be honest: founder has no channel advantage yet; that becomes the first work item
- **M5** competitor-traffic answer must include Readless's SEO content engine, not just "competitor exists"
- **M6** first-10 plan must be a concierge-onboarding plan, not a launch-flood plan
- **M7** time allocation must shift HEAVILY toward audience-build in the remaining build window AND post-launch

---

## Step 0A — Forcing questions (Step 0.5 findings woven in)

### M1 — Audience reality

**Question:** Name a specific person who would actively seek out tldrof. Where do they hang out NOW?

**Founder's answer (simulated, naive):** *"Jake — engineer at a mid-size SaaS company, mid-30s, subscribes to AlphaSignal, TLDR Tech, Lenny's Newsletter, Pragmatic Engineer, and Bensbites. He reads HN every morning, follows Lenny Rachitsky and Pieter Levels on Twitter, has a Notion full of half-read newsletter clippings, has tried Mailbrew years ago and let it lapse, currently uses ChatGPT manually to summarize the long ones. Reachable via HN."*

**Skill challenge:** Jake is a fine persona — but he is the EASIEST persona to acquire and the WORST-LTV. He is technically capable (could build a Python script), price-sensitive (already paying for ChatGPT Plus, Cursor, Linear, etc. and feels saaS-fatigued), and dogfood-saturated (every other founder ships a productivity tool to Jake).

**Refined accepted answer (the founder, post-pushback):**
- **Primary v1.0 ICP — "Jake the saturated technical reader":** as above. Cheap to reach, low-LTV, moderate retention. Use to validate product mechanics, not as the long-term wedge.
- **Latent v1.0.5+ ICP — "Maya the corporate professional":** managing partner at a law firm or finance director, mid-40s, subscribes to industry verticals (Law360, ABA Journal, Bloomberg Law / Axios Pro Rata, Term Sheet, The Information), reads them on an M365 corporate account, can't use Shortwave/Notion Mail because IT policy forbids OAuth, has an assistant who handles inbox. Reachable via vertical-industry newsletters, LinkedIn long-form, paid placements, referrals from peers.
- **Specific places Jake currently spends attention:** HN front page (daily), Substack apps for Lenny's, Twitter/X feed (Pieter Levels, Lenny, Sahil Bloom, founders), r/sideproject (lurker), Indie Hackers (light)
- **Specific places Maya currently spends attention:** her industry-specific Slack/community (e.g., Bar Association Slack, ProductFinance Slack), LinkedIn (heavy), Bloomberg Terminal / Bloomberg Law portal, the trade journals in her vertical, conference circuit (annual). Almost zero overlap with HN/Twitter.

**v1.0 decision (per M0d Option B):** Ship to Jake. Defer Maya to v1.0.5 with a concierge-waitlist treatment.

### M2 — Discovery path

**Question:** Walk through the specific path by which Jake discovers tldrof. Minimum 3 steps. Step 1 is NOT Show HN.

**Founder's answer (simulated, naive):** *"Jake sees my Show HN post in the morning, clicks through, signs up, completes the forward-from-inbox bankruptcy flow, gets the 60-second magic moment."*

**Skill challenge: Show HN as step 1 = refused per skill rule.** Force a real multi-step funnel.

**Refined accepted answer:**

For Jake, plausible 3-step discovery paths (multiple, because no single channel suffices):

**Path A — Build-in-public Twitter:**
1. (Days -30 to -7 pre-launch) Founder posts daily on X about the build: "Day 3 — Mailgun inbound pipeline working, here's the latency math." 5-10 followers initially, grows via replies to Pieter Levels / Lenny / Marc Lou.
2. Jake follows a few of those accounts; sees a reply from `@iliyaov` (or whichever handle the founder picks) about a "TLDR-of-TLDRs" project; clicks through to landing page.
3. Lands on a waitlist page (pre-launch) or signup page (post-launch); subscribes.

**Path B — Show HN (one of multiple channels):**
1. Founder posts Show HN at calculated time (Tuesday 7am PT, per HN-launch literature).
2. Jake sees it during morning HN reading; the title "50 unread newsletters? Forward them all here. Get one digest in 60 seconds. Inbox debt cleared." hooks because Jake has 50 unread newsletters.
3. Clicks through, lands on landing page, signs up.

**Path C — Indie Hackers / r/SideProject cross-post:**
1. Founder cross-posts launch story to Indie Hackers ("How I built TLDR-of-TLDRs in 20 days as a solo founder") and r/SideProject (per community rules, days 1-2 after HN to avoid duplicate-content penalty).
2. Jake lurks in Indie Hackers; sees post.
3. Clicks through; signs up.

**Path D — Newsletter-creator placement (medium-term):**
1. Founder pitches Lenny / Pragmatic Engineer / TLDR Tech for a sponsored placement or a guest column ("How I built TLDR-of-TLDRs"). Pays ~$2-5K for a sponsored placement or ~free for guest column.
2. Jake reads his usual Pragmatic Engineer issue; sees tldrof mentioned.
3. Clicks through; signs up.

Path A is the cheapest and starts NOW (pre-launch). Path B is the one-shot launch event. Path C is the immediate follow-up. Path D is the v1.0.5 channel after some traction.

### M3 — Pre-launch audience

**Question:** Show evidence of existing audience. Specific numbers.

**Founder's honest answer:** *"LinkedIn ~996 followers (semiconductor/hardware industry, wrong ICP). Substack ~11 subscribers. Twitter/X 0 (no account presence to speak of). Domain registered recently. No prior shipped consumer products."*

**Accepted answer (with honest acknowledgment):** Effectively zero ICP-relevant audience. **Triggers Mode C (Audience-Build Sprint).** This is THE load-bearing constraint of the entire marketing plan.

### M4 — Channel honesty

**Question:** Name ONE distribution channel where the founder has a credible, demonstrable advantage.

**Founder's honest answer:** *"I don't have one yet. Closest thing is maybe LinkedIn since I have 996 followers there, but they're hardware engineers, not the right ICP. I write technically well but have no published track record."*

**Accepted answer:** "I don't have one yet" — becomes the **first work item, not a future-tense aspiration.** Choose ONE channel where the founder COMMITS to building advantage over the next 60 days. Recommended: **Twitter/X build-in-public** because (a) Pieter Levels-pattern proven, (b) reaches Jake-ICP, (c) compounds, (d) low capital cost. See Mode C audience-build sprint for cadence.

### M5 — Competitor traffic source

**Question:** Where does Readless actually get its users?

**Founder's naive answer:** *"I don't know. Their landing page is fine; they're on Twitter but it doesn't look highly active. I assumed word-of-mouth or PH launch."*

**Web-search evidence (this run):**
- **Readless's primary acquisition channel = SEO via heavy content marketing.** Their blog posts dominate SERPs for: "best newsletter summarizers 2026", "Mailbrew alternatives", "Readwise vs Feedly", "best AI newsletters 2026", "TLDR Newsletter review 2026", "Meco pricing 2026", "Matter App pricing 2026", "The Information price per month 2026", and many more. This is a systematic SEO content engine targeting comparison and pricing queries.
- This is exactly the playbook Ahrefs used (founder mentioned in earlier brainstorming): produce 1 high-quality comparison-or-pricing article per week, rank in SERPs over 6–12 months, capture intent traffic.
- Implication: Readless has likely been building this for 6–12+ months before tldrof launches. **tldrof cannot win Readless's SEO turf in the launch window — that's a 12-month minimum project.** tldrof's launch must come through channels Readless is NOT dominant in.
- Channels Readless does NOT appear to dominate: HN (no significant Show HN footprint visible), Twitter/X build-in-public, Indie Hackers community presence, vertical-industry placements, ProductHunt (Meco has stronger PH presence).

### M6 — First 10 paying customers

**Question:** Name the specific path to your first 10 paying customers.

**Founder's naive answer:** *"15 paying conversions within first 14 days post-launch per P6 — most through Show HN traffic, plus 5 HN-cohort friends as private-beta users from CEO PC3."*

**Skill challenge (per M0b / Superhuman precedent):** "15 conversions in 14 days via Show HN" is the lottery-ticket plan. Real first-10 plan needs NAMED people.

**Refined accepted answer (concierge-first, the recommended plan):**

The first 10 paying customers should be MANUALLY ONBOARDED by the founder, Superhuman-pattern. Specifically:
1. **5 HN-cohort friends** (per CEO PC3) — the founder identifies these by name now: friend who reads AlphaSignal, friend in YC, friend at SaaS startup, friend who shipped previous side projects, friend who is current Mailbrew refugee. Each gets a personalized email + a 30-min video onboarding.
2. **5 newsletter authors / creators** the founder admires and reads — pitch them tldrof in exchange for their feedback. Lenny Rachitsky is over-pitched but worth one attempt; the Pragmatic Engineer's author; TLDR Newsletter team; the Bensbites curator; a few Substack writers in the founder's adjacent space. Each gets a personalized email offering free annual access in exchange for product feedback + (if they like it) one social post.
3. **5 audience-build sprint contacts** — people the founder meets via the Mode C audience-build sprint over the next 30 days (build-in-public Twitter replies, r/SideProject genuine engagement, Indie Hackers comments). Convert 5 to paying over 30 days.

That gets the founder to 15 paying via NAMED humans, not lottery tickets. Names go in a spreadsheet; outreach happens by hand. This is the Superhuman / Readwise / The Browser playbook applied at solo-founder scale.

### M7 — Time allocation

**Question:** What % of pre-launch time on audience-building vs building?

**Founder's honest answer:** *"I'm Day 5 of a 20-22 day build. Remaining ~15 days. Audience-build is currently 0% — heads-down on Mailgun MX, Claude pipeline, Stripe Checkout. Maybe 5% if I count the time I'll spend writing the Show HN post."*

**Skill challenge (per skill rule):** <30% on audience pre-launch is acknowledged risk. Given the audience-from-zero starting point, this is the **single biggest cause of the v0.1 of this skill's "ship to silence" prediction.**

**Refined accepted answer:**
- Days 6–22 of build: shift to **20% time on audience-build minimum** even at the cost of build velocity. Cut features (de-prioritize the picker entirely — already a stretch goal per CEO PC1; if it slips it's fine).
- Specific audience-build activities in remaining build window:
  - Days 6–8: set up Twitter/X account; first 3 build-in-public posts; reply to 5 accounts/day in target ICP
  - Days 9–14: write 1 long-form post on "What I learned building TLDR-of-TLDRs in 20 days"; post to LinkedIn + Twitter + (after launch) HN; start outreach to 5 HN-cohort friends to be private-beta users
  - Days 15–22: prep launch sequence; finalize 10-person concierge waitlist; pre-write 5 cross-channel launch posts
- Post-launch days 1–60: **50%+ time on audience + outreach**, not on product polish. The product is "good enough"; the audience is not.

---

## Step 0B — Mode confirmation

**Mode C (Audience-Build Sprint) is the primary deliverable.** See `audience_build_sprint.md`.

**Companion deliverables produced (per task brief):**
- `marketing_plan.md` (this file — Mode-B-style focused review)
- `launch_playbook.md` (per Section 5)
- `icp.md` (per Section 2)
- `audience_build_journal.md` (cadence-tracking template)

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | URL | Founded | Pricing | Primary acquisition (verified) | Public user complaints | Positioning vs tldrof | Honest assessment |
|---|---|---|---|---|---|---|---|
| **Readless** | readless.app | ~2024–2025 (1 yr) | $4.90/mo Pro, free Lite | **SEO content engine** (multiple SERP-dominating blog posts on comparisons/pricing/best-of lists) | "No instant magic moment, first digest in 24h" (founder's own competitive intel); "subscribe-forward UX, hard to use with locked accounts" | Direct overlap on architecture; Readless leads on price/SEO; tldrof differentiates on bankruptcy framing + 60s magic moment + auto-forward helper | **Probably winning the SEO game but unclear on actual MRR.** Signup glitch reported by founder suggests low traffic. Pricing race-to-the-bottom limits LTV. Solo founder = capability parity. |
| **Meco** | meco.app | 2021 | Free / $34.99/yr Pro | **Product Hunt + newsletter-creator affiliate program** | Limited free tier; AI summaries paid-only | App-shaped (mobile-first reader), not digest-shaped; different motion | Likely winning on volume (free tier + 4.77 Google Play rating, 660+ reviews). LTV unclear; ARPU likely low. |
| **Readwise Reader** | readwise.io/reader | 2022 (Reader); Readwise 2017 | ~$10–12/mo bundled | **Partnerships + creator collabs + dev API + organic from Readwise base** | Heavy app surface; not digest-first | Adjacent — Reader is a read-later/RSS/newsletter app, not a digest-of-digests | Strongest financial position (Readwise has 4M+ registered, 3M+ MAU, 8%+ monthly growth). Not the same product; competes for share of attention. |
| **Mailbrew (legacy)** | mailbrew.com | 2020, acquired by Readwise 2023, discontinued | Was $8-10/mo, now free skeleton | Was Product Hunt + word-of-mouth | "Discontinued" / "migrate to Readwise Reader" | Historical comp — proves the motion can fail to scale and get acqui-hired-into-discontinued | **Cautionary tale.** Solo team built a beloved product, couldn't scale solo, got swept into a larger reader. Same risk shape for tldrof. |

### 1b. Canonical-success comparables (the part the design doc skipped)

| Canonical | Motion class | Price | Primary acquisition | Onboarding | Launch gate | What they did that tldrof's plan does NOT |
|---|---|---|---|---|---|---|
| **Superhuman** | Premium-concierge consumer SaaS | $30/mo (now $30; launch was higher) | Waitlist (450K peak) + concierge + referrals | Vohra personally onboarded first 200; 14-person concierge team at scale | **PMF-signal (Vohra ≥40% "very disappointed")** — not calendar | (1) Manual onboarding before any public launch (2) PMF-signal launch gate (3) Premium pricing for premium positioning (4) Waitlist to control growth rate |
| **Readwise** | Niche-indispensable consumer SaaS | ~$10/mo | Bootstrapped product-led + partnerships + creator collabs + dev API ecosystem | Self-serve, freemium→paid (later paid-only after free trial) | Product-led continuous; no big-bang | (1) Partnership channel built from day 1 (2) Creator collaborations as primary growth (3) API/dev ecosystem to compound (4) No reliance on launch events |
| **The Browser** | Curation-as-product consumer subscription | $5–10/mo | Editor's personal network + word-of-mouth + slow compounding | Trial-free or low-trial | Continuous | (1) Editor-as-brand (named curator with reputation) (2) Slow-grow, never relied on big launches |
| **Substack-paid (subscriber side)** | Niche-indispensable per-publication subscription | $5–50/mo each | Creator's existing audience IS the funnel | Creator-owned | Continuous | Audience-precedes-product, always |

### 1c. Pattern surface

**What the canonical successes have in common that tldrof's plan lacks:**

1. **Audience-precedes-product, always.** Superhuman = Vohra's network + waitlist; Readwise = founder's content + partnerships; Substack-paid = creator's pre-existing audience; The Browser = editor's reputation. tldrof has no pre-existing ICP-relevant audience. **This is the single biggest delta.**

2. **PMF-signal launch gate, not calendar gate.** Superhuman's Vohra Score was the gate. Readwise didn't have a "launch" — they ramped continuously. tldrof has a calendar gate (day 20–22). **Skill anti-pattern #8 fires here.**

3. **Manual concierge for first N users.** Vohra personally onboarded first 200. tldrof plans to ship to public Show HN with 5 friends as private beta. **The 5 is the right instinct (CEO PC3); 200 is the right scale model. Aim for 20–50 manual onboards before public launch.**

4. **Compounding acquisition channel built in, not bolted on.** Readwise has partnerships + dev API; Substack has creator-network effects. tldrof has nothing compounding in v1.0 — every signup is a one-shot acquisition that costs the same as the next. **Even adding ONE compounding channel (e.g., a referral mechanic in-product, or a public "your time saved this week" share image) buys leverage.**

**Where direct competitors diverge from canonical-success patterns:**
- Readless = SEO content engine. Compounding channel (SEO posts rank for years). But pricing race-to-the-bottom commits to commodity LTV. Halfway-canonical.
- Meco = Product Hunt + creator affiliate. Compounding via creators. But free-tier dominant commits to ad-or-volume LTV strategy. Different game.
- Mailbrew = couldn't sustain solo, got absorbed. Negative-example.

**Which pattern is the current plan implicitly following:** **None cleanly.** Current plan is "Show HN + cross-post to X (without X audience) + bankruptcy framing." That's the indie-hacker default pattern, which has ~5% success rate per Daniel King's 2026 HN data and Pieter Levels' explicit warnings (no audience = no launch).

**Recommendation:** explicitly adopt a **Superhuman-scaled-down + Readwise-compounding** hybrid:
- Manual onboard first 20–50 users (Superhuman model) before public launch
- Add ONE compounding channel from day 1 (build-in-public Twitter cadence — Levels model — OR partnerships with 2–3 newsletter creators — Readwise model)
- Gate public launch on PMF-signal (e.g., "70% of manually-onboarded users use product 3+ days/week for 3 weeks") not calendar
- Show HN becomes ONE channel of a multi-channel sequence, not the launch

**Founder homework:** read Vohra's Lenny's Newsletter interview ("Superhuman's secret to success") + Readwise's "Why we're bootstrapping Readwise" blog post. Both are linked in Sources below. ~2 hours of reading. Single highest-leverage homework in this whole plan.

---

## Section 2 — ICP specification

See `icp.md` for the full ICP doc. Summary here:

**v1.0 primary ICP — "Jake the saturated technical reader":**
- Engineer / founder / PM at SaaS or AI-adjacent company; mid-30s; US-based
- Subscribes to 5–15 daily/weekly newsletters in tech/AI/startup verticals
- HN reader, Twitter follower of Pieter Levels and Lenny, Substack reader, Indie Hackers lurker
- Pays for: ChatGPT Plus ($20), Cursor ($20–40), Linear ($8), Notion ($10), Substack subscriptions ($5–10 each)
- Complaints in adjacent categories: "ChatGPT Plus rate-limits me when I bulk-paste 20 newsletters", "Mailbrew shut down", "Readwise Reader is great but I want a daily summary not a reader"
- Objections to tldrof: "$9/mo is a lot when ChatGPT can do this manually", "I tried Readless and it was OK", "How is this different from Mailbrew?", "I don't want to set up forwarding rules"
- Reasons to convert: "60-second magic moment lands on first visit", "auto-forward setup is one click for Gmail", "the time-saved math is funny/shareable"

**v1.0.5+ deferred ICP — "Maya the corporate professional":**
- Managing partner at a law firm or finance director or healthcare exec; mid-40s; US-based; corporate M365 / Outlook
- Subscribes to 3–8 vertical industry newsletters
- Cannot use OAuth-based AI inbox tools per IT policy
- LinkedIn-heavy, vertical-Slack-heavy, almost no HN/Twitter
- Pays for: Bloomberg Terminal ($24K/yr), industry conferences, professional memberships
- Reachable via: vertical newsletter placements, LinkedIn long-form, peer referrals
- **Defer to v1.0.5** (per M0d Option B). Don't pursue in v1.0.

---

## Section 3 — Distribution channel-by-channel

| Channel | Reach (1-5) | Cost (1-5; 5=cheap) | Conversion (1-5) | Founder fit (1-5) | Effort to start (1-5; 5=easy) | Leverage score (R×Conv×Fit ÷ Cost⁻¹ ÷ Effort⁻¹) | Verdict |
|---|---|---|---|---|---|---|---|
| Show HN | 4 | 5 | 2 | 3 | 5 | Medium | KEEP — one channel of multi-channel launch; not primary |
| Twitter/X build-in-public | 3 (compounding) | 5 | 3 | 2 (no current following) | 4 | High after ramp | KEEP — primary audience-build channel; commit 60+ days |
| Substack content cadence | 2 (compounding) | 5 | 4 | 3 (has 11 subs) | 4 | Medium-High after ramp | KEEP — content compounds, ICP overlap good, leverages 11 existing subs |
| LinkedIn organic (long-form) | 3 (compounding) | 5 | 3 | 3 (996 hardware followers — wrong ICP but base) | 4 | Medium | CONDITIONAL KEEP — post long-form about the build journey; hardware engineers may bring 1–2 customer referrals but main use is ICP-shift over time |
| LinkedIn paid | 3 | 1 | 3 | 2 | 3 | Low | CUT for v1.0 — premature |
| Indie Hackers | 2 | 5 | 4 | 4 | 5 | Medium | KEEP — tight community fit, low effort, day-2 launch cross-post |
| Reddit r/SideProject | 3 | 5 | 3 | 4 | 4 | Medium | KEEP — day-2 launch cross-post, follow community rules carefully |
| Reddit other (r/productivity, r/getmotivated) | 2 | 5 | 2 | 2 | 2 | Low | CUT — community rules harsher, ban risk high |
| Product Hunt | 4 | 5 | 3 | 3 | 4 | Medium-High | KEEP — separate launch event day +7 (different audience overlap with HN) |
| SEO content | 1 (12-mo ramp) | 5 | 5 | 3 | 2 | Low at launch, high in 12 months | DEFER to v1.0.5+ — Readless already dominates the SERPs; entering this fight pre-launch is wrong |
| Newsletter-creator placements (sponsored / guest) | 4 | 2-3 | 5 | 2 | 3 | Medium-High | DEFER to v1.0.5 — pursue after launch with traction proof |
| Podcast guesting | 3 | 5 | 4 | 2 (no track record yet) | 2 | Medium | DEFER — pursue at v1.0.5 once founder has launch story to tell |
| Cold email outreach (to 50 named HN-cohort friends/peers) | 2 | 5 | 5 | 5 | 5 | High | KEEP — pre-launch concierge-onboarding outreach is highest-conversion channel for first 10–20 |
| Paid Google/Facebook/TikTok ads | 4 | 1-2 | 2 | 1 | 1 | Low | CUT for v1.0 |
| Discord/Slack communities (founder-specific) | 2 | 5 | 4 | 3 | 3 | Medium | KEEP — soft presence in 2–3 communities pre-launch |
| Affiliate program (Meco's playbook) | varies | 5 | 4 | 3 | 2 | Medium (future) | DEFER to v1.0.5 — set up only after 50+ paying users to make economics work |

**Solo-founder channel commit (max 3–4):**
1. **Twitter/X build-in-public** (primary audience-build, compounding, 60+ day commitment)
2. **Substack long-form** (compounding content channel; cross-post Twitter threads as essays)
3. **Cold email / personal outreach** (concierge-first 20-person onboarding)
4. **Launch event channels** (Show HN + Indie Hackers + r/SideProject + Product Hunt — 4 sub-channels run as ONE coordinated multi-day launch sequence; do not treat as "4 separate channels" but as ONE sequence with multiple touchpoints)

**Channels deferred to v1.0.5+:**
- SEO content (after launch, target the post-launch "TLDR-of-TLDRs vs Readless" comparison query specifically as the first SEO target)
- Newsletter-creator placements (after launch with traction proof)
- Podcast guesting
- Affiliate program

**Channels cut:**
- All paid ads
- LinkedIn paid
- Reddit beyond r/SideProject
- Discord/Slack (deprioritize unless founder is already an active member somewhere)

---

## Section 4 — Pre-launch audience-building plan

This is the load-bearing section under Mode C. See `audience_build_sprint.md` for the full 30/60/90 plan. Headline:

- **Days 6–22 of remaining build (now → launch):** Twitter/X account live, 1 build-in-public post per weekday, reply 5x/day to ICP accounts. Plus daily Substack-as-blog post on Sundays. Plus 50-person cold-email list compiled and 20 outreach emails sent. Plus 5 HN-cohort friends recruited as private-beta users.
- **Days 23–52 (post-launch month 1):** continue Twitter cadence, run launch sequence per `launch_playbook.md`, manually onboard every paying user with a 15-min video call (Vohra-pattern), measure PMF-signal weekly.
- **Days 53–82 (post-launch month 2):** if PMF signal hits, scale Twitter cadence and add Substack weekly + 1 podcast appearance. If not, return to concierge-onboarding mode.

---

## Section 5 — Launch playbook

See `launch_playbook.md` for the full sequenced playbook. Headline corrections to the design doc's "Day 18 Show HN + cross-post to X" plan:

### 5a. Launch gate — PMF-signal, not calendar

**Design doc's gate:** Day 18 (now 20–22 per CEO review) calendar. Show HN + cross-post.

**Recommended gate:** Replace pure calendar with **hybrid PMF-signal-and-calendar**:
- **Hard outer calendar bound:** Day 60 from now (gives founder runway; not infinite).
- **PMF-signal soft gate (must pass before public launch):** by end of build (day 22), founder has manually onboarded 10 private-beta users; by day 35, 70% report using the product 3+ days/week for the prior 2 weeks; by day 35, 50% would answer "very disappointed" to the Vohra question.
- **If PMF signal hits before day 60:** launch immediately.
- **If PMF signal does NOT hit by day 60:** launch anyway (the calendar bound), but with explicit acknowledgment that the launch is a continuation of beta, not a victory lap. Treat as discovery, not as scale.

This is a hybrid because pure-PMF-signal gating delays indefinitely; pure-calendar gating fires whether or not the product is indispensable (skill anti-pattern #8). Hybrid bounds risk on both sides.

### 5b. Sequenced multi-channel launch (replaces "Show HN + cross-post to X")

Full hour-by-hour in `launch_playbook.md`. Headline:

| Day | Channel | Action |
|---|---|---|
| -30 to -1 | Build-in-public Twitter + Substack | Daily build posts, weekly long-form |
| -14 | Personal email | Soft pre-announce to ~50 named contacts |
| -7 | Substack long-form | "What I built in 20 days" essay; sets up the story |
| -3 | Twitter | Build-in-public thread previewing launch with screenshot of the magic moment |
| 0 morning (Tue 7am PT) | Hacker News | Show HN with bankruptcy-framing headline |
| 0 + 2h | Twitter | Thread with HN link (after initial HN engagement signal) |
| 0 + 4h | LinkedIn long-form | Story version (different audience overlap, includes the founder-journey angle) |
| 0 + 24h | Indie Hackers | Long-form launch post |
| 0 + 48h | r/SideProject | Compliant cross-post per community rules |
| 0 + 7d | Product Hunt | Separate launch event |
| 0 + 14d | Substack retrospective | "Our first week: X paying, Y lessons" |
| 0 + 14d | Newsletter outreach | Pitch 5 newsletter authors with traction numbers |
| 0 + 30d | Podcast outreach | Pitch 5 podcasts in vertical |

**Risk callouts:**
- HN miss = no recovery if it's the only channel. **Mitigated by having Indie Hackers + r/SideProject + Product Hunt as separate-audience channels in the sequence.**
- All-on-Twitter = no recovery if algorithm shifts. **Mitigated by Substack cadence as parallel compounding channel.**
- Single subreddit = ban risk. **Mitigated by only using r/SideProject (founder-tolerant); avoiding r/productivity etc.**
- **Readless competitive risk:** at HN, expect at least one "how is this different from Readless?" comment within 30 minutes. **Pre-write the answer (bankruptcy framing + structural moat + 60s vs 24h).** Have it in a draft text file, paste-ready.

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing BAND before the price point

**Design doc's anchor:** $9/mo, anchored against Readless's $4.90 floor (CEO PC1 confirmed "hold $9").

**Band evidence (from web search):** $5 (Readless, Browser, Substack-paid floor) → $30 (Superhuman). $10–15 is the niche-indispensable consumer SaaS sweet spot per Readwise data. ChatGPT Plus at $20 is the consumer-AI anchor most ICPs subconsciously benchmark against.

**Is $9 right?**

- For the **HN-cohort Jake persona**: $9 is at the high end of comfort. Jake has ChatGPT Plus, Cursor, Linear, Notion — each adding $9 to his stack requires defending the spend. $9 works if the product clearly displaces 30+ min/week of manual ChatGPT summarization (the design doc's footnote math).
- For the **corporate Maya persona (deferred)**: $9 is FAR too cheap. Maya doesn't price-shop at the bottom; she trust-shops near the top of the band. $19–29/mo for Maya is the more honest positioning, and the "corporate / regulated / can't-use-OAuth" segment justifies the premium.
- For the **annual-billing question**: skill literature shows annual billing dramatically increases retention. Offer 20% off annual ($86/yr) at trial-end. Most premium consumer SaaS do this.

**Recommendation:**
- **v1.0:** Hold $9/mo for the HN-cohort ICP (per CEO PC1). Add **$86/yr annual option (20% off)** at trial-end conversion. The annual option does two things: (a) increases retention dramatically, (b) signals "we're confident in our retention" to skeptics.
- **v1.0.5 (corporate path):** Spin up a separate landing page at `tldrof.com/corporate` or similar at $19/mo or $29/mo for the corporate segment. Concierge-onboarded. Different acquisition channel. Tested as a SEPARATE pricing experiment, not as a tier of v1.0.

**Failure mode flagged (skill anti-pattern #7):** matching Readless's $4.90 would be a trap. Cheapening signals commodity to exactly the trust-led segment that buys near the top of the band. Hold $9 minimum; lean higher for the corporate path.

### 6b. Trial mechanics — revisit M0d

Per M0d, the 7-day free-trial-with-CC-at-Stripe-Checkout-post-trial is right for the HN-cohort ICP and wrong for the corporate ICP. Recommendation:
- **v1.0 (HN-cohort path):** 7-day free trial as designed. Add ONE friction-removal: require CC at signup (not at trial-end). This shifts attracted segment from "trial-shopper" toward "intent-buyer" — modest improvement in retention without changing the architecture significantly.
- **v1.0.5 (corporate path):** No free trial. Concierge demo + 14-day money-back guarantee + annual billing. Different motion entirely.

### 6c. Packaging
- v1.0: single tier at $9/mo or $86/yr. Don't introduce tiers prematurely.
- v1.0.5: introduce "Pro" ($19/mo) only when there's a feature wedge to justify it (the per-newsletter slider from v1.1, advanced auto-forward across all email clients, priority support).
- Never introduce "Free" tier without a clear acquisition rationale — Meco's free tier is a different motion (volume-LTV).

---

## Section 7 — Post-launch growth loops

What compounds for tldrof:

| Loop | In v1.0? | Plan |
|---|---|---|
| Referral mechanics (in-product invite) | NO | **Add to v1.0 if possible:** at first digest, embed "Saved 47 min — share your time-saved with a friend?" share-card image; embed referral code that gives both parties 1 free month. Low engineering cost; first compounding channel. |
| Content compounding (SEO ranking) | NO | **Defer to v1.0.5.** Write 1 comparison post per week starting at launch ("tldrof vs Readless", "tldrof vs Mailbrew (alternative)", "tldrof vs Meco"). 12-month ramp. |
| Network effects | NO | **Not viable for tldrof.** Product doesn't get better as more people use it (each user's digest is independent). No network effects to build. |
| Brand compounding (consistency) | Starts at launch | Twitter cadence + Substack cadence ARE the brand-compounding. Commit 12+ months. |
| Retention as growth (WOM) | YES (potential) | The "share your time saved" mechanic above turns retention into acquisition. **Single highest-leverage growth-loop addition.** |

**If none of the above were viable**, tldrof would be acquisition-treadmill (every new user = new acquisition spend). At least one compounding channel exists (Twitter brand + content), but it's slow. **Adding referral mechanics in v1.0 (or v1.0.5) is the single most valuable growth-loop investment.**

---

## Section 8 — Metrics & instrumentation

Already heavily covered in CEO Review O1-O3 + post-skill-cleanup item 2 (`filter_setup_rate_48h`). Marketing-side adds:

**Acquisition by channel (UTMs):**
- `utm_source=hn|twitter|linkedin|indiehackers|reddit-sideproject|producthunt|substack|cold-email|referral`
- `utm_medium=organic|paid|share-card`
- `utm_campaign=launch-day|build-in-public|comparison-post|...`

**Conversion funnel by channel:**
- Landing-page view → signup → magic-moment-completion → trial-active-day-3 → trial-to-paid
- Specifically track: **trial-to-paid by channel**. Show HN traffic likely has LOWER trial-to-paid than cold-email-concierge traffic. Make this visible.

**Activation rate definition:**
- "Activated" = user completed magic moment AND set up auto-forwarding within 48 hours. (Aligns with CEO post-skill-cleanup `filter_setup_rate_48h` metric.)

**Day-7 / day-30 retention:**
- Cohort by signup week. Track conversion to paid + d30 active rate. Industry benchmark: ~25% first-term churn is normal; target <5% monthly steady-state.

**LTV/CAC ratio:**
- For v1.0, treat CAC as fully-loaded founder time + paid placements + ads (nothing paid in v1.0 so CAC = founder time). LTV at $9/mo with 5% monthly churn = ~$180. LTV/CAC ratio is irrelevant at <100 users; revisit when data exists.

**Vanity metrics to ignore:**
- Twitter followers (correlation with revenue weak; track engaged followers + replies instead)
- HN upvotes (correlation with revenue near-zero; track HN-driven signups + HN-driven paid)
- Total signups (without retention)

**Weekly dashboard (Notion table is fine):**
- Per channel: signups, magic-moment-completion, paid, churn
- Cohort retention curves
- `filter_setup_rate_48h` (the L5 leading indicator)
- WoW growth in paid

---

## Section 9 — Risk analysis

| Risk | Likelihood | Severity | Mitigation |
|---|---|---|---|
| Channel concentration on Show HN (>60% from HN) | High at launch | High | Force multi-channel launch sequence (Section 5); explicit goal: no channel >50% of paid in month 1 |
| Readless counter-launches bankruptcy framing | Medium | Medium | Ship faster on bankruptcy framing; SEO content on "vs Readless" within 2 weeks of launch; structural-moat language (auto-forward + corporate, deferred) |
| Founder time on audience-build stays at 0% during remaining build | High (path of least resistance) | Critical | This is THE plan-killer. Force commit: 20% time minimum days 6–22; 50% time minimum days 23–60. Write it into TODOS.md as a daily checkbox. |
| Free-trial cohort selects for trial-shoppers; first-cohort churn is brutal | Medium-High | High | Concierge-onboard first 20 manually; observe churn signal; iterate before scaling |
| 60-second magic-moment fails to deliver under load (Anthropic rate limits, etc.) | Medium (mitigated by CEO A2 Tier 2) | Critical at launch moment | Already addressed in CEO/Eng reviews; rehearse spike at 50-email backlog with founder's own emails day -7 |
| Pricing $9 race-to-bottom mismatch (corporate ICP undershoot) | Medium | Medium | Hold $9 for v1.0 HN-cohort; spin separate corporate path at $19-29/mo as v1.0.5 |
| Mailbrew-pattern: founder builds beloved product, can't scale solo, gets acqui-hired-into-discontinued | Latent | High over 2-3 year horizon | Strategic Ladder Rung 2+ is the answer; partnerships/creator-channel from day 1 is the hedge |
| Regulatory / publisher complaint about forwarded paid newsletters | Low (architecture defends this) | Low (single domain block if it happens) | Already addressed in Open Question 7; ship as designed |
| Founder runs out of cash/time before traction | Medium | Critical | Make the v1.0 success threshold (15 paying / day 14) the actual go/no-go gate, not 25 paying / day 30. Below 15, pivot conversation; below 5, kill conversation. |
| Outside-voice missed: SOLO FOUNDER + CONSUMER SaaS is structurally hard per Pieter Levels' explicit warning | Existential | Existential | Accept the difficulty. Internalize: 6-month timeline minimum; multiple iterations expected; the "20-day build → launch" plan is build cycle 1 of N, not the whole story. |

---

## Outside-voice critique (simulated independent CMO review)

**Single biggest marketing risk the inside review missed:**

The Strategic Ladder framing (App → Suite → Concierge → Spawn-a-Business Platform) is bleeding into v1 product/marketing decisions in a way the inside review hasn't named. Specifically:
- The "blueprints" join table in v1.0 schema is justified as "Rung 2 prep"
- The MCP/API in v1.1 is justified as "power-user / OpenClaw integration"
- The per-newsletter slider in v1.1 is framed as "strongest moat candidate"

**The risk:** every one of these decisions optimizes for the Rung 2+ user (a future hypothetical) at the cost of v1 marketing clarity for the Rung 1 user (the actual paying customer in the next 60 days). v1 marketing must be ABOUT TLDR-of-TLDRs only, with no narrative leakage from rungs 2–4. **Even the founder's pitch decks and Twitter bio should NOT mention the Strategic Ladder.** Save that for fundraising conversations 18 months out.

**Channel positioned stronger than reality:**

The "M365 / corporate / 400M users" structural moat is positioned as a v1.0 marketing advantage but is structurally impossible to acquire via v1.0's HN-cohort launch channels. Removing this claim from v1.0 launch copy is the honest move (M0d Option B). Keeping it dilutes the bankruptcy framing AND fails to actually deliver corporate acquisitions.

**Audience claim lacking evidence:**

"Engineers, PMs, founders, AI-adjacent professionals who already subscribe to multiple TLDRs" is presented as one persona but contains at least 4 different sub-segments (devs reading TLDR Tech, PMs reading Lenny's, founders reading Stratechery, AI engineers reading Latent Space). Each has different price sensitivity, different LTV, different reachable channels. The v1.0 launch picks "Jake the saturated engineer" specifically because he's most reachable via Show HN; the marketing copy should reflect that one persona, not the omnibus.

**Provocative reframe the founder might not have considered:**

The most interesting acquisition channel tldrof has access to — that is mentioned NOWHERE in the design doc or this review — is **inside the digest itself**. Every digest tldrof sends is an artifact the user reads at the start of their day. Including a one-line "Saved 47 min today — share your time saved with a friend" embed (with auto-generated share-card image) turns every digest into a small acquisition surface. Per CEO PC1 priority order, this is consistent with the structural advantages already positioned. **Single most valuable marketing-loop addition not yet in the plan.** Cost: ~1 day eng. Implement in v1.0.5 if not v1.0.

---

## Outputs / artifacts

- **`marketing_plan.md`** — this file
- **`launch_playbook.md`** — sequenced multi-channel launch playbook with PMF-signal-and-calendar hybrid gate
- **`icp.md`** — ICP specification for Jake (primary) and Maya (deferred)
- **`audience_build_sprint.md`** — 30/60/90-day audience-build sprint (Mode C primary deliverable)
- **`audience_build_journal.md`** — cadence-tracking template

---

## Top 3 action items for THIS WEEK

1. **Set up the Twitter/X account + post the first 3 build-in-public posts** (1 hour total). Follow 50 ICP accounts (Pieter Levels, Lenny, Sahil Bloom, Marc Lou, plus the founders of Readless / Meco / Readwise). Reply 5x/day to ICP accounts on tweets you have something useful to say about. Cadence: 1 build-in-public post per weekday for the remaining build window minimum.

2. **Compile the 50-person cold-email list + send first 10 outreach emails for private-beta** (3 hours). HN-cohort friends + newsletter authors + founders the founder admires. Personalized emails; ask for 30-min video onboarding in exchange for free annual access. Target: 10 said-yes by end of week; 20 by end of build window. This becomes the Vohra-pattern concierge cohort.

3. **Kill the secondary curated picker from v1.0 scope (per M0c anti-feature finding) AND drop M365/corporate marketing claims from v1.0 launch copy (per M0d Option B)**. Costs nothing; reclaims engineering time; sharpens positioning. Both decisions are easier now than after launch. Update design_document.md accordingly so build doesn't drift.

---

## Sources (web research, this run)

- [How Superhuman Grows — How They Grow](https://www.howtheygrow.co/p/how-superhuman-grows)
- [Superhuman's secret to success: Vohra on Lenny's Newsletter](https://www.lennysnewsletter.com/p/superhumans-secret-to-success-rahul-vohra)
- [Superhuman CEO Rahul Vohra on waitlists, freemium pricing — TechCrunch](https://techcrunch.com/2020/02/28/superhuman-ceo-rahul-vohra-on-waitlists-freemium-pricing-and-future-products/)
- [Why We're Bootstrapping Readwise](https://blog.readwise.io/why-were-bootstrapping-readwise/)
- [Readwise 2026: Usage, Revenue, Valuation & Growth Statistics](https://www.fueler.io/blog/readwise-usage-revenue-valuation-growth-statistics)
- [Readless vs Readwise Reader (2026): Honest Comparison](https://www.readless.app/compare/readless-vs-readwise-reader)
- [Meco Pricing 2026: Free vs Pro (Is $35/Year Worth It?)](https://www.readless.app/blog/meco-pricing-2026)
- [Meco: The #1 newsletter reader](https://meco.app/)
- [Mailbrew Alternatives — Digest](https://usedigest.com/blog/mailbrew-alternatives/)
- [Show HN by the Numbers: 188,000 Posts, 14 Years of Data — Daniel King 2026](https://danfking.github.io/blog/2026/04/23/show-hn-by-the-numbers/)
- [How to Launch on Hacker News: A Practical Guide to Getting 500+ Upvotes — Calmops](https://calmops.com/indie-hackers/hacker-news-launch-500-upvotes/)
- [News Subscription Churn Rate Benchmark 2026](https://retentioncheck.com/churn-benchmarks/news-subscriptions)
- [Subscription churn metrics and benchmarks — Elena Verna](https://www.elenaverna.com/p/subscription-churn-benchmarks-and)
- [How to Use #BuildInPublic on X to Market Your SaaS — Inflow Labs](https://inflowlabs.com/blog/how-to-use-buildinpublic-on-x/)
- [Building in Public: The 10-Year Distribution Strategy — SoftwareSeni](https://www.softwareseni.com/building-in-public-the-10-year-distribution-strategy-behind-solo-founder-revenue/)
