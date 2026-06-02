# Marketing Plan — Threadline

**Product:** Threadline — Linear-style project tracking tool for engineering teams at 50-500 person companies
**Pricing claim:** $40/seat/month, no free tier, 14-day trial
**Founders:** 2 ex-Google engineers, no prior B2B sales experience
**Stated audience surface:** 200 X followers, ~50-person personal email list, no professional content history
**Stated validation gate:** 5 paying companies by day 30
**Stated distribution plan:** "Show HN at launch + content marketing on the engineering management blog"
**Stated differentiation:** "Better than Linear for engineering-specific workflows"
**Review date:** 2026-06-01
**Skill version:** plan-cmo-review v0.3.0
**Run mode:** **Mode A with Section 4 elevated** (Mode A vs C tie-breaker: mid-build B2B SaaS with hard 30-day validation gate AND <500 ICP-aligned audience → Mode A with elevated Section 4 over Mode C alone)

---

## TL;DR FOR THE FOUNDERS

You are technical-strong, marketing-naive. Step 0.5 finds **5 of 5 premises fail**: launch platform is wrong audience class for the actual buyer, no canonical-success comparable was used, the in-scope feature list contains at least two anti-features for the segment that will pay you, the 14-day no-friction trial selects against the time-poor engineering managers who actually convert, and the dogfood/buyer mismatch is severe (you are IC engineers building for engineering managers).

**The plan you wrote will ship to silence.** Reasons:
1. "Show HN + the engineering management blog" is one viable channel and one fantasy channel (you don't run an engineering management blog; you have 200 followers and ~50 emails).
2. "Better than Linear" is not a wedge — Linear is the canonical success in the category, has hundreds of thousands of dollars of brand momentum, $100M+ ARR with $35K total marketing spend, and a customer page that reads as a who's-who. You are not going to outpolish them. You need a wedge against the segment Linear actively under-serves, not "better than Linear."
3. The 30-day "5 paying companies" gate is calendar-driven for a retention-driven SaaS at a price band where ELT approval cycles routinely run 30-90 days. The gate is mis-specified.

Read on; the prescriptions are concrete.

---

## Step 0 — Pre-review audit

### Existing context

Design doc provided in the founder prompt is the entire artifact. There is no separate ICP doc, no landing page evidence, no content history, no waitlist artifact, no prior planning session output.

### Founder audience audit (numeric)

| Surface | Count | ICP-aligned? | Effective audience |
|---|---|---|---|
| X (Twitter) followers | 200 | Unknown — assume largely fellow ex-Google engineers; unclear how many are EMs at 50-500 person SaaS companies | Likely <50 ICP-aligned |
| Personal email list | ~50 | Personal contacts; some may be engineers/EMs at target companies | Likely <20 ICP-aligned |
| Professional content history | None | n/a | 0 |
| LinkedIn following | Not stated; assume modest | Unknown | Unknown, probably <500 ICP-aligned |
| GitHub stars on prior projects | Not stated; assume modest from ex-Google work | Unknown — Google-internal work doesn't transfer; OSS contributions might | Unknown, probably negligible |
| Prior shipped B2B products | None (no prior B2B experience) | n/a | 0 |

**Effective ICP-aligned audience: <100, and that's generous.** Pre-launch audience is essentially zero relative to the goal (sell $40/seat to engineering teams of 50-500). This is a load-bearing finding.

### Activation rule applied

- Mid-build (implicit; "Show HN at launch" implies build-then-launch)
- Hard launch implied by "5 paying companies by day 30"
- Audience: <500 ICP-aligned

**Tie-breaker rule from SKILL.md fires explicitly:** mid-build + hard launch gate + small/misaligned audience → **Mode A with Section 4 elevated**, NOT Mode C alone, because Mode C would skip the launch playbook the founder still needs to ship in ~30 days.

### Web-search competitive landscape (Step 0 pass — full landscape in Section 1)

Top direct competitors in modern engineering project tracking:
- **Linear** — $10-16/user/month, free tier with 250-issue cap and unlimited members, $100M+ ARR, $400M+ valuation, customer page that reads as "Vercel, Ramp, Cash App, OpenAI, Anthropic, Mercury, Retool…", grew via Twitter-led waitlist (10k signups), founder credibility, polish-as-marketing, ~$35K total marketing spend reported to reach $100M ARR. [Linear pricing](https://linear.app/), [GrowthHunt case study](https://www.growthhunt.ai/growth-story/linear), [Eleken case study](https://www.eleken.co/blog-posts/linear-app-case-study)
- **Jira** — Atlassian's incumbent, 300k+ organizations, 24 years old, 6,000+ marketplace apps, 15% Data Center price increase in Feb 2026.
- **Shortcut** — modern Linear alternative for mixed product+engineering teams that need configurable workflows + integrated docs.
- **Plane** — open-source self-host alternative, gaining traction with teams who want to avoid per-seat pricing at scale.
- **Height** — AI-native issue tracker, "Height can suggest subtasks, auto-assign, surface blockers before standup."
- **Tegon** — open-source Jira/Linear alternative, AI-driven, did a Show HN.

**The category is crowded with well-funded, design-led incumbents AND a fresh wave of OSS + AI-native challengers. "Better than Linear" is not a position; it's an aspiration.**

---

## Step 0.5 — PREMISE-LEVEL FINDINGS BLOCK

> **This block is the highest-value output of this review. Five of five premises fail. Tactical sections below inherit these findings.**

### Premise extraction

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis pre-test) |
|---|---|---|---|
| P1 | Launch platform: "Show HN" | Distribution plan | HN is right audience for some dev tools but the BUYER for $40/seat/mo at 50-500 person SaaS companies is the engineering MANAGER, often with VP/Director sign-off — not the IC who upvotes on HN |
| P2 | Audience class: "engineering managers, tech leads, IC engineers" lumped together | Target users | These are three distinct buyer personas with different attention surfaces. ICs read HN, EMs read Pragmatic Engineer + LeadDev, VPs read Lenny's + go to events. Lumping them flattens the targeting |
| P3 | Pricing point: $40/seat/month, no free tier | Pricing | Linear is $10-16/seat. $40/seat is 3-4x Linear. Without a documented differentiation that justifies a 3-4x premium against an entrenched category leader, this is anchored on nothing |
| P4 | "Friends + HN cohort" for first 10 customers | First-10 plan | "Friends" of ex-Google engineers may be Googlers. Google does not use Linear-class tooling and the friends are not the buyer. HN cohort is upvotes, not POs |
| P5 | Validation gate: 5 paying companies by day 30 | Validation gate | B2B mid-market companies have procurement cycles. SOC2/legal review for new vendor adds 2-6 weeks. 30 days is calendar-driven, not signal-driven |
| P6 | Differentiation: "Better than Linear for engineering-specific workflows" | Differentiation | Linear IS the engineering-specific tool. "Better than Linear at being Linear" is positioning vapor |
| P7 | Dogfood mix: implicit (2 ex-Google engineers dogfooding on themselves) | Implicit in founder description | Google engineers do not use Linear (internal tooling), do not write POs, and are not the EM/VP buyer persona. The dogfood audience does not match the paying ICP |

### M0a — Launch-platform audience-class fit

**Question:** Is Show HN the right audience class for a $40/seat B2B SaaS bought by engineering managers?

**Web-search evidence:** Tegon (open-source Linear/Jira alternative) did a Show HN — typical traction pattern for dev-tool style launches is variable (Linear-class incumbents' Show HN posts get modest engagement compared to launch-day Pragmatic Engineer features or Lenny's coverage). Linear itself did NOT launch via Show HN — it launched via a Medium article + founder Twitter + closed waitlist + Sequoia partner introduction. [Linear case study](https://www.eleken.co/blog-posts/linear-app-case-study), [Tegon Show HN](https://news.ycombinator.com/item?id=40912920)

**Audience-class match analysis:**
- HN audience: ICs and tech leads, founders, hobbyists, infrastructure people. EMs are present but in the minority and rarely the buyer for new vendor evaluation.
- Threadline buyer: EM, Director of Engineering, or VP Eng at a 50-500 person SaaS who has budget authority for $40/seat. This buyer reads Pragmatic Engineer, LeadDev, Lenny's, attends LeadDev / SREcon / StaffPlus, and lurks Rands Leadership Slack (30k members).
- ICs may *recommend* Threadline up the chain, but the IC-bottom-up path is the LINEAR playbook and Linear has dominated it. Trying to repeat Linear's playbook against Linear is not viable.

**Verdict: PREMISE FAILS.** Show HN is wrong audience class for the *buyer*. It is the *ICs* audience class, which is the recommender, not the buyer, and is also Linear's stronghold. The plan should either (a) lead with EM-targeted publications and events (Pragmatic Engineer, LeadDev, Rands), or (b) abandon the bottom-up-via-IC motion and commit to a top-down sales motion with cold outreach to EMs/Directors.

**Cascading implications:** M2 discovery path cannot start with "they see my Show HN post." Section 3 channel ranking must demote HN to recommender-channel status. Section 5 launch playbook needs an EM-targeted entry channel.

### M0b — Canonical-success comparable

**Question:** What's the canonical success at this motion class — vertical-specific B2B SaaS displacing a category leader?

**Web-search evidence:**
- **Linear itself** — the canonical success at this motion class. Documented playbook: build-in-public on Twitter, founder Twitter following → 10k waitlist signups → handpicked weekly invites of ~10 → closed Slack community for feedback → expanded launches at funding milestones → polish-as-marketing → no paid acquisition; reached $100M ARR with ~$35K total marketing spend. [GrowthHunt](https://www.growthhunt.ai/growth-story/linear), [Pragmatic Engineer interview with CTO](https://newsletter.pragmaticengineer.com/p/linear).
- **Pragmatic Engineer + Lenny's-class newsletter ecosystem** — for B2B engineering tools sold to EMs, sponsorship/feature in these newsletters is the equivalent of "content-led SaaS" channel that Ahrefs / ConvertKit ran for marketers. Pragmatic Engineer specifically refuses sponsorships, but the *podcast* takes limited long-term sponsors. Lenny's Newsletter does take sponsorships at premium CPM rates. [Pragmatic Engineer about](https://newsletter.pragmaticengineer.com/about), [Pragmatic Engineer ethics on sponsorship](https://blog.pragmaticengineer.com/sponsor/), [Pragmatic Engineer podcast sponsorship](https://blog.pragmaticengineer.com/podcast-sponsorship/).
- **Vertical wedge precedent:** Shortcut won the "mixed product+eng teams" wedge against Linear by not trying to out-Linear Linear. Plane won the "self-host / OSS" wedge. Height won the "AI-native" wedge. **Notice the pattern: each successful Linear-adjacent product picked a wedge Linear deliberately does not serve, not a head-on "better Linear" claim.**

**Deltas vs current plan:**
| Canonical | Did | Threadline plan does NOT |
|---|---|---|
| Linear (2019) | Built audience on Twitter for 12-18 months BEFORE launch | Plans to launch with 200 followers |
| Linear | Waitlist-gated, handpicked first 10/week | Plans to "Show HN" — broad, ungated |
| Linear | Founder credibility (designer at Airbnb, ex-Coinbase) was the trust anchor | Founders are "ex-Google engineers" — true, but Google-engineering credibility does not transfer to "I understand 50-500 person SaaS engineering workflow" |
| Linear | Found a wedge: "anti-agile, design-led, fast" | Threadline wedge is "better Linear" which is not a wedge |
| Shortcut/Plane/Height | Picked a Linear-NOT-serving segment | Threadline targets Linear's exact ICP |

**Verdict: PREMISE FAILS.** Canonical success was not consulted. The plan is implicitly imitating Linear at a stage where Linear has already won the position. The plan needs a wedge Linear deliberately does not serve.

**Possible wedges** (founder must pick): regulated industries (FedRAMP, HIPAA), self-host, AI-native triage (Height-adjacent), incident-management-integrated (Datadog/PagerDuty-style), engineering-finance integrated (resource allocation + headcount), or a specific company-size band Linear is admittedly weak at (Linear themselves acknowledge weakness above ~100-200 engineers per Pragmatic Engineer interviews; the 200-500 band may be a real underserved segment).

### M0c — Anti-feature surface

**Question:** Are any in-scope features anti-features for the paying ICP?

The design doc gives one-liner features (Linear-style), so this is partial. From the founder's framing:

**Candidate anti-features:**
- **No free tier + 14-day trial:** the 14-day trial structure is itself anti-feature for the EM/Director buyer at 50-500 person companies. These buyers don't trial-shop; they evaluate via vendor calls, security review, then pilot. A 14-day clock running on procurement is hostile to the buyer.
- **"Linear-style" implies the same speed/polish bar Linear hit:** matching Linear's polish bar requires Linear-class engineering investment in the IDE-ish front-end. Two ex-Google engineers can do this, but the cost (engineering hours per shipped polish unit) competes against time available for cold-outreach and sales. This is an indirect anti-feature: it commits the founders to a build burn-rate that crowds out the sales work the GTM needs.
- **Trying to serve EMs + tech leads + ICs in one product:** product surface that satisfies all three audiences fragments the value prop. Linear's wedge was specifically "design-led, opinionated, IC-favoring" — Threadline trying to additionally please EMs at the same surface is product-strategy split.

**Verdict: PREMISE FAILS** (at least 2 anti-features under marketing-naive default; can be tightened with founder input on the full feature list).

**Owed decision:** kill, defer, or enterprise-tier each anti-feature candidate. Specifically reconsider 14-day no-CC trial → consider concierge-onboarded pilot instead (see M0d).

### M0d — Freebie-disqualifier / acquisition-mechanic selection bias

**Question:** Does the 14-day trial select for the wrong segment relative to the paying ICP?

**Diagnostic:** map mechanic → segment attracted.
- "14-day free trial" attracts: time-rich evaluators, indie devs, side-project users, small teams that may not have budget at all.
- "Paying ICP" for $40/seat × 50-500 engineers = $24K-240K ARR contracts. Buyer: EM with budget approval or Director/VP. Time-poor, money-rich, trust-led.

**Mismatch:** the 14-day trial attracts time-rich evaluators. The buyer is time-poor and won't kick the tires personally. A trial without a paired sales motion is an artifact for the wrong segment.

**Web-search evidence on B2B mid-market dynamics:** Per the B2B SaaS pricing research, B2B engineering tool buyers care about ROI, longer sales cycles, multiple stakeholders, willingness to pay value-priced. Flat-rate self-serve compresses cycle for SMB; mid-market wants vendor calls, security review, executive sponsorship. [B2B SaaS pricing guide](https://softwarepricing.com/blog/saas-pricing-models/)

**Verdict: PREMISE FAILS.** The 14-day trial is validation theater for the wrong segment. A pilot/POC structure (named champion, scoped 30-day evaluation with founder onboarding) is the correct mechanic for the stated ICP.

**Owed prescription:** replace "14-day trial" with "concierge pilot": 30 days, founder personally onboards, named success metric agreed upfront, $X/seat after pilot with annual commit. This is the Superhuman / Linear-early-days playbook.

### M0e — Dogfood / buyer audience-class match

**Question:** Do the founders dogfood on the same audience class that will pay?

**Setup:** 2 ex-Google ICs building for EMs at 50-500 person SaaS companies.

**Mismatch analysis:**
- Google ICs work in a 100,000+ engineer org with Google-internal tooling (Critique, Buganizer, Piper, etc.). The workflow, the org-shape, the procurement reality, and the day-shape are all different from a 50-500 person SaaS EM.
- Google ICs do not write POs, do not approve vendors, do not have budget authority for $40/seat across a team.
- "Engineering-specific workflows" as Google ICs experienced them are NOT the workflows the buyer (EM at a Series B-C SaaS) faces.

**Severity: HIGH.** This is exactly the failure mode M0e warns about. The dogfood is two ex-Google ICs; the buyer is a Series-B-C engineering manager. Different worlds.

**Verdict: PREMISE FAILS.**

**Prescription (BOTH PIVOTS, per v0.3.0 strengthened M0e):**
1. **Pivot the target audience in marketing materials, ICP doc, and launch sequencing** to engineering managers / Directors at the 50-500 person band specifically. Not "engineers." The buyer.
2. **Expand dogfood subjects to include 5-10 EMs at the target band BEFORE any public launch.** Find them through warm intros (X network from 200 followers + 50 emails — start there; LinkedIn cold-outreach to specific named EMs at named target companies). 1-2 weeks of buyer-aligned dogfood minimum before any launch decision.

The wrong fix (which would now trip the v0.3.0 anti-pattern #14) would be: "We'll defer the EM audience until v1.0.5 and ship for ICs first." That preserves the mismatch.

### Step 0.5 cascading findings — summary

| Premise | Verdict | Section it cascades into |
|---|---|---|
| P1 launch platform | FAILS | Section 3 (channel scoring), Section 5 (launch sequence) |
| P2 audience class lumping | FAILS | Section 2 (ICP), Section 3 |
| P3 pricing | FAILS at justification level | Section 6 |
| P4 first-10 path | FAILS | Section 5 |
| P5 validation gate | FAILS | Section 5 (launch gate) |
| P6 differentiation | FAILS | Section 1 (positioning), Section 2 (ICP) |
| P7 dogfood mismatch | FAILS | Section 2, Section 4 |

**5 of 5 M0a-M0e premises fail.** This triggers the PREMISE-LEVEL FINDINGS BLOCK requirement (already placed at the top of this document above the TL;DR).

---

## Step 0A — Forcing questions (simulated honest-naive founder answers, then refused/accepted)

Founders are simulated as B2B-naive ex-Google engineers per the prompt. I am answering as them with the honest-naive plausible answer, then the skill refuses or accepts.

### M1 — Audience reality

**Naive founder answer:** "Engineering managers at series B-D SaaS companies who hate Jira."

**Refused.** Demographic category. Refused per skill rule.

**Forced-specific answer the skill demands they produce:** A named composite — *"Priya, Director of Engineering at a 220-person Series C fintech SaaS in NYC. She came up through Stripe, Brex, or similar. Reads Pragmatic Engineer (paid). Listens to LeadDev podcast and Software Engineering Daily. Active in Rands Leadership Slack. Attends one LeadDev event per year. Currently uses Linear for two teams and Jira for two teams (legacy contract). Pain: she spends 4-6 hours/week chasing status across the two systems, and quarterly planning is a manual aggregation hell. She'd switch if a single tool covered both groups without forcing the Jira-locked team to migrate their 4-year history."*

**Attention surfaces (≥3 named):** Pragmatic Engineer newsletter & podcast; LeadDev Slack + conferences; Rands Leadership Slack (30k members); Lenny's Newsletter (some EM content); Software Engineering Daily podcast.

**Status: ACCEPTED** (with the warning that the founders must validate this composite by talking to 5+ actual Priyas, since they have not yet — they are dogfooding on themselves who are not Priya).

### M2 — Discovery path

**Naive founder answer:** "She sees our Show HN post and clicks through."

**Refused.** Per skill rule, Show HN cannot be step 1. Also Priya does not read HN.

**Forced answer:**
1. Priya reads a Pragmatic Engineer post or guest post on "engineering project tracking patterns at 200-engineer companies" (founder-written, takes 6-8 weeks to land).
2. The post mentions Threadline as a contributing tool / case study (NOT a paid placement — Pragmatic Engineer refuses sponsorships, but does accept high-quality guest contributions and does cover named tools in editorial features).
3. OR Priya hears Threadline mentioned in Rands Slack by another Director discussing the cross-tool aggregation problem, sees Threadline named.
4. Priya visits the Threadline landing page, sees specific positioning ("for the 100-500 engineer band Linear admits it's weaker for; native Jira migration without forcing the legacy team to abandon ticket history").
5. Priya books a 20-minute call with a founder (concierge pilot, not free trial).
6. Founder personally onboards her two teams over 2 weeks.
7. Pilot converts to annual contract at ~$40/seat after a 30-day evaluation.

**Status: ACCEPTED** with the caveat that this path is currently aspirational — founders have not yet written for Pragmatic Engineer, are not yet in Rands, and have no landing page. Each step has a real prerequisite they must build.

### M3 — Pre-launch audience

**Naive founder answer:** "200 X followers, ~50-person email list."

**Acknowledged numbers per prompt.** Per skill rule, the honest "<500 ICP-aligned" answer triggers Audience-Build Sprint mode considerations — handled via Mode A with Section 4 elevated per tie-breaker rule.

**Status: ACCEPTED as a fact. The fact is small. Section 4 carries the load.**

### M4 — Channel honesty

**Naive founder answer:** "We're good at building. We can post on Twitter."

**Refused** (per rule: "I can build it" is product not distribution; "I know how to use Twitter" without followers is not a channel advantage).

**Forced answer:** "We don't have a demonstrable distribution advantage. Our ex-Google background may give us warm intros to a small number of EMs at Google-alumni-founded companies (Stripe, Notion, Vercel, etc.), if we work our network actively. That's a referral surface, not a content channel. Our only credible non-trivial channel is **direct outreach to a list of named EMs** — labor-intensive, slow, but actually fits a 200-follower team."

**Status: ACCEPTED.** The skill notes: no-credible-channel becomes the FIRST work item, not a future-tense aspiration.

### M5 — Competitor traffic source

**Naive founder answer:** "Probably Google? Maybe HN?"

**Refused.** Guess not verified.

**Forced research result (done via this skill's WebSearch):**
- **Linear:** brand search, direct, referral from customer/founder Twitter, no paid acquisition reported. ~$35K total marketing spend to $100M ARR. Channel: Twitter (founder), waitlist, customer-logo flywheel. Show HN was not the launch surface.
- **Shortcut:** content marketing (Shortcut blog, "the modern alternative" positioning), product-led free tier, integrations marketplace as recommender surface.
- **Jira/Atlassian:** SEO + brand + enterprise sales (different motion entirely).
- **Plane:** GitHub (OSS distribution, ~30k+ stars), HN multiple Show HNs, dev-Twitter.
- **Height:** AI-native angle gets press coverage; Product Hunt featured.

**Pattern:** None of the modern winners used Show HN as a primary channel. Linear's Twitter-driven waitlist + handpicked invite-only beta is the most relevant precedent.

**Status: ACCEPTED.** Founders are not flying blind anymore; the data is in.

### M6 — First 10 paying customers

**Naive founder answer:** "Friends + HN cohort."

**Refused.** "Friends" of ex-Googlers are likely Googlers (Google doesn't buy Linear-class tools). HN cohort is upvotes, not contracts.

**Forced answer:** The founders need a **named list of 30-50 specific EMs at specific 50-500-person SaaS companies** they can email tomorrow. Concrete approach:
- Mine the ex-Google diaspora for EMs (LinkedIn search: "engineering manager" + "ex-Google" + company size 50-500).
- Mine ex-Google founders' alumni companies (Stripe, Notion, Figma alumni networks).
- Filter for companies that publicly mention frustration with Linear OR Jira (search engineering blogs, conference talks).
- First 10 paying customers = 5 from warm-intro / founder network + 5 from cold outreach with strong specificity.

**Acceptable concrete plan:** "We will build a list of 50 named EMs by end of week 1, contact 10/week with personal emails, target 1 pilot from every 10 (10% reply × 50% pilot conversion ≈ 1 pilot/10 emails)."

**Status: ACCEPTED** if the founders commit to producing the named-50 list this week.

### M7 — Time allocation

**Naive founder answer:** "We've been spending ~90% on build."

**Refused.** Per skill rule, <30% on audience-building flips the ratio wrong.

**Forced answer:** The founders must shift to ≥40% on audience-building immediately. Concrete cadence: 1 founder spends 20+ hours/week on writing (1 long-form essay/week, podcast pitches, Rands Slack presence, cold outreach), other founder continues build but pauses non-critical polish work for the next 60 days. **The product is already in the "Linear can do this too" parity band; more polish does not change the win/lose. Audience build does.**

**Status: ACCEPTED** with explicit acknowledgment that the founders may resist this (technical founders typically do).

---

## Step 0B — Mode lock

**Mode A with Section 4 elevated.** Locked.

Reason (per tie-breaker): mid-build + hard 30-day validation gate + <500 ICP-aligned audience. Mode C alone would skip the launch playbook. Mode A delivers both the launch playbook (Section 5) and the audience-build sprint (Section 4).

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Tool | Year | Pricing | Apparent traffic source | Public complaints | Positioning vs Threadline | Winning? Why? |
|---|---|---|---|---|---|---|
| **Linear** | 2019 | Free (250 issues) / $10 / $16 | Brand search, founder Twitter (Karri Saarinen 80k+), customer-logo flywheel, no paid | "Too opinionated for mixed teams," "weak at >100-200 engineers," "limited customization for non-eng teams" | Threadline is "Linear but for engineering specifically" — Linear is ALREADY that. Threadline is positioned ON TOP of Linear's exact ICP without a wedge | YES. $100M ARR, $35K marketing spend, customer page reads as who's-who. Cited: [GrowthHunt](https://www.growthhunt.ai/growth-story/linear) |
| **Jira** | 2002 | ~$8.15/user (Standard) → enterprise pricing | SEO, brand, enterprise sales | "Too configurable," "slow," "configuration hell" | Incumbent at the high end. Threadline could displace at the mid-band but only if the migration story is strong | DOMINANT (300k orgs) but losing share to Linear at the modern-eng end |
| **Shortcut** | 2014 (orig Clubhouse) | ~$10/user free up to 10 | Content marketing, product-led, integrations | "Less polished than Linear," "more configurable for mixed teams" | Already won the "mixed product+eng" wedge | Solidly positioned in a specific wedge |
| **Plane** | 2022 | OSS free, hosted ~$8/user | GitHub stars, HN Show HN posts, dev-Twitter | "Still maturing," "fewer integrations" | Won "self-host / OSS" wedge | Growing fast in a specific wedge |
| **Height** | 2020-ish | ~$8.50/user | Product Hunt, AI-native press coverage | "AI features still in beta," "less mature" | Won the "AI-native" wedge | Riding the AI wave |

### 1b. Canonical-success comparables (motion-class: developer-facing B2B SaaS displacing an incumbent)

| Canonical | Year | Price | Acquisition channel | Onboarding model | Launch gate | Delta vs Threadline plan |
|---|---|---|---|---|---|---|
| **Linear** | 2019 | $10-16/user | Founder Twitter → waitlist → handpicked invites; polish-as-marketing; customer flywheel | Self-serve with high polish; concierge for early cohort | Closed beta gated on quality feedback, not calendar | Threadline plans to launch on Show HN with no waitlist, no prior audience, no handpicked invites, and a calendar gate |
| **Stripe** | 2010 | Usage-based | Docs-as-marketing, developer relations, founder presence | Self-serve API, no sales until enterprise | PMF signal-driven via design partners | Threadline has no docs strategy, no DevRel, and no design partners |
| **Superhuman** | 2017 | $30/mo | Invite-only waitlist, two-sided referral, founder-led concierge onboarding (Vohra personally onboarded first 200) | Pure concierge | Vohra "very disappointed" ≥40% test | Threadline has no concierge plan and is calendar-gated |
| **Notion** | 2016 (relaunch) | $8-15/user | Community + creator-led + viral templates | Self-serve, freemium | Long PMF iteration before scaling | Threadline plans no community, no creator partnerships, no freemium loop |

### 1c. Pattern surface

**What canonical successes share that the current plan lacks:**
1. **Pre-existing founder audience** — Saarinen had a designer-and-Coinbase-era following; Patrick Collison had HN cred from prior projects; Vohra had Rapportive credibility. Threadline founders have 200 followers and no professional content track. **This is the load-bearing missing piece.**
2. **Waitlist-gated invite-only first cohort.** None of the canonical successes did "post on HN and hope." All did closed beta with handpicked early users.
3. **Founder-led concierge onboarding** for first 50-200 users. Even Linear, ostensibly self-serve, did handpicked invites of ~10/week.
4. **Wedge that the incumbent visibly does not serve.** Linear's wedge was "anti-Jira-configurability." Threadline's stated wedge is "better Linear at Linear's exact thing" — not a wedge.
5. **PMF-signal-driven launch gates,** not calendar.

**Where direct competitors diverge from canonical-success patterns:** Tegon (Show HN-led), several smaller Linear-alternatives — these are the ones that did NOT compound. They illustrate the failure mode the current plan is heading toward.

**Which pattern is the plan implicitly following?** A blend of "Show HN-led indie SaaS" (Tegon-class, low compound) + "content marketing" (no audience to leverage) — not the Linear / Stripe / Superhuman playbook the founders' ambition implies.

**Founder action items from Section 1:**
- Study Linear's first 18 months in detail. Read Karri Saarinen's posts and the Pragmatic Engineer Linear interview. Specifically copy: build-in-public cadence, waitlist mechanic, handpicked-invite cadence.
- Study Superhuman PMF engine. Vohra's First Round Review post on the very-disappointed test.
- Pick a wedge. Refuse to launch on "better Linear."

---

## Section 2 — ICP specification

Output: `icp.md` (separate artifact).

Headline: **Director of Engineering at a 100-500 person Series B-D SaaS, currently using Linear and/or Jira with cross-team aggregation pain, with budget authority for tooling decisions ≤$50/seat.**

Detail in artifact.

---

## Section 3 — Distribution channel-by-channel

### Channel scoring for THIS team (200 followers, no content history, B2B mid-market motion, EM buyer)

Scoring: 1=weak 5=strong for **THIS team specifically.**

| Channel | Reach | Cost | Conversion | Founder fit | Effort | Leverage | Recommend? |
|---|---|---|---|---|---|---|---|
| Show HN | 4 | 1 (free) | 1 (wrong audience class for EM buyer) | 2 (technical comfort, no HN rep) | 1 | LOW | No, OR demote to recommender-channel only |
| Pragmatic Engineer (sponsorship) | 5 | n/a — no sponsorships accepted | n/a | n/a | n/a | n/a | NOT AVAILABLE |
| Pragmatic Engineer (podcast sponsorship) | 4 | High ($X K per slot, long-term only) | 4 (right audience class exactly) | 4 (if money allows) | 2 | **HIGH** | YES if budget exists |
| Pragmatic Engineer (guest writing) | 4 | Time only | 4 | 2 (no track record yet — Orosz curates heavily) | 5 | MEDIUM-HIGH if accepted | TRY but assume 4-8 week pitch-to-publish, low acceptance probability |
| Lenny's Newsletter (sponsorship) | 5 | Premium CPM | 4 | 4 (if budget) | 2 | **HIGH** | YES if budget exists |
| Lenny's (guest post) | 4 | Time | 4 | 2 | 4 | MEDIUM-HIGH | TRY |
| LeadDev Slack | 3 | Free | 4 | 3 (need to build presence first) | 3 | **MEDIUM-HIGH** | YES |
| LeadDev events (sponsor / speak) | 4 | Mid-high | 5 | 3 | 4 | **HIGH** | YES — pick next LeadDev conf and submit a talk |
| Rands Leadership Slack | 3 (30k members, but no-sell norm) | Free | 3 (community presence, NOT direct selling — risk of ban) | 2 (need to genuinely participate, not pitch) | 4 (sustained months of presence) | MEDIUM | YES with long horizon, no direct selling |
| Twitter/X organic | 2 (200 followers; need to grow) | Free | 2 (slow ramp) | 3 (technical founders can write threads) | 4 | LOW initially, MEDIUM if cadence sustained | YES — build-in-public for 90 days |
| LinkedIn organic | 3 (better for B2B EM audience than X) | Free | 3 | 3 | 3 | MEDIUM | YES — underused by technical founders, fits EM audience |
| Cold outreach (DM + email) | 4 (named lists) | Low | 4 (when targeted) | 4 (technical founders write credible technical emails) | 5 (labor-intensive) | **HIGH** | YES — THE primary channel for first 10 customers |
| SEO / content | 4 long-term | Free (time) | 3 | 3 | 5 (6-12 month ramp) | MEDIUM (long horizon) | YES for compounding, but not for 30-day gate |
| Podcast guesting (Software Engineering Daily, LeadDev, Engineering Enablement, Pragmatic Engineer Podcast) | 4 | Free | 4 | 3 (need angle to pitch) | 3 | **HIGH** | YES — pitch 10 podcasts in week 2 |
| Product Hunt | 3 | Free | 2 (PH audience is broader product/consumer, not EM-specific) | 3 | 3 | MEDIUM-LOW | OPTIONAL secondary channel |
| Reddit (r/ExperiencedDevs, r/cto, r/programming) | 3 | Free | 2 (self-promo gets banned) | 2 | 3 | LOW | NO direct posting; OPTIONAL participation if genuine |
| Paid ads (Google) | 3 | High ($20-50 CPC for EM keywords) | 2 (low intent at the keyword level) | 1 | 3 | LOW | NO for v1 |
| Affiliate / partnership | 2 | n/a | 2 | 1 | 4 | LOW | Premature |

### Surviving channels (ranked by leverage for THIS team)

1. **Cold outreach to named EM list** — primary engine for first 10 customers
2. **Podcast guesting** — pitch 10 in week 2-3
3. **LeadDev events / Slack + Rands Slack presence** — slow compound, start now
4. **LinkedIn organic (EM audience)** — fits buyer attention surface; technical founders rarely exploit
5. **Lenny's sponsorship OR guest post** — if budget allows or pitch lands
6. **Twitter/X build-in-public** — slow compound; mandatory for founder credibility surface
7. **SEO / content** — 6-12 month compound; start now for next-year traction

### Channels to demote / cut

- Show HN — demoted to "post once, ideally after a Pragmatic Engineer or LeadDev surface gives social proof to link in the HN post."
- "Engineering management blog" (founders' fantasy) — they don't run one, can't materialize a readership in 30 days. Replace with guest-post strategy.

### Motion-class rules applied

**B2B SaaS (mid-market):** Per skill rule, generic social channels are weak; specific vertical publications carry far higher conversion. Named the vertical publications: Pragmatic Engineer, Lenny's, LeadDev, Software Engineering Daily, Engineering Enablement Podcast, Rands Slack. These are PRIMARY, not auxiliary.

**Note: this is NOT a dev tool motion** — dev tool rules (GitHub-as-marketing, docs-as-marketing, anti-marketing tone) apply when the BUYER is a developer. The buyer here is the EM/Director. Some dev tool rules carry over (technical-honest tone in any IC-facing surface) but the GitHub-stars-as-social-proof rule is muted because EMs don't pick tools by GitHub star count. Founders should still publish a GitHub repo if they ever go OSS or want IC-credibility lever, but it's not the channel.

---

## Section 4 — Pre-launch audience-building plan (ELEVATED per Mode A tie-breaker)

This is the load-bearing section. Output: also written into `audience_build_journal.md`.

### Day 1-30 (audience-build week 1-4)

| Week | Cadence | Specific outputs | Channel |
|---|---|---|---|
| Week 1 | Build the named lists | 50 named EMs (LinkedIn) + 10 podcast targets + 5 newsletter targets + apply to Rands Slack with genuine intent letter | Lists, applications |
| Week 1 | 1 long-form essay | "What ex-Google ICs learned shipping for engineering teams that are NOT Google" (the meta-credibility frame: acknowledge the gap; show learning) | Personal blog + LinkedIn + X |
| Week 1 | 5 outreach emails | First 5 cold-outreach emails to EMs (personal, no pitch, ask for 20-min user interview) | Email |
| Week 2 | 10 outreach emails + 5 podcast pitches | Continue outreach; pitch SED, LeadDev podcast, Engineering Enablement, Dev Interrupted, The Pragmatic Engineer Podcast | Email |
| Week 2 | 1 essay | "Why the 100-500 engineer band is genuinely different from Linear's sweet spot" — the wedge essay | Blog + LinkedIn + X |
| Week 2 | LinkedIn cadence | 3 LinkedIn posts/week starting week 2 | LinkedIn |
| Week 3 | 10 outreach + interviews land | Conduct first 5 user interviews | Calls |
| Week 3 | 1 essay | "What 10 engineering directors actually said about cross-tool aggregation" (interview synthesis) | Blog + LinkedIn |
| Week 3 | Rands presence | Daily participation if accepted; answer questions, no pitch | Slack |
| Week 4 | 10 outreach | Convert 1-2 interviews to design-partner pilots | Email/calls |
| Week 4 | 1 essay + 1 Twitter thread | Build-in-public on the design-partner work | X + LinkedIn |

**By day 30 outputs:** 4 long-form essays published, 5-10 user interviews conducted, 1-2 design partners committed to pilot, 40-50 named cold-outreach emails sent, 5-10 podcast pitches sent (1-2 booked).

**NOT a launch by day 30.** The "5 paying companies by day 30" gate is replaced (see Section 5) with "5 design partners in pilot by day 60, 5 paying by day 90" — see Section 5 for the gate redesign.

### Day 31-60

- Pilot delivery (founder-led concierge onboarding for design partners)
- Continue essay cadence (1/week)
- Podcast appearances start landing (recorded → published lag is 2-4 weeks)
- Apply to speak at next LeadDev conference (typically 3-6 months ahead booking)
- Pitch 1 guest post to Lenny's Newsletter and 1 to Pragmatic Engineer (low acceptance probability; pitch anyway)

### Day 61-90

- Convert design-partner pilots → paying contracts (Vohra-style: gate the broader launch on ≥40% "very disappointed" from pilot users, not calendar)
- Build the "we have N paying customers, here's the data" launch artifact
- Sequenced launch (Section 5) once the PMF signal is met

### Refused alternatives

- "We'll start posting more on Twitter" — vague; refused.
- "We'll just keep building until launch" — explicitly rejected; ratio wrong.

---

## Section 5 — Launch playbook

### 5a. Launch-gate question

**Question:** Calendar (day N) or PMF signal?

**Founder's stated gate:** Calendar — "5 paying companies by day 30."

**Verdict: WRONG GATE.** This is retention-driven B2B SaaS at a price band that triggers procurement review (legal + security + budget) in most 50-500 person SaaS companies. Procurement cycles routinely run 30-90 days. Even if Threadline is product-perfect on day 30, paying-company-by-day-30 is gated by buyer-side procurement, not seller-side launch readiness.

**Replacement gate:** **Vohra-style PMF + concierge-pilot signal.**
- **Gate 1 (day 30):** 5 design partners committed to pilot, founder-onboarded, NOT yet paying.
- **Gate 2 (day 60):** ≥3 design partners report ≥40% of their team would be "very disappointed" if they lost Threadline. Founder personally interviewed each.
- **Gate 3 (day 90):** 3+ pilots converted to paid annual contracts. THIS is when the public sequenced launch fires.

If gate 2 fails, the product is not ready for public launch regardless of calendar. Keep iterating with design partners.

If the founders defend the calendar gate, they must explain why their retention-driven SaaS is an exception to the Vohra/Superhuman precedent. Acceptable reasons: explicit time-bounded event (e.g., they have runway concerns and must show MRR to investors by day 90 — but that's a runway gate, not a marketing gate, and it argues for a longer pre-launch raise, not a premature public launch).

### 5b. Sequenced launch playbook (fires AFTER PMF gate met, approximately day 90+)

| Time | Channel | Specific action |
|---|---|---|
| Day -60 to launch | Audience-build | Continued cadence per Section 4 |
| Day -30 | Design partner referrals | Ask each of the 3-5 paying design partners for 2 warm-intro EMs each → ~10 warm leads |
| Day -14 | Pre-announce | Personal email to ~100-person list (the original 50 + new connections from outreach) |
| Day -7 | Twitter thread + LinkedIn long-form | Build-in-public thread: "We have N paying customers. Here's what we learned. We're opening up." Include specific customer logos (with permission) |
| Day -7 | Podcast booking | Time at least 1 podcast appearance to drop within launch week |
| Day 0 morning | Pragmatic Engineer / Lenny's | If a guest post landed, time it for launch week |
| Day 0 morning | LinkedIn launch post | Long-form post by founder, EM-targeted, includes design partner quotes |
| Day 0 + 4h | Show HN | NOW post Show HN with social proof (named customers, paying contracts) — LinkedIn surface as the lede, HN as a secondary social-proof surface. HN audience is the recommender, not the buyer; positioning is "tool that N engineering teams now depend on," not "new tool, please try it." |
| Day 0 + 24h | LeadDev Slack | Post in #show-and-tell or relevant channel (compliant, not spam — present learnings, not pitch) |
| Day 0 + 48h | Rands Slack | Same — community-respectful share, after months of genuine participation |
| Day 0 + 7d | Product Hunt | Separate launch event (different audience, partly overlapping). Coordinated launch with hunter relationships secured in advance |
| Day 0 + 14d | Podcast cluster | Schedule 3-5 podcast appearances to drop in succession |
| Day 0 + 30d | Substack / blog retrospective | "What happened in our first 30 days post-launch" with traction numbers |

**Risk callouts:**
- HN miss = no recovery if it's the only channel. **No longer the only channel here.**
- LinkedIn algorithm shift = recovery via newsletter / podcast.
- Rands Slack ban for self-promo = real risk if founders pitch too directly. **Mitigation:** only post after months of genuine non-promotional participation.

### 5c. Tonal rules (motion-class adapted)

This is NOT a dev tool launch (buyer is EM, not IC), so the dev-tool anti-marketing tonal rule applies only on the IC-recommender surfaces (HN, r/programming if used). On those surfaces:
- Lead with technical specifics (architecture, named trade-offs, honest "Linear is better at X" comparisons)
- Code-first framing if any open-source component exists
- Cut superlatives entirely

On EM-facing surfaces (LinkedIn, LeadDev, Lenny's, podcasts):
- Lead with the BUYER's pain (cross-tool aggregation, quarterly planning) not the product features
- Include design-partner names + quotes (social proof is the load-bearing element for EM trust)
- Tone: peer-to-peer engineering leader, not vendor pitch

---

## Section 6 — Pricing & packaging

### 6a. Pricing-BAND question

**Question:** Did $40/seat inherit from competitor anchoring, ICP WTP evidence, or "felt right"?

**Inferred answer:** Felt right. The plan does not justify $40/seat against anything specific. Linear is $10-16. Jira is ~$8. $40 is 2.5-5x the category band.

**ICP-WTP evidence the founders need to gather:**
- Ask the 5+ user-interview EMs (Section 4): "What do you currently pay per seat for engineering tooling? What was the most expensive per-seat tool you've approved? What was the cheapest you rejected for quality reasons?"
- Look at adjacent tools EMs approve at higher per-seat: DataDog ($15-100+/host), PagerDuty ($21-39/user), Sentry ($26/user starts), Linear Business $16/user — the upper-band of accepted engineering tooling sits around $15-40, with infrastructure exceeding it.

**Verdict on the BAND:** $40/seat is at the very top of the accepted band for engineering-team-process tooling. NOT impossible — but requires a sharp differentiation story that justifies 3-4x Linear. The plan does not currently have that story. **The price is defensible only if the wedge is defensible.** With current "better Linear at Linear" positioning, $40/seat will not survive procurement.

**Two viable paths:**
1. **Reduce to $15-25/seat** to match the upper band of accepted engineering process tooling and remove the price objection from procurement.
2. **Keep $40/seat** and EARN it with a wedge so specific that the buyer accepts the premium (e.g., "Threadline replaces both Jira AND a separate planning tool, so net spend goes down for teams running both" OR "Threadline is the only tool with native FedRAMP / HIPAA at this price band, so it unblocks regulated SaaS").

The CURRENT plan does neither — $40 without the wedge — and is the worst case.

### 6b. Standard pricing coverage

| Element | Current plan | Recommendation |
|---|---|---|
| Free tier | None | Keep no free tier — appropriate for the trust-buy ICP per M0d. Don't backslide into freemium. |
| Trial | 14-day | **REPLACE with 30-day concierge pilot.** Founder-led onboarding. Named success metric agreed upfront. Concierge converts to annual contract or doesn't — no self-serve "trial." |
| Annual discount | Not stated | Mandatory. Annual billing dramatically improves retention. Default to annual contract for the buyer profile. Offer 15-20% annual discount only as a closing concession, not as a marketing-page price. |
| Pricing model | Per-seat | Per-seat is fine for this category. Watch for the seat-deflation risk (companies cap seats to control cost — common in tools that admins gate access to). Consider tiered plans (Starter / Pro / Business) so the unit doesn't have to scale linearly. |
| Tier structure | Not stated | Build 3 tiers: Starter (no SSO, basic), Pro (SSO, audit log, $40-ish/seat), Enterprise (SOC2 attestation, dedicated support, custom). The Pro tier is the headline price. |

---

## Section 7 — Post-launch growth loops

What compounds:
- **Customer-logo flywheel** (Linear's strongest loop): each enterprise customer becomes social proof for the next. Build a customer page from launch day. Get explicit logo-usage permission in pilot contracts.
- **Founder content compounding** (Pragmatic Engineer trajectory): essays compound over years. Start now.
- **Podcast appearances** compound — each appearance is replayed indefinitely.
- **In-product referral mechanic** — possible (engineering teams collaborate cross-company; "invite a peer EM" mechanic can work). Build in v1.1.

What's linear (does not compound):
- Cold outreach. Necessary for first 10, will not scale to 100.
- Paid ads (none recommended).

**Acquisition-treadmill risk:** if no compounding loop fires by month 6, the business is acquisition-treadmill. Surface as risk in Section 9.

---

## Section 8 — Metrics & instrumentation

### Measure

| Metric | Definition | Target | Frequency |
|---|---|---|---|
| Outreach reply rate | (Replies / cold emails sent) | ≥8-15% per industry benchmark | Weekly |
| Interview → pilot rate | (Pilots committed / interviews conducted) | ≥20% | Weekly |
| Pilot → paid rate | (Annual contracts signed / pilots completed) | ≥50% | Monthly |
| Vohra "very disappointed" | (Users answering "very disappointed" / total surveyed) | ≥40% (Superhuman bar) | Monthly during pilot |
| Day-30 retention (per pilot team) | (% of seats still active after 30 days) | ≥80% | Monthly |
| Time-to-first-value (TTFV) | (Time from invite to first ticket created) | <10 min for ICs | Per pilot |
| Founder content velocity | Essays / posts / podcast appearances per week | 1 essay/week, 3 LinkedIn/week | Weekly |

### Do NOT measure (vanity)

- X follower count
- HN upvotes
- Total signups (without retention)
- Newsletter open rates (without revenue correlation)

---

## Section 9 — Risk analysis

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| Linear ships the same feature in 3 months | HIGH | Could kill wedge entirely | Pick a wedge Linear has publicly said no to (e.g., specific regulated industry, specific company-size band Linear admits weakness in) |
| HN launch flops | MEDIUM | LOW if HN is no longer the primary channel | Demote HN to recommender surface as recommended; founder-content + cold outreach + pilots carry the load |
| Cold outreach reply rate is <5% | MEDIUM | HIGH (no pilots = no proof = no launch) | If <5% in week 2, refine ICP and outreach copy; consider hiring SDR or using LevelUp Leads-style agency |
| Pragmatic Engineer / Lenny's guest pitches all rejected | HIGH (these are competitive) | MEDIUM | Plan B: own newsletter, build to 1k subs in 6 months; podcast guesting as the higher-probability surface |
| $40/seat doesn't survive procurement | HIGH if no wedge | HIGH | Either find the wedge (Section 1) or drop to $20-25/seat to remove procurement objection |
| Calendar pressure forces premature launch | HIGH (founder bias) | HIGH | Lock the PMF gate (Section 5a) and refuse to launch on calendar |
| Rands Slack ban for self-promo | MEDIUM | LOW (one community) but compounds to reputation damage | Refuse to pitch in Rands for at least 90 days of genuine participation |
| Procurement adds 30-90 days to "pay" timeline | CERTAIN | Resets validation gate | Already mitigated by Section 5a gate redesign |
| Acquisition-treadmill (no compounding loop) | MEDIUM | HIGH long-term | Build in-product referral mechanic; commit to content compound; design partner case studies as compounding artifact |
| Two ex-Google ICs burn out trying to be sales + content + product | HIGH | HIGH | Explicitly split: one founder primarily on build, one primarily on GTM. Pause non-critical product polish |

---

## Outside voice — independent critique (self-administered)

Per skill instructions, run an outside voice. In this fixture I cannot spawn a Codex/subagent; instead I do an honest adversarial reread.

**1. Biggest marketing risk the inside review missed:**
The Director-of-Engineering buyer rarely buys NEW tools without an existing reference customer in their network. The plan assumes design partners → social proof → broader adoption, but underestimates **the cold-start trust problem**: the FIRST design partner is the hardest, because no one wants to be the first reference. The plan needs an explicit warm-intro-leverage strategy for design partner #1 (likely an ex-Google founder-network EM who buys on relationship, not on social proof).

**2. Channel mentioned that's weaker than positioned:**
LinkedIn organic. I scored it MEDIUM-HIGH leverage, but LinkedIn organic reach for technical founders without an existing audience is brutal (algorithm favors job-change announcements and bland thought-leadership; technical depth gets buried). Realistic expectation: 200 impressions per post for the first 3-6 months. Honest re-score: MEDIUM not MEDIUM-HIGH.

**3. Audience claim lacking evidence:**
The "Priya" ICP composite is plausible but unvalidated. The founders have not actually talked to a Priya yet. Until they do 5+ buyer interviews, "Priya wants cross-tool aggregation" is a hypothesis, not data.

**4. Provocative reframe the founder might not have considered:**
**Do not build a Linear-clone for Mid-Market.** Consider instead: build a *cross-tool aggregation layer* that sits on top of Linear AND Jira (the actual pain Priya described). Don't compete with Linear; integrate with Linear and Jira, and sell the layer that solves cross-tool reporting / quarterly planning. This is a MUCH smaller surface area, much faster to ship, much easier to position ("not replacing your tool, solving your reporting hell"), and Linear becomes a partner rather than a competitor. Worth seriously considering as a pivot before more build investment. (This is the kind of premise-shift the office-hours skill would surface in detail.)

---

## Summary action items (this week)

Three load-bearing commitments for the founders THIS WEEK:

1. **Build the named-50 EM list** by end of week. Specific, named EMs at named 50-500-person SaaS companies. Mine ex-Google diaspora first.
2. **Conduct 5 user interviews** with named EMs in the next 14 days. Specifically ask the questions in Section 6a (WTP, current spend, pain) AND the M0e dogfood-pivot questions. Validate or invalidate "Priya."
3. **Decide the wedge** by end of week 2. Cannot be "better Linear." Must be a segment / use case Linear publicly does not serve. Options listed in Section 1 1b deltas. Pick one.

Schedule self-check: re-run `/plan-cmo-review` in 30 days to evaluate progress against this plan.

Recommended follow-up skills:
- `/office-hours` — STRONGLY RECOMMENDED before more build. The "better Linear" framing should not survive a serious office-hours session.
- `/plan-ceo-review` — if the wedge pivot changes pricing or ICP materially
- `/plan-eng-review` — once the wedge is locked, re-review the product spec against the wedge

---

## WebSearch URLs invoked

- [Linear pricing 2026](https://linear.app/)
- [Linear vs Jira vs Shortcut comparison](https://tech-insider.org/linear-vs-jira-2026/)
- [Linear case study — Eleken](https://www.eleken.co/blog-posts/linear-app-case-study)
- [Linear $100M ARR with $35K marketing spend — GrowthHunt](https://www.growthhunt.ai/growth-story/linear)
- [Pragmatic Engineer Linear story](https://newsletter.pragmaticengineer.com/p/linear)
- [Pragmatic Engineer about & ethics on sponsorship](https://newsletter.pragmaticengineer.com/about)
- [Pragmatic Engineer podcast sponsorship](https://blog.pragmaticengineer.com/podcast-sponsorship/)
- [B2B SaaS pricing models](https://softwarepricing.com/blog/saas-pricing-models/)
- [Tegon Show HN](https://news.ycombinator.com/item?id=40912920)
- [Linear waitlist 10k story — Growth Letter](https://www.growth-letter.com/p/this-startup-had-10000-people-on)
- [Cold email SaaS benchmarks](https://www.saleshandy.com/blog/saas-cold-email/)
- [B2B SaaS cold outreach engineering managers](https://www.cleverly.co/blog/cold-email-strategy-for-b2b-saas)
- [LeadDev community](https://leaddev.com/the-human-centered-technical-community)
- [Rands Leadership Slack](https://randsinrepose.com/welcome-to-rands-leadership-slack/)
- [Superhuman PMF engine — First Round](https://review.firstround.com/how-superhuman-built-an-engine-to-find-product-market-fit/)
- [Linear's path to PMF — First Round](https://review.firstround.com/linears-path-to-product-market-fit/)
