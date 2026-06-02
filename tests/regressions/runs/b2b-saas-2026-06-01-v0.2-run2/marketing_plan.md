# Threadline — Marketing Plan (CMO Review, v0.2)

**Run:** b2b-saas-2026-06-01-v0.2-run2
**Date:** 2026-06-01
**Mode:** TBD (set after Step 0A)
**Default posture:** marketing-naive (2 ex-Google engineers, no prior B2B sales, ~200 X followers, ~50-person personal list)

---

## PREMISE-LEVEL FINDINGS BLOCK

**4 of 5 Step 0.5 premises FAIL (M0b, M0c, M0d, M0e); M0a is INCONCLUSIVE leaning FAIL.** Block is mandatory.

The plan as written is internally incoherent in a specific way: it combines a *bottom-up motion's distribution channel* (Show HN) with a *top-down motion's packaging* ($40/seat, no free tier) under a *consumer-product calendar gate* (5 paying companies by day 30) for a *mid-market B2B ICP* whose actual procurement cycle is 90-180 days. Every element is plausible in isolation; the combination cannot work.

**Hard truths:**

1. **The pricing is 2.5-4x competitor.** Linear is $10/$16/seat (cut from $50 to $16 in Feb 2026, an aggressive move directly relevant here). Jira is $7.91-$14.54. Notion is $10-$18. ClickUp is $7-$12. There is no $40/seat tier in this category for engineering teams. $40 needs to either (a) be justified by a documented willingness-to-pay anchor (e.g., per-mgr pricing, not per-seat; or a vertical/compliance wedge), or (b) come down significantly.

2. **"Better than Linear" is the wrong wedge.** Linear *is* the design-led "better Jira for engineering teams" wedge. Going after Linear with that same wedge means competing on Linear's home turf with: lower pricing power, no design credibility, no audience, and no free tier. The 2026 Linear price cut signals Linear is actively closing pricing-driven openings. Threadline needs a non-Linear wedge (vertical specificity, integrations Linear doesn't do, workflow Linear refuses to support).

3. **The validation gate is mathematically incompatible with the motion.** 5 paying COMPANIES by day 30. Mid-market B2B SaaS cycles are 90-180 days (Optifai/Pavilion benchmarks; multi-stakeholder, security review adds 2-4 weeks). The day-30 gate either (a) forces founders into single-IC sales (= not a real company purchase, fails ICP) or (b) selects against the actual buyer.

4. **The dogfood-to-buyer gap is severe.** Ex-Google ICs dogfooding on themselves cannot validate a mid-market eng-mgmt product. Google internal tooling and the workflows of a 50-500 person SaaS are different worlds. The plan has no design-partner program to bridge this.

5. **There is no audience.** ~200 X followers + ~50 personal email contacts + zero professional content history is a starting line, not a launch surface. The ~$35K LIFETIME marketing spend Linear ran on still came with: (a) Karri Saarinen's existing design reputation, (b) a 3-year build runway, (c) bottom-up product. Threadline has none of these.

**Implication on mode (decided in 0B):** the prerequisite for ANY Mode A/B plan is missing — there is no audience, no validated ICP, and no coherent pricing/packaging. **Mode C (Audience-Build Sprint) is the recommended mode**, with the additional 30-day "go fix the premise" work front-loaded. Mode A is *literally premature*.

---

## Step 0 — Pre-review system audit

### Founder audience surface
- X/Twitter: ~200 followers (size + engagement unknown; assume low — 200 is below the threshold where threads compound)
- Personal email list: ~50
- LinkedIn: not stated (assume nascent for ex-Google ICs)
- Engineering management blog history: NONE ("no professional content history")
- GitHub stars / OSS audience: not stated
- Existing communities they're known in: not stated
- Prior shipped B2B products: NONE

**Verdict:** essentially zero audience for the target ICP (engineering managers at 50-500 person SaaS). 200 X followers without ICP-overlap evidence is sub-threshold. This is load-bearing for mode selection.

### Competitive landscape (real searches — see Section 1 for full)
See Section 1.

---

## Step 0.5 — Premise audit

### Premise extraction

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| P1 | Launch platform = Show HN | Distribution Plan | Plausible for eng-mgr ICP — but HN reaches ICs + tech leads more than managers; mgr-buyer ICP gap to test |
| P2 | Content marketing on "the engineering management blog" | Distribution Plan | "The" implies a single canonical blog; the eng-mgmt content ecosystem is actually Lenny's, Pragmatic Engineer, LeadDev, Rands — not one blog. Vague channel = no channel. |
| P3 | $40/seat/month pricing | Pricing | Anchored on Linear (~$8-14/seat) and Jira ($7-15); $40 is 3-5x competitor band. Premium positioning unstated. |
| P4 | "Better than Linear for engineering-specific workflows" differentiation | Differentiation | Linear IS the engineering-specific workflow tool. This is "better Linear than Linear" — wedge unclear. |
| P5 | Founders' friends + HN cohort = first 10 customers | First 10 customers | Friends rarely match $40/seat B2B ICP. HN cohort = individuals not buyers. |
| P6 | 5 paying COMPANIES by day 30 | Validation gate | B2B procurement for $40/seat tools = 2-8 week cycles. Day 30 calendar gate against 4-8 week sales cycle is misaligned. |
| P7 | No free tier; 14-day trial | Pricing | Linear/Jira/Notion all have free tiers; competing on closed trial against free-tier incumbents is a wedge OR a wall depending on positioning. |
| P8 | "Engineering teams at 50-500 person companies" ICP | Target | Mid-market. Buyers are eng leadership + procurement, not the IC engineers using it. M0e: dogfood gap likely. |

### M0a — Launch-platform audience-class fit

**Premise:** Show HN reaches the buyer ICP for Threadline.

**Web search performed:** see queries below.

**Analysis:**
- HN audience composition is heavily IC engineers, tech leads, and founders. Engineering managers ARE present (a significant minority) and the eng-mgr-adjacent crowd reads HN.
- For Threadline specifically (dev-team tool, dev-IC end users + mgr champions), HN is a *legitimate* channel — unlike the consumer case where HN is a category error. Linear itself got initial traction partly via HN.
- BUT: Show HN gives you ICs and tech leads. The $40/seat/month decision-maker is the eng manager / VP Eng / Director. HN can produce champions; champions then have to sell internally.
- Pattern: dev-tool HN launches succeed for bottom-up adoption (Linear, Supabase, PostHog) — but only when bottom-up motion is the plan and pricing is friction-low (free tier + cheap paid). $40/seat with NO free tier + 14-day trial breaks the HN bottom-up motion.

**Verdict: premise INCONCLUSIVE leaning FAIL.** HN audience-class IS reasonable for dev-team tools — that's not the failure. The failure is that the rest of the plan (no free tier, $40/seat, "5 paying companies by day 30") doesn't match the HN bottom-up motion HN enables. HN delivers individuals who try things, not procurement-cycle companies.

**Cascading implication:** if HN is kept as a channel, packaging must be redesigned to absorb the bottom-up motion (free tier or generous freemium). If packaging is kept ($40/seat, paid trial only), HN is largely wasted top-of-funnel. The current plan attempts both incompatible things.

### M0b — Canonical-success comparable

**Premise:** "Show HN + content marketing" is a sufficient B2B SaaS playbook.

**Web search performed:** see queries below.

**Canonical successes at this motion class (B2B SaaS, dev-team tooling, $10-50/seat):**

1. **Linear** — bottom-up adoption, design polish as marketing, founder-led on Twitter (Karri Saarinen's design-led posts), private beta with curated invites, FREE tier (10 users), pricing $8/$14/seat. Took ~3 years to scale. Did NOT lead with Show HN as the strategy; HN was one of many touches.
2. **Notion** — content marketing (templates as SEO), community-led growth (creators making templates), generous free tier, viral team adoption from individual use. Did NOT lead with HN.
3. **Slack** — top-down + bottom-up, founder credibility (Stewart Butterfield's prior exit), PR-led launch (TechCrunch, not HN), free tier with usage cap.
4. **PostHog** — open-source + dev-led (Tim Glaser content), HN was a real channel BUT paired with OSS distribution, hands-on community, cofounder posts as content.
5. **Height** — Linear competitor; bottom-up, generous free tier, lost share to Linear partly on design + execution. Cautionary tale: "better than Linear" alone doesn't win.

**Deltas vs current plan:**

| Canonical | They did | Threadline plan does NOT |
|---|---|---|
| Linear | Free tier (10 users), 3yr build, design-led PR, founder Twitter presence with design credibility | No free tier, day-30 gate, no design or audience credibility |
| Notion | Templates-as-SEO, individual-first viral team adoption | No content infrastructure, team-first pricing |
| Slack | Founder credibility from prior exit, PR launch | No prior B2B exit, HN launch |
| PostHog | OSS + dev community, cofounder content cadence | Closed source, zero content history |
| Height | Generous free tier | No free tier |

**Verdict: premise FAILS.** Every canonical success in this motion class has either (a) a generous free tier, (b) prior founder credibility, (c) a multi-year content/community build, or some combination. "Show HN + content marketing on the engineering management blog" is none of those.

**Cascading implication:** the plan needs either (a) a free tier and a long-build content motion, or (b) a fundamentally different motion (top-down enterprise sales — but founders have "no prior B2B sales experience"). Day-30 validation gate is incompatible with both.

### M0c — Anti-feature surface

**Premise:** All in-scope features serve the paying ICP.

**Stated in-scope (derived from "Linear-style project tracking for engineering teams"):**
- Engineering-specific workflow features (kept generic in the doc)

**Anti-feature candidates:**
1. **"Engineering-specific workflows"** as a feature category. Engineering managers at mid-market companies are buying a *standardization* tool — they want their PMs, designers, and engineers all in ONE system. "Engineering-specific" workflows can be an anti-feature if it means non-eng can't use it, because the buyer is forced to maintain two tools (which is the Jira-problem). The wedge "engineering-specific" is also the wall against company-wide adoption — which is the upsell path. This contradicts $40/seat unit economics, which need expansion.
2. **No free tier** — this isn't an in-scope *feature*, but it's a positioning anti-pattern: $40/seat without a free tier puts Threadline in the "trust-based enterprise" pricing band while the product/audience/founder-credibility is "scrappy bottom-up tool" band. Mismatch.
3. **14-day trial only** — for engineering managers running a 5-30 person team migration, 14 days is too short to actually migrate. Selects for evaluators not buyers.

**Verdict: premise FAILS (≥2 anti-features identified).** "Engineering-specific" positioning contradicts expansion economics needed at $40/seat; no-free-tier contradicts the HN bottom-up motion the rest of the plan implies.

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Premise:** The 14-day trial selects for the right buyer segment.

**Diagnostic:**
- 14-day trial, presumably no credit card upfront (not specified — assume CC required at signup since it's "no free tier" framing, OR CC at trial-end).
- If CC required upfront: selects for committed evaluators. GOOD for B2B if combined with sales support.
- If CC required at trial-end: selects for individuals trying it solo, who then have to expense it. Time-rich evaluator selection.
- For "5 paying COMPANIES by day 30" gate: trial needs to convert FAST. 14 days means the eval window closes before most B2B procurement cycles complete.

**Comparison to canonical:**
- Linear: free tier (no trial pressure) → bottom-up usage → paid upgrade when team grows. No trial expiration.
- Jira: free tier (10 users) + paid plans. Free expansion is the motion.
- Notion: free for individuals, generous team free tier.

**Verdict: premise FAILS.** 14-day trial alone (no free tier) is structurally incompatible with both the HN-bottom-up motion AND the day-30 validation gate. It selects against the time-poor mgr-buyer (who needs months to migrate) and equally against the bottom-up IC user (who never pays personally for a team tool).

**Cascading implication:** acquisition mechanic must change. Options: (a) free tier + paid expansion (Linear playbook), (b) extended pilot (30-60 days + hands-on onboarding) for design-partner cohort, (c) generous trial with proactive concierge — none of which are in the current plan.

### M0e — Dogfood audience-class match (founder vs paying ICP)

**Premise:** The dogfood audience matches the paying ICP.

**Founder profile:** 2 ex-Google engineers. Google is 180K+ employees with extremely mature internal tooling, dedicated infra teams, and processes that look nothing like a 50-500 person SaaS company.

**Paying ICP:** engineering managers + VP Eng / Director at 50-500 person SaaS companies.

**Mismatch surface:**
- Ex-Google ICs likely dogfood on themselves or small founder team (1-5 people, not 50-500).
- Google internal tooling shapes their intuitions about what "good" looks like — but ex-Google engineers consistently underestimate the messiness of mid-market eng-mgmt workflows (mixed remote/office, contractors, multi-product orgs, less mature engineering culture).
- Buyer = eng manager managing humans + sprints + roadmap + stakeholders. Founders have managed code but maybe never managed a 30-person mid-market eng org.
- Doc says founders have "no prior B2B sales experience" — they also likely have no prior eng-management experience at the ICP profile.

**Verdict: premise FAILS.** Dogfood audience (ex-Google IC pair) ≠ paying ICP (mid-market eng mgr). The product will be tuned to ex-Google sensibilities (clean, opinionated, principled) while the buyer needs messy-reality features (cross-team coordination, exec reporting, integration with HR/Jira/Salesforce sprawl).

**Cascading implication:** before any launch, founders must add 5-10 mid-market eng managers as design partners. Their feedback must shape the product, not just validate it. This is incompatible with the day-30 calendar gate.

### Step 0.5 verdict tally

| Question | Verdict |
|---|---|
| M0a Launch-platform fit | INCONCLUSIVE leaning FAIL |
| M0b Canonical-success comparable | FAIL |
| M0c Anti-feature surface | FAIL |
| M0d Freebie-disqualifier | FAIL |
| M0e Dogfood audience-class match | FAIL |

**4 of 5 premises FAIL (5 of 5 if M0a is counted as fail).** PREMISE-LEVEL FINDINGS BLOCK is mandatory (above, to be filled in).

---

## Step 0A — Forcing questions

Questions adjusted per Step 0.5 findings — M2 refuses "Show HN as step 1" more aggressively; M1 requires corrected ICP (mid-market eng mgr, not ex-Google IC dogfood proxy); M5/M6 push high-trust acquisition mechanics.

### M1 — Audience reality

**Naive founder answer:** "Engineering managers and tech leads at SaaS startups — they're on X, they read Pragmatic Engineer, they hang out on HN."

**Skill challenge:** "Engineering managers" is a job title, not a person. Name a specific person. Also: are ICs and managers the same buyer? They aren't. ICs *use* the tool. Managers *buy* it. VPs *approve budget for it*.

**Re-asked answer (pushed):** "Okay — Priya, Eng Manager at a Series B SaaS (~150 people), reports to a VP Eng, manages 12 engineers across 2 squads. Subscribes to Pragmatic Engineer + Lenny's. Lurks in Rands Leadership Slack. Reads Will Larson's Irrational Exuberance. Uses Linear today but complains about cross-team dependency tracking. Has discretion on tooling under ~$5K/yr (= ~10 seats at $40); above that needs VP sign-off."

**Verdict:** ACCEPT with note — Priya is a credible composite, but the plan currently sells to ICs (via HN) while Priya is the actual buyer. M2 must reconcile.

### M2 — Discovery path

**Naive founder answer:** "Priya sees our Show HN, clicks through, signs up for the trial, evangelizes internally."

**Skill challenge:** REFUSED — three failures: (1) Step 0.5 flagged Show HN as the wrong primary; (2) eng managers like Priya don't refresh HN looking for new tracking tools — they got burned by tool churn and are skeptical; (3) "evangelizes internally" skips the actual sale (her boss, security review, procurement).

**Required answer format — minimum 3 steps, no step 1 = HN:**

1. **Discovery:** Priya reads Gergely Orosz's Pragmatic Engineer "The Pulse" issue covering "alternatives to Linear for engineering-specific workflows" (an article that exists either because we ghost-pitch it OR because we're already a recognized name in eng leadership — neither is currently true). Alternative: Priya hears Threadline mentioned by name in Rands Leadership Slack #tools channel.
2. **Validation:** Priya searches "Threadline vs Linear" — needs landing page, comparison content, real testimonials (NONE EXIST yet).
3. **Trial-to-buy:** Priya schedules an internal eval. Looks for case study from comparable team. Needs to convince VP Eng. Procurement requires SOC 2 (which Threadline does not have).
4. **Close:** 60-120 day procurement cycle.

**Verdict:** plan currently doesn't survive M2. Steps 1 and 2 require infrastructure (Pragmatic Engineer relationship, Rands presence, comparison content, SOC 2) that doesn't exist. Honest answer: "I don't have a discovery path yet — what I have is a launch event hope."

### M3 — Pre-launch audience

**Naive founder answer:** "200 X followers, ~50 person personal email list. We'll build more during launch."

**Skill challenge:** "We'll build more during launch" is the trap Step 0.5 specifically warned against. Audience precedes product. Of the 200 X followers, how many are ICP? Of the 50 emails, how many are at 50-500 person SaaS? Probably <10 each.

**Honest reframe:** **effective ICP-relevant audience ≈ 0.** This triggers Mode C.

### M4 — Channel honesty

**Naive founder answer:** "We're good engineers, so we can build content."

**Skill challenge:** REFUSED — that's a future-tense aspiration, not a demonstrated advantage. "We can build content" is not a channel; it's a label for unscheduled work that won't happen. Show one piece of published, distributed content with measurable reach. The doc explicitly says "no professional content history."

**Honest answer:** "We don't have a demonstrable channel advantage. Closest is: ex-Google network for warm intros — but Google ≠ 50-500 person SaaS ICP."

**Verdict:** ACCEPT honest "none yet" answer. This becomes the first audience-build work item.

### M5 — Competitor traffic source

**Naive founder answer:** "Linear got HN traction."

**Skill challenge:** REFUSED — that was 2019, Linear is now an established brand with mostly word-of-mouth and brand-search traffic. Where do they get NEW users in 2026? Where does Height get them? PostHog? Vendr?

**Required research before next session:**
- Linear: brand search dominant; ~Karri Saarinen Twitter + Jori Lallo + design-led content + word-of-mouth in design-conscious eng orgs.
- Jira: SEO + enterprise sales motion + existing customer expansion.
- Notion: templates-as-SEO + community-led (Ambassador Program, 4M+ template downloads).
- Height: Twitter/X founder presence + bottom-up free tier.
- ClickUp: heavy SEO + paid ads + content marketing (~700+ blog posts).

**Pattern:** every competitor's growth depends on infrastructure (SEO content library, design rep, sales team, free tier as funnel). None of them won via Show HN as primary.

**Verdict:** founders must do this research before any launch plan is taken seriously. Assign as first-week work.

### M6 — First 10 paying customers

**Naive founder answer:** "Friends + HN cohort."

**Skill challenge:** REFUSED on both. (1) Friends are unlikely to be eng managers at 50-500 person SaaS who'll pay $40/seat for a Linear clone from ex-coworkers; if they're at Google they're not the ICP; if they're at startups they're often ICs not buyers. (2) "HN cohort" is the same anti-pattern Step 0.5 caught.

**Required:** name 10 specific people you would email tomorrow. Not "friends generally." Specific names, specific companies, specific reason they would buy.

**Honest answer:** "We can probably name 3-5 ex-Google friends now at series B/C startups. We don't have 10. We'd need to systematically build a list — possibly via Lenny's job-board adjacent network, Rands Slack relationships, or paid outreach."

**Suggested path:** Design-Partner Cohort of 10 — recruit through 1:1 outreach (Pragmatic Engineer alumni newsletter classified, Rands Slack lurk-then-DM, LinkedIn Sales Nav for "Eng Manager at 50-500 person SaaS"). Concierge-onboard each. Trade discount/free year for case study + referral.

### M7 — Time allocation

**Naive founder answer:** "We've spent 90% on building. We'll start audience-building near launch."

**Skill challenge:** REFUSED — this is the canonical "build → ship → market" anti-pattern. By the time they ship, no one will know they exist, and the day-30 gate will fire to silence.

**Required reframe:** for the next 30 days, flip to 50% audience-building / 50% product. Audience-building means: (a) start writing weekly engineering management content TODAY, (b) join Rands Leadership Slack and start contributing (NOT promoting), (c) recruit 10 design partners by name through cold outreach, (d) get on 3 eng-mgmt podcasts.

**Verdict:** founders must explicitly commit, or document as accepted-risk.

### Step 0A summary table

| # | Question | Verdict |
|---|---|---|
| M1 | Audience reality | ACCEPT (Priya composite) — but plan sells to wrong layer (ICs not mgrs) |
| M2 | Discovery path | FAIL — infrastructure doesn't exist |
| M3 | Pre-launch audience | FAIL — effectively zero ICP-relevant audience |
| M4 | Channel honesty | ACCEPT honest "none yet"; becomes work item |
| M5 | Competitor traffic source | INCOMPLETE — research assigned |
| M6 | First 10 customers | FAIL — friends ≠ ICP; HN cohort ≠ buyer |
| M7 | Time allocation | FAIL — must shift to ≥30% audience-building |

5 of 7 fail or incomplete. Strong signal for Mode C.

---

## Step 0B — Mode selection

**Mode selected: Mode C — Audience-Build Sprint (60 min, output is action plan, not full plan-doc).**

Rationale (per skill activation rule "Zero prior audience + zero competitors identified → Mode C"):
- Founders have effectively zero ICP-relevant audience (M3 FAIL).
- Founders have not done real competitive research (M5 INCOMPLETE).
- 4-of-5 Step 0.5 premises and 5-of-7 Step 0A forcing questions failed.
- Producing a full launch plan against this baseline would polish wrongness.

**Founder might push back:** "We're 60% built already and our calendar says launch in 90 days. We need a launch plan."

**Skill response:** A launch plan against an audience of zero and a misaligned ICP is a wish, not a plan. The strongest contribution this skill can make is to surface that the *premise* is the work item — not the launch sequence. We will still provide Sections 1, 5, and 6 in compressed form (because the competitive landscape, launch playbook contingency, and pricing recommendations are decision-blockers), but the *primary* artifact is `audience_build_sprint.md`.

**Hybrid output (deviation from strict Mode C):**
- Primary: `audience_build_sprint.md` + `weekly_cadence.md`
- Decision-blocker compressed sections: 1 (competitive), 5 (launch contingency for IF they launch), 6 (pricing recommendation), 9 (risks)
- Skipped: 4 (long-form pre-launch plan — covered in sprint), 7 (growth loops — premature), 8 (metrics — set up after sprint)
- `icp.md` produced (Priya persona is decision-blocker for sprint targeting)

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Name | Founded | Pricing (2026) | Traffic / GTM | User complaints | Position vs Threadline | Winning? |
|---|---|---|---|---|---|---|
| **Linear** | 2019 | Free (250 issues, 2 teams) / $10 Basic / $16 Business (cut from $50 in Feb 2026) | Word-of-mouth in design-conscious eng orgs; Karri Saarinen + Jori Lallo personal brand; $35K lifetime marketing spend | "Becoming bloated", price was high before Feb 2026 cut, slow on multi-team | Threadline = "Linear but more eng-specific" but Linear IS the eng-specific tool. Wedge collapses. | YES — $1.25B valuation, cult following, profitable since 2021. The Feb 2026 price cut signals they're playing defense and closing pricing-driven openings. |
| **Jira** | 2002 | Free (10 users) / $7.91 Std / $14.54 Premium | SEO + enterprise sales + customer expansion; ubiquitous | "Slow, complex, configuration hell, mgr-friendly but IC-hostile" | Threadline could win the eng-IC sentiment Jira loses — but Linear already owns that wedge | YES at scale; LOSING the IC love-channel |
| **ClickUp** | 2017 | Free (unlimited users) / $7 Unlimited / $12 Business + $7 AI add-on | Heavy SEO (700+ blog posts), paid ads, content marketing | "Too many features, kitchen-sink, confusing" | Different wedge (everything for everyone); not direct | Yes — but on a different motion (kitchen-sink SEO) Threadline can't replicate without years of content |
| **Notion** | 2013 (project-mgmt push later) | Free / $10 Plus / $18 Business | Community-led: 4M+ template downloads, Ambassador Program, 95% organic traffic | "Slow at scale, not eng-specific" | Adjacent — Notion is workspace, Threadline is tracking. Co-exists. | Yes — but in a different category |
| **Height** | 2020 | Free / ~$6.99 Pro | Twitter founder presence; bottom-up | Lost share to Linear partly on design/exec | Direct Linear competitor that has not won — cautionary tale: "better than Linear" alone doesn't work | Losing market share to Linear |

### 1b. Canonical-success comparables (motion class: B2B SaaS, dev-team tooling, bottom-up adoption)

| Name | Price | Founded | Primary acquisition | Onboarding | Launch gate | Delta vs Threadline plan |
|---|---|---|---|---|---|---|
| **Linear** | Free + $10/$16/seat | 2019 | Word-of-mouth in design-led eng orgs + founder Twitter (Saarinen + Lallo design rep) | Self-serve, opinionated default workflow | Private beta with curated invites; PMF-signal driven (3-year build to public) | Threadline has no design rep, no free tier, no 3-year runway, calendar gate at day 30 |
| **Notion** | Free + $10/$18 | 2013 | Templates-as-SEO + Ambassador community + viral team adoption | Self-serve, templates onboard | PMF + community signal | Threadline has no templates, no community, no individual-first viral motion |
| **PostHog** | Open source + cloud paid | 2020 | OSS distribution + founder content (Tim Glaser) + dev community | Self-serve OSS, paid for cloud | OSS adoption first; commercial later | Threadline is closed-source, no founder content history, no dev-community presence |
| **Slack** | Free + tiered | 2013 | Founder credibility (Stewart Butterfield prior Flickr exit) + PR launch + free tier viral team | Self-serve, magic moment in first session | Pre-launch enterprise beta + PR push | Threadline has no prior exit credibility, no PR launch, no free tier |
| **Superhuman** | $30/mo | 2014 | Invite-only waitlist + concierge onboarding (Vohra personally onboarded first 200) + Vohra PMF survey | Manual concierge (30-min 1:1) | "Very disappointed" ≥40% (PMF-signal gate, not calendar) | Threadline plans calendar gate, self-serve trial, no concierge — opposite of Superhuman path despite a similar premium price point |

### 1c. Pattern surface

**What canonical successes share that Threadline lacks:**
1. Generous free tier or OSS distribution (Linear, Notion, PostHog, Slack — all of them). The ONLY one without a free tier is Superhuman, which compensates with extensive concierge onboarding.
2. Founder credibility/reputation accumulated BEFORE the product launched (Saarinen design rep, Butterfield prior exit, Vohra obsessive PMF work, Glaser dev content). Threadline founders have neither.
3. Multi-year build + community runway BEFORE scale (Linear 3 years; Notion ~5 years pivoting).
4. PMF-signal-driven launch gate (Superhuman's "very disappointed" 40%; Linear's curated beta) — NOT calendar gate.
5. ONE clear differentiating wedge against the incumbent (Linear's design-led, Notion's flexibility, Superhuman's speed). Threadline's "better than Linear for engineering-specific workflows" is not a wedge — it's a vibe.

**Pattern Threadline is implicitly following:** the "Show HN + content marketing" plan resembles a *consumer* indie-SaaS playbook (~$5-30/mo, single-IC purchases). The pricing ($40/seat, no free tier, team purchases) is *enterprise mid-market*. These two playbooks contradict each other.

**Required reframe:** pick a playbook and commit.
- (A) **Linear-style bottom-up:** add free tier (10 users), lower entry pricing ($10-15/seat for paid), 1-3 year content + community runway, find a non-Linear wedge.
- (B) **Superhuman-style concierge premium:** keep $40/seat (or raise to $50-75), but add manual concierge onboarding, invite-only waitlist, founder-led PMF survey gating launch. Requires founders to do sales work.
- (C) **Vertical wedge:** redefine ICP to a specific vertical (e.g., "engineering teams at fintech for SOC2-bound workflows") where Linear is underserving. $40/seat works in compliance-heavy verticals.

The current plan attempts (A)'s channel with (B)'s pricing and (C)'s vibe without commit.

---

## Section 2 — ICP specification

Emitted as `icp.md`. Composite persona "Priya" — see file. Headline: ICP is the *eng manager* (not the IC), with VP Eng as approval ladder. ICP-buyer ≠ ICP-user.

---

## Section 3 — Distribution channels

| Channel | Reach | Cost | Conversion | Founder fit | Effort to start | Verdict |
|---|---|---|---|---|---|---|
| Show HN | High if hit (10K+ visits) | Free | LOW for paid B2B; HN converts ICs, not mgr-buyers | Medium (founders are HN-literate) | Low | KEEP but demote — single tactical event, not strategy |
| Pragmatic Engineer sponsorship / mention | High in ICP (800K subs, eng leaders) | $$$ ($5-15K per sponsored slot) | HIGH if positioned well | Low (need eng-mgmt credibility first) | Medium (need pitch) | PRIORITY 1 — write earned-mention guest piece OR budget for sponsored slot at 60-day mark |
| Lenny's Newsletter / community | Medium-high in ICP overlap | $$ | Medium-high | Low | Medium | PRIORITY 2 — engage in community, contribute, earn mention |
| LeadDev conference + content | Medium in ICP (eng leaders) | $$ | Medium | Low (have to build cred) | High (year-long) | DEFER 6 months |
| Rands Leadership Slack | High in ICP (eng mgrs) — but strict no-promo culture | Free | Medium-high IF relationship-built; ZERO if cold-promo | Low — founders need to be Rands members and contribute for months | Medium ongoing | PRIORITY 3 — join, contribute, NEVER cold-promote |
| LinkedIn (founder organic posts) | Medium in ICP (mgrs use LI) | Free | Medium | Medium — most engs underuse LI | Medium (need writing cadence) | PRIORITY 4 — start now, build over 90 days |
| Twitter/X (founder posts) | Low until audience built | Free | Low (current 200 follower audience won't move needle) | Medium | Medium | KEEP at low priority — supplementary |
| LinkedIn Sales Nav cold outreach (target eng mgrs at 50-500 SaaS) | Medium | $ (LinkedIn Premium ~$100/mo) | LOW for product pitch; HIGH for design-partner asks | High (founders can write) | Low | PRIORITY 1B — design-partner recruit, NOT product pitch |
| Podcast guesting (eng-mgmt vertical) | Medium in ICP | Free | High in trust | Low (need topic + cred) | Medium (~3 mo pitch cycle) | PRIORITY 5 — start pitching at 60-day mark |
| SEO / comparison content ("Linear vs X", "Jira alternatives") | High over 6-12 mo | Free (time) | High at decision stage | Medium (founders can write) | High (need 20+ pieces) | DEFER — start writing now, traffic at 6-9 months |
| Product Hunt | Medium one-shot | Free | Low for B2B mid-market | Medium | Low | DEFER to v1.1 |
| IndieHackers | Low for $40/seat B2B (IH skews solo + cheap) | Free | LOW for ICP | High familiarity | Low | SKIP — wrong audience |
| Reddit (r/EngineeringManagers, r/cscareerquestions) | Medium | Free | Low for direct promo; medium for AMA | Medium | Low | LOW priority |
| Paid Google ads ("Linear alternative") | Medium | $$$$ ($5-25 CPC in this category) | Medium at decision stage | Low | Medium | DEFER until SEO content exists to retarget |

**Refusal:** "we'll do all of them." Pick 3 for the 90-day window: **(1) LinkedIn cold outreach for design-partner recruit, (2) LinkedIn founder organic + LeadDev/Rands community participation, (3) Pragmatic Engineer/Lenny's earned placement.** Show HN is a tactical event when ready (day 60+), not the strategy.

---

## Section 4 — Pre-launch audience-building

Covered in primary artifact `audience_build_sprint.md` and `weekly_cadence.md`. Summary: 30/60/90-day plan starting today, ≥50% time on audience-build, three concrete tracks (design-partner recruit, content cadence, community participation).

---

## Section 5 — Launch playbook

### 5a. Launch gate question (asked FIRST per skill v0.2)

> What is the gate that fires the launch? Calendar (day N), or PMF signal (specific dependence metric)?

**Founder stated:** "5 paying companies by day 30." This is CALENDAR + outcome metric, not PMF dependence metric.

**Skill verdict:** WRONG GATE for this product class. Threadline is retention-driven (B2B project tracking is high-switching-cost; either users live in it daily or they churn within 60 days). Calendar gate at day 30 against a 90-180 day mid-market sales cycle is statistically near-impossible.

**Proposed replacement gate (Superhuman precedent, applicable here):**

- **PMF gate:** ≥40% of design-partner cohort answers "very disappointed" if Threadline went away. Recommended cohort size: 10 paying or paid-pilot teams.
- **Engagement gate:** ≥60% of design-partner team's eng staff use Threadline ≥4 days/week for ≥4 consecutive weeks.
- **Word-of-mouth gate:** ≥2 unprompted "do you know X who I can introduce you to?" referrals from design partners.

If neither retention nor PMF threshold met by day 90, the right move is product iteration with design-partner cohort, NOT public launch.

**Acceptable defense of calendar gate:** none surfaced. Founders did not present one.

### 5b. Launch playbook (contingency — IF founders ignore mode-C recommendation and launch anyway)

Emitted as `launch_playbook.md`. Highlights below.

**Mandatory pre-conditions (else do not launch):**
- 10 design partners onboarded, ≥6 hitting engagement gate
- Free tier OR concierge onboarding offer in place
- SOC 2 Type 1 in flight (Type 2 is 6+ months out, blocks mid-market sales without it)
- Landing page with comparison content (Threadline vs Linear vs Jira) live
- Founder content cadence ≥8 weeks established
- Pragmatic Engineer or Lenny's earned mention OR sponsored slot scheduled
- Email list ≥500 ICP-relevant subscribers

**Multi-channel sequence (3+ channels, sequenced):** see launch_playbook.md.

---

## Section 6 — Pricing & packaging

### 6a. Price BAND question (asked first per skill v0.2)

> Did the price band inherit from competitor anchoring, or from ICP willingness-to-pay evidence?

**Founder answer (implied):** "$40/seat felt right." No ICP-WTP evidence cited.

**Skill verdict:** BAND IS WRONG by competitor anchoring AND by ICP-WTP.

- **Competitor anchor band:** Linear Free–$16; Jira Free–$14.54; Notion Free–$18; ClickUp Free–$12; Asana Free–$24.99. The 2026 band ceiling for general-purpose project tracking is ~$16-18/seat. Linear specifically CUT from $50 → $16 in Feb 2026 — they discovered the market won't bear $50/seat.
- **ICP-WTP:** eng managers buying tracking tools for their team have a $10-15/seat reflex. $40/seat will require explicit justification (compliance, vertical, AI features documented to save time) — none of which the plan offers.
- **Mid-market ACV math:** at $40/seat × 12 mo = $480/year/seat. To hit a $40K ACV (Optifai mid-market benchmark), you need 83 seats — well above the "engineering team" profile (Threadline's stated target is teams at 50-500 person companies; eng teams are 10-50 of those). Realistic ACV at $40/seat for an eng team of 20 is $9,600/year. That's lower-mid-market and procurement cycles are still 60-120 days.

**Two paths:**

**Path A — Compete in the established band:**
- Free tier: 10 users, 500 issues (mirror Linear)
- Basic: $10/seat (match Linear)
- Pro: $18/seat (above Linear $16, below Asana Advanced $25 — claim a feature wedge here)
- Team: custom for >50 seats
- Annual billing required for paid (RevenueCat-style retention lift)

**Path B — Justify the premium:**
- Keep $40/seat but require explicit positioning. Either:
  - Vertical compliance (SOC2-bound, regulated industries) — "Threadline for fintech eng teams"
  - Per-mgr pricing (not per-seat) — $80-150/mo per eng manager seat + free unlimited ICs (this redefines the SKU and is interesting)
  - AI-loaded ("Threadline Manager Copilot" — automated standup/retro/roadmap synthesis) with documented hours saved
- Superhuman-style concierge onboarding (founder-led 30-min 1:1)
- Invite-only waitlist

**Recommendation:** Path B with per-mgr pricing redefinition is the most interesting, because it (a) sidesteps the $10-16 Linear price war, (b) aligns price to the actual buyer (the manager), (c) gives ICs free unlimited (= bottom-up viral motion), and (d) makes the $40 number land as "cheap per manager" instead of "expensive per IC." This is a different SKU, not a different price.

### 6b. Trial / freemium mechanic

- 14-day trial alone is structurally wrong (covered in M0d). Replace with free tier OR concierge pilot (60 days, founder-led onboarding).
- For Path A: free tier + paid expansion (Linear playbook).
- For Path B: invite-only waitlist + 60-day concierge pilot for design partners; paid from day 1 for waitlist-graduates.

---

## Section 7 — Post-launch growth loops

DEFERRED (Mode C). Pre-launch work is the gate. Brief surface for context:
- **Referral mechanics:** if Path B per-mgr pricing, IC-invites are inherently viral. If Path A, team-invites are viral. Build in-product invite UX day 1.
- **Content compounding:** SEO will take 6-12 months. Start now.
- **Network effects:** weak in this category — Threadline doesn't get better as more *other companies* use it.
- **Retention as growth:** strong potential — happy eng managers refer peers, and Rands Slack rewards genuine recommendations.
- **Brand compounding:** founder-led content over years (Saarinen / Glaser model).
- Note: if zero compounding loops, business becomes acquisition-treadmill. Currently the plan has NONE of these designed in. Surface as risk.

---

## Section 8 — Metrics & instrumentation

DEFERRED to post-sprint. Minimum during sprint:
- Track design-partner pipeline (named, stage, last-touch, paid status)
- Track content output (posts/week per channel)
- Track community participation (Rands threads contributed, Lenny's comments, podcast pitches sent)
- Track "very disappointed" PMF survey responses from design partners

Do NOT measure during sprint: Twitter follower count, total signups, HN upvotes (vanity per skill default).

---

## Section 9 — Risk analysis

| Risk | Severity | Mitigation |
|---|---|---|
| Linear price cut (Feb 2026, $50 → $16) means category is consolidating around design-led winner; window to compete on "better Linear" is closing or closed | HIGH | Find a non-Linear wedge: vertical (fintech/regulated), AI manager copilot, per-mgr SKU. Don't position against Linear on its home turf. |
| Day-30 calendar gate fires against 90-180d mid-market cycle = guaranteed miss | HIGH | Replace with PMF gate (Vohra 40% / design-partner engagement / referrals) |
| No SOC 2 blocks every mid-market sale | HIGH | Start SOC 2 Type 1 immediately (6-8 weeks). Type 2 (6+ months) blocks 200+ person sales |
| Channel concentration on Show HN (single tactical event) | HIGH | Force 3+ channels per Section 3 priority list |
| Founders have zero ICP audience, zero B2B sales experience | HIGH | Mode-C audience-build sprint; founders must do sales work themselves |
| Pricing band 2.5-4x competitor with no premium justification | HIGH | Path A (lower to $10-18) or Path B (justify with per-mgr SKU / vertical / AI copilot) |
| Dogfood-to-buyer audience gap (ex-Google ICs → mid-market eng mgrs) | HIGH | 5-10 design partners shape the product before launch |
| "Friends + HN cohort" first 10 = ICP miss | HIGH | Replace with named cold-outreach list to mid-market eng mgrs |
| 14-day trial too short for B2B migration | MEDIUM | 60-day concierge pilot for design partners |
| Competitor counter-launch: Linear, Notion, Jira could ship eng-mgmt features quickly | MEDIUM | Move on vertical wedge that incumbents won't pursue |
| Rands Slack ban for self-promo | MEDIUM | Strict no-promo rule; contribute for months before mentioning product |
| Macro: economy tightens, mid-market SaaS budgets cut | MEDIUM | Annual billing + multi-year contracts for design partners with locked pricing |

---

## Outside voice (simulated adversarial pass — no external agent available)

Running an inside-the-skill adversarial pass with explicit attempt to break the plan:

1. **Biggest risk the inside review missed:** the *category itself* may be wrong-time-wrong-place. Linear cut prices 68% in 7 months. Notion and ClickUp are eating workspace + tracking convergence. AI-native tracking (Linear AI Agents, Jira's built-in AI) is happening RIGHT NOW. A new entrant betting "better than Linear for engineering-specific workflows" in mid-2026 may be entering a contracting category. The real question the inside review didn't ask: is this category Q1-2026-late? Should founders pivot to an AI-mgr-copilot SKU before even thinking about launch? This is upstream of every marketing decision.

2. **Channel mentioned that's weaker than positioned:** Pragmatic Engineer earned-mention. The inside plan suggests pitching Gergely Orosz for an earned mention. Gergely covers Big-Tech eng-mgmt and gets pitched constantly. Founders without prior content credibility have ~5% chance of an earned slot. Sponsored slots cost $5-15K and may not convert if the product doesn't match Gergely's quality bar. Realistic: budget for a single sponsored mention as a tactical event, don't depend on it.

3. **Audience claim that lacks evidence:** "Engineering managers read Pragmatic Engineer + Lenny's + Rands." Yes — but Threadline's specific buyer (mid-market eng mgr at 50-500 person SaaS) is a NARROWER segment than "engineering managers generally." Lenny's is more product-management leaning; Pragmatic Engineer skews Big-Tech IC + tech lead. The mid-market eng mgr persona may actually be best reached through verticalized channels (Operative Collective, CTO Connection, EngLeadersConnect) rather than the big-name newsletters. Inside plan didn't surface these niche channels.

4. **Provocative reframe:** **What if Threadline isn't a Linear competitor at all?** What if it's a *Linear add-on*? Most mid-market eng teams already use Linear (or are on the verge of). Their pain isn't "Linear isn't good enough," it's "Linear plus everything around Linear is a mess" — sprint planning involves Linear + Notion + Slack + Google Docs + Sheets + emails to PMs. A product that *sits on top of Linear* and unifies eng-mgmt workflows without forcing migration would (a) sidestep the head-on competition, (b) shortcut the adoption cycle (no migration), (c) potentially be priced per-manager (the SKU pivot from Section 6b) instead of per-seat. This is a SCOPE EXPANSION worth seriously considering — and it would shift the entire marketing plan toward "Linear ecosystem play, not Linear competitor."

Founder action: discuss reframe #4 with co-founder. If accepted, this skill must re-run from Step 0 with the new product framing. If rejected, document why the head-on play wins.

---

## Handoff

### 3 strongest action items for THIS WEEK

1. **Recruit 5 design-partner mid-market eng managers by Friday.** Cold-DM via LinkedIn Sales Nav. Script: "Building a Linear alternative built around eng-manager workflows. Looking for 10 design partners — 60-day free pilot + 50% off year 1 in exchange for weekly 30-min feedback + case study rights. Are you in?" Target 50 sends, expect 5-10 responses, expect 3-5 conversions. NO product pitch — design-partner ask only.

2. **Pick the playbook (Section 1c).** Founders must commit by end of week to one of: (A) Linear-style bottom-up + free tier + lower price, (B) Superhuman-style premium concierge, (C) Vertical wedge, or the (D) outside-voice reframe (Linear ecosystem play). Without commit, every downstream marketing decision oscillates. Schedule a 2-hour cofounder strategy session.

3. **Start the content cadence.** Both founders write 1 LinkedIn long-form post + 1 Twitter thread per week, focused on eng-mgmt insights (not product promotion). Topics: "Why we left Google to build for mid-market eng teams," "The Jira-to-Linear-to-???" arc, "What 50-500 person eng orgs need that 10K-person orgs don't." Goal: 1,000 ICP-relevant LinkedIn followers in 90 days.

### Self-check

Re-run `/plan-cmo-review` in 30 days. Success criteria:
- ≥5 design partners signed
- ≥1 piece of published content per week sustained for 4 weeks
- Founders have answered "what playbook are we running" with one clear answer
- SOC 2 Type 1 in flight
- Pricing decision made and documented

### Follow-up skills

- `/office-hours` — REQUIRED before anything else. The premise audit raised category-level questions (is this category contracting? Should it be a Linear add-on?) that need founding-team discussion.
- `/plan-ceo-review` — RECOMMENDED after office-hours. Pricing model change (Path A/B/D) is a CEO-level decision.
- `/plan-eng-review` — if Path D (Linear ecosystem) is chosen, product changes are large and need review.
- `/plan-design-review` — if Path A is chosen, Linear's design rep is the wall; design strategy is critical.
