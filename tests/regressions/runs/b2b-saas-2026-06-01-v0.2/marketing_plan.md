# Marketing Plan — Threadline (B2B SaaS, Linear-style PM for engineering teams)

**Skill:** plan-cmo-review v0.2
**Run date:** 2026-06-01
**Fixture:** b2b-saas (synthetic)
**Founders:** 2 ex-Google engineers, no prior B2B sales experience
**Marketing-naive default:** ACTIVE (no qualifying evidence rebuts it; premise-challenge is load-bearing)

---

## PREMISE-LEVEL FINDINGS BLOCK

**4 of 5 Step 0.5 premises FAILED. This block is mandatory.**

The plan as written reflects technically-strong, B2B-marketing-naive founders accepting a set of premises that contradict each other and contradict the canonical motion-class playbook. Before any tactical optimization, the founders owe themselves answers to these five strategic questions:

1. **Motion mismatch — bottom-up market, top-down pricing.** Linear/Notion/Slack ALL won this category with aggressive free tiers driving bottom-up adoption + team-invite virality. Threadline's "no free tier, $40/seat, 14-day trial" cuts off the proven playbook for the category and substitutes a sales-led mid-market motion the founders have ZERO experience executing (no B2B sales background). Either change the motion (add free tier; let bottom-up work) OR change the GTM team (hire B2B sales; build SOC 2 first; accept 12-month sales cycle). The current plan does neither and assumes the trial converts on its own. **It will not.**

2. **Procurement reality vs trial mechanic.** Mid-market (50-500 person SaaS cos) procurement REQUIRES SOC 2 Type II (80% of RFPs), SSO, and 4-8 weeks of security review. SOC 2 Type II takes 10-14 months to achieve. A 14-day trial doesn't survive the procurement clock. The validation cohort at day 30 will be small teams (10-25 seats) and solo developers — NOT the stated ICP. The 5-companies-by-day-30 gate validates the wrong segment.

3. **Launch channel sells to the influencer, not the buyer.** Show HN reaches IC engineers. The $40/seat purchase decision is made by EMs and tech leads. HN can plant bottom-up seeds (if the product allows bottom-up — which the no-free-tier model doesn't), but it does NOT close mid-market deals. The plan conflates awareness with procurement.

4. **Positioning is reactive, not positional.** "Better than Linear" requires an X that's visible on first glance. The doc doesn't name the X. Linear's wedge against Jira was "fast, opinionated, designed by ex-Airbnb design taste." Threadline's wedge against Linear is unstated. Without it, the EM asks "why switch from a tool that works?" and the answer is silence.

5. **Dogfood mismatch.** Ex-Google IC founders dogfooding 2-person workflows will ship a fast IC tool. The buyer (EM at 50-500 person SaaS) needs roll-up reporting, cross-team dependency views, SSO admin, audit logs, exec dashboards. The product will be calibrated for the wrong audience signature unless EM/tech-lead interviews drive feature selection BEFORE feature lock.

**The single most important question for the founders to answer this week:** Are you running a bottom-up motion (free tier, team virality, multi-year cadence) or a sales-led mid-market motion (SOC 2, named accounts, AE hires, 12-month cycles)? You cannot run both with the current resources. The plan as written attempts both and ships neither.

(Tactical sections 1-9 below proceed AS IF the founders will reckon with the above; tactics that depend on the motion choice are flagged accordingly.)

---

---

## Step 0 — Pre-review system audit

### Existing context read

The fixture provides a one-paragraph design doc only — no implementation doc, no landing page yet, no prior planning artifacts named. Explicit marketing claims in the doc:

- Pricing: $40/seat/month, no free tier, 14-day trial
- ICP: engineering managers, tech leads, IC engineers at 50-500 person SaaS companies
- Distribution: "Show HN at launch + content marketing on the engineering management blog" (note: blog doesn't exist yet)
- First 10: "Founders' friends + HN cohort"
- Validation gate: 5 paying COMPANIES by day 30 (calendar-driven)
- Differentiation: "Better than Linear for engineering-specific workflows"

### Competitive landscape (web search summary, expanded in Section 1)

Direct competitors:
- **Linear** — $10/seat Basic, $16/seat Business, free tier with unlimited members + 250-issue cap. Annual billing required for paid. Bottom-up adoption, design-led, opinionated PM. THIS IS THE ANCHOR THREADLINE POSITIONS AGAINST.
- **Jira** (Atlassian) — incumbent, $7-15/seat depending on tier; widely disliked but entrenched
- **Shortcut** (née Clubhouse) — engineering-focused PM, $8-12/seat
- **Height** — AI-first PM, recently struggled/sunset trajectory per 2026 coverage
- **Plane** — open-source Linear alternative

### Founder audience audit (numeric)

- X/Twitter following: **200** (negligible by B2B-marketing standards; AND not segmented as eng-leader-followers)
- Email list: **~50** personal (not professional segmentation)
- LinkedIn following: NOT REPORTED (notable absence — LinkedIn is the strongest B2B channel; ex-Google network should be ≥1000 by default)
- Content history: **None professional**
- GitHub stars on prior OSS: NOT REPORTED
- Newsletter: None
- Community presence (eng leadership Slacks, Rands Leadership, etc.): NOT REPORTED
- Prior shipped B2B products: None (no B2B sales experience stated)

**Read:** This is a zero-audience start for the B2B engineering-leader segment. 200 X followers is a rounding error against The Pragmatic Engineer (800k+) and Lenny's Newsletter (millions). The founders have ex-Google credibility — a real but soft asset — but no demonstrated channel into eng-leader attention.

### Activation rule trigger

By the skill's activation rules:
- Zero audience + competitors identified → ordinarily Mode C (Audience-Build Sprint)
- HOWEVER: ex-Google network is a latent asset (probably 500-2000 reachable engineering managers via LinkedIn/warm intros if mined). This is NOT "zero audience" — it's "untapped audience surface area."
- Recommend **Mode A (Full Review)** with explicit Audience-Build Sprint embedded as Section 4 — because the marketing problem in B2B SaaS is not just audience-building; it's also procurement, SSO/SOC 2 readiness, motion choice, ICP precision. Mode C alone would skip too much. Locked in Step 0B below.

**Default marketing-naive assumption: ACTIVE.** No qualifying evidence rebuts it. The founders are technically strong (ex-Google) but have no prior B2B traction, no marketing track record, no documented audience. Premise-challenge is load-bearing.

---

## Step 0.5 — Premise audit

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| P1 | Launch on Show HN | "Distribution Plan" | HN is reasonable for eng audiences BUT Show HN does not produce procurement-grade trust at $40/seat * 50-500 seats = $24K-$240K ACV — needs verification, not refutation |
| P2 | Content on "engineering management blog" | "Distribution Plan" | Singular "the" — implies blog doesn't exist; this is a 6-12 month asset, not a launch tactic |
| P3 | $40/seat/month, no free tier | "Pricing" | 4x Linear's $10/seat Basic. Anchored UP from competitors. ICP-WTP evidence missing. Bold but unjustified |
| P4 | 14-day trial | "Pricing" | Time-based trials in B2B PM tools usually start AFTER procurement (SOC 2 review etc.), not before. Procurement timeline > 14 days for mid-market |
| P5 | 5 paying companies by day 30 | "Validation gate" | Calendar-gated for a retention-driven product. SOC 2 Type II takes 10-14 months; without it, mid-market RFPs disqualify you. Day 30 = ~friends-of-friends only |
| P6 | First 10: "Founders' friends + HN cohort" | "First 10" | Friends-of-founders are NOT mid-market eng-team buyers; they are individual engineers/startups. Wrong segment for the stated ICP |
| P7 | "Better than Linear" positioning | "Differentiation" | Reactive, not positional. "Linear but X" requires X to be visible at first glance; no X stated |
| P8 | No free tier | "Pricing" | Cuts off bottom-up adoption — the EXACT motion Linear/Notion/Slack used to dominate. Major strategic premise to challenge |
| P9 | ICP is "EM + tech lead + IC engineer" | "Target users" | Three different buyer profiles. EMs make purchase decisions; ICs influence; tech leads bridge. Conflated = unfocused positioning |
| P10 | "Engineering management blog" implies EM is content audience | inferred | But ICs are the daily users in bottom-up motion. Content target ≠ user target. Worth challenging |

### M0a. Launch-platform audience-class fit

**Premise:** Launch on Show HN.

**Founder's naive answer:** "Our product is for engineering teams; HN is full of engineers; this is the obvious place."

**Web search:** HN audience composition skews "predominantly software engineers" — IC engineers and senior ICs more than engineering managers. Themes that resonate: work/life balance, high-quality codebase, technical depth. Successful Show HN posts for PM-adjacent tooling exist (Linear had quiet HN adoption; Plane open-source resonates with HN; Height got attention). HN is genuinely a credible eng-audience platform — UNLIKE the tldrof case where HN was a category error.

**However, two important caveats:**
1. HN reaches **IC engineers more than engineering managers**. The buyer for a $40/seat team tool is the EM/tech lead. HN sells to influencers, not deciders.
2. Show HN produces awareness, not procurement signal. A $24K-$240K mid-market deal does not close from a Show HN post; it closes after a 30-90 day evaluation including SOC 2/SSO review.

**Verdict: PREMISE SURVIVES — with significant scope limitation.** HN is a reasonable awareness channel; it is NOT a viable "first 10 paying customers" channel for this price band and procurement profile. The naive founder answer over-weights HN's role.

**Cascading implication:** M2 (discovery path) must NOT have "Show HN" as step 1 toward paying customers. HN can be step 1 toward AWARENESS for ICs who then advocate upward, but the real conversion path runs through EM/tech lead trust channels (LinkedIn, eng leadership newsletters, peer references). Founders should treat HN as top-of-funnel + recruiting credibility, not as a sales channel.

### M0b. Canonical-success comparable

**Premise (implicit in doc):** "Be better than Linear" as positioning. No explicit canonical-success playbook named.

**Founder's naive answer:** "Linear is the comparable — they're the modern winner in this space."

**Web search:** Linear IS a direct competitor, but the canonical-success PLAYBOOK Linear used has named patterns the doc isn't following:

- **Linear's playbook:** Bottom-up adoption via FREE TIER (unlimited members, 250-issue cap). "One person starts using it, invites their team, which then invites other teams." Polish-as-marketing, founder presence (Karri Saarinen), opinionated stance against bloat. Network effects from team-invite virality. NO heavy paid acquisition.
- **Notion's playbook (same motion class — workspace/PM tool):** Bottom-up via aggressive free tier; "individual users embed in workflows, pull into orgs"; community-led (template gallery, evangelism); 95% organic growth. TikTok virality in Jan 2021.
- **Slack's playbook (team collab, same buyer pattern):** Free tier with usage caps that hit at team scale; bottom-up; team-channel virality.

**The pattern these THREE canonical successes share that Threadline's plan DOES NOT:**
1. Free tier as the virality engine (Threadline = "no free tier")
2. Bottom-up motion gated by free → paid upgrade triggers (Threadline = trial-only, no bottom-up entry)
3. Multi-year content + product cadence before mass-market traction (Threadline = "Show HN at launch")
4. Founder-as-content-channel (Karri Saarinen blog, Ivan Zhao interviews, Stewart Butterfield bench) — Threadline founders have NO content history

Direct-competitor-only thinking ("be better than Linear") misses that Linear WON with a free tier and 5+ years of polish-as-marketing. "Better than Linear, with no free tier, launching on Show HN" is the opposite playbook.

**Verdict: PREMISE FAILS.** The plan implicitly anchors on Linear as competitor but ignores Linear/Notion/Slack as PRECEDENTS for the motion class. The canonical-success playbook for "Linear-style PM for engineering teams" requires free tier + bottom-up + multi-year cadence. The plan has none of these.

**Cascading implication:** The pricing premise (P3, P8) needs full re-examination in Section 6. The launch sequence (Section 5) cannot assume bottom-up team-invite virality without the free-tier mechanic that makes it work. The "5 paying companies by day 30" gate (P5) is implausible against this motion class's precedent (Linear took years; Notion took years).

### M0c. Anti-feature surface

**Premise:** All in-scope features serve the paying ICP.

**Founder's naive answer:** "We're building Linear for engineering teams; everything we ship is for engineering teams."

**Doc lacks an explicit feature list**, so I'll work from positioning: "Linear-style project tracking for engineering teams... engineering managers, tech leads, IC engineers." Three buyer profiles. Likely-anti-feature candidates by inference:

1. **"No free tier" combined with bottom-up tool category** → This is itself an anti-feature relative to positioning. The product TYPE (PM tool for teams) requires bottom-up adoption to land; the BUSINESS MODEL (no free tier) cuts off the adoption path. Direct contradiction.
2. **14-day trial in a mid-market B2B PM tool** → Anti-feature relative to procurement reality. Mid-market buyers run SOC 2/SSO reviews that exceed 14 days. Trial starts before evaluation can finish; clock runs out mid-procurement; trial converts at very low rates.
3. **Calendar-gated launch (day 30 validation)** → Anti-feature relative to retention-led PM motion. Linear shipped quietly, iterated for years; Threadline plans to gate validation at day 30 with no PMF signal.
4. **"Show HN" as primary launch** → Anti-channel relative to the EM/tech-lead buyer. Sells to IC engineers (HN audience) not EMs (decision-maker).

**Verdict: PREMISE FAILS.** At least 2 anti-features (no free tier + 14-day trial + calendar gate + HN-primary launch are 4 separate contradictions to positioning/business model). The founders owe themselves the decision: kill, defer, or restrict per anti-feature.

**Cascading implication:** Section 6 must directly address the no-free-tier / no-bottom-up decision. Section 5 must address the trial-length and gate-type decisions. These are not optimization questions; they are strategic motion questions.

### M0d. Freebie-disqualifier (acquisition-mechanic selection bias)

**Premise:** 14-day free trial as acquisition mechanic.

**Founder's naive answer:** "Free trial is standard for B2B SaaS; it's how Linear and everyone else does it."

**Diagnostic — who does a 14-day free trial actually attract?**
- Time-rich evaluators willing to set up a tool, import data, and run a parallel system for 14 days
- For PM tools specifically: solo developers, very small teams (2-5 people), curious EMs at unfunded pre-seed startups
- NOT mid-market 50-500 person eng teams: those teams require IT/Security review, data migration planning, change management, and budget cycles BEFORE they can meaningfully trial

**For the stated ICP (mid-market eng teams), the procurement reality:**
- SOC 2 Type II is a precondition (80% of mid-market RFPs require it; Threadline likely doesn't have it on day 1)
- SSO via Okta/Google Workspace is a precondition
- IT-approved data residency / vendor risk assessment takes 4-8 weeks
- Procurement budget cycles are quarterly

A 14-day trial doesn't even survive the procurement clock. **The trial selects FOR small early-adopter teams and AGAINST the stated ICP.**

**Verdict: PREMISE FAILS.** Cheap-trial mechanic produces validation theater. The 5 trial signups will be small teams (10-25 seats), validating a different segment than the 50-500 person target. The founders will mis-tune the product to small-team needs.

**Cascading implication:** Section 5 (launch playbook) must propose a high-trust alternative: design partner program (manual onboarding + concierge of 5-10 named teams) BEFORE public trial launch. Section 6 must address tier strategy: free-for-small + paid-for-team is the canonical play. Section 8 metrics must measure cohort segment, not just trial→paid conversion (which will be misleading if cohorts are wrong-segment).

### M0e. Dogfood audience-class match

**Premise (implicit):** The founders, as ex-Google engineers, are dogfooding the product.

**Founder's naive answer:** "We're engineers building for engineers; we know exactly what they need."

**Analysis:**
- Founders are ex-Google engineers (likely IC SWEs, not engineering managers at scale). Their lived experience is of Google-scale tooling (Critique, Mondrian, Buganizer), not mid-market SaaS tooling.
- Stated ICP is mid-market (50-500 person) SaaS company engineering teams — culture, process, scale, and tooling-budget are DIFFERENT from Google.
- The founders likely dogfood on their own 2-person workflow. That tunes for 2-person needs (speed, minimalism, IC ergonomics) not 50-500 person needs (cross-team coordination, EM reporting views, exec roll-ups, SSO admin).

**Specific mismatches likely to emerge:**
- Founder dogfood prioritizes IC keyboard shortcuts (Linear-clone reflex); ICP needs EM weekly status views
- Founder dogfood ignores SSO/RBAC; ICP requires it on day 1
- Founder dogfood ignores audit logs / compliance; mid-market requires them
- Founder dogfood treats one project as the unit; mid-market needs org-wide programs, dependencies across teams

**Verdict: PREMISE FAILS.** Dogfood audience (2 ex-Google ICs) ≠ paying ICP (mid-market EM/tech-lead buyers at 50-500 person SaaS cos). The product will ship calibrated to the wrong audience signature.

**Cascading implication:** Section 4 audience-building must include EM/tech-lead interviews BEFORE feature lock. Section 2 ICP spec must separate buyer from user (EM = buyer, IC = user). Without this, the founders will build a beautifully-fast IC tool that EMs won't buy because it lacks the admin/reporting surface they need.

### Step 0.5 verdict summary

| # | Question | Verdict | Cascade |
|---|---|---|---|
| M0a | Launch-platform fit | SURVIVES (with scope limit) | HN = awareness only, not procurement channel; constrains M2 path |
| M0b | Canonical-success comparable | FAILS | Linear/Notion/Slack used free-tier bottom-up; plan uses opposite playbook. Section 6 pricing rethink mandatory |
| M0c | Anti-feature surface | FAILS | At least 3 anti-features (no free tier in bottom-up category; 14-day trial under SOC 2 procurement; calendar-gated retention-led product). Strategic, not tactical |
| M0d | Freebie-disqualifier | FAILS | 14-day trial selects small-team early-adopters, NOT mid-market ICP. Cohort = wrong-segment validation theater |
| M0e | Dogfood mismatch | FAILS | Ex-Google IC founders dogfooding for 2-person workflows; paying ICP is EM at mid-market. Product calibrates to wrong audience |

**4 of 5 premises FAIL.** This is a far worse premise-block than the tldrof fixture (which failed 2 of 5). The PREMISE-LEVEL FINDINGS BLOCK at top of document is mandatory and load-bearing.

The skill's "marketing-naive default" + "extrospective" stance produced the right diagnosis: the founders accept a constellation of premises that contradict each other (no-free-tier + bottom-up market; 14-day trial + mid-market procurement; calendar gate + retention-led category). These contradictions are invisible WITHIN the design doc's framing; they only surface when the framing itself is interrogated.

---

## Step 0A — Forcing questions (tactical, 7)

Step 0A inherits Step 0.5 findings. Refusals are sharper because the framing has already failed in 4 of 5 dimensions.

### M1. Audience reality

**Founder's naive answer:** "Engineering managers and tech leads at 50-500 person SaaS companies. They hang out on HN, read Lenny's, lurk in Rands Leadership Slack."

**Challenge:** Three roles named (EM + tech lead + IC) ≠ one audience. The BUYER is the EM; the DAILY USER is the IC; the tech lead bridges. They have different attention surfaces. "Lurk in Rands Leadership" is a real signal but Rands' Slack has explicit anti-vendor norms. Lenny's audience is heavily PM-skewed, not EM-skewed. Naming three roles and three places is generic, not specific.

**Sharpened answer (what the founders should arrive at):**
- **Primary BUYER persona:** "Priya, VP Eng at a 180-person Series B SaaS company (e.g., a Fintech, devtools co, or vertical SaaS). 12 years experience (was a tech lead at Stripe, now manages 4 EMs / 30 engineers). Reads The Pragmatic Engineer weekly (paid subscriber); listens to Engineering Enablement Podcast; active in a private Slack of ~50 VP Eng peers; attends LeadDev SF annually."
- **Secondary USER persona:** "Marcus, Senior Eng / Tech Lead, leads a 6-person team within Priya's org. Sets up the tooling. Reads The Pragmatic Engineer free tier, lurks HN, active on Bluesky for tech."
- **Decider chain:** Marcus discovers → uses on small project → recommends to his EM → EM presents to Priya → Priya approves budget → Procurement runs SOC 2/SSO review → contract.

**Verdict:** M1 answer needs explicit buyer/user split + named publications/communities with realistic access patterns. Concrete 5+ attributes per persona, 3+ named attention surfaces per persona.

### M2. Discovery path

**Founder's naive answer:** "They see our Show HN post, click through, sign up for trial, convert."

**Challenge — REFUSED.** Per skill rules (Step 0A refusal list AND Step 0.5 M0a cascade): "Show HN" cannot be step 1. Compounded refusal: this path also collapses "discover" and "buy" into one step, which doesn't survive mid-market procurement.

**Sharpened path (the real 5-7 step path):**
1. Marcus (tech lead) sees a Pragmatic Engineer issue mentioning Threadline as one of "5 tools shaking up engineering PM" (sponsorship or feature)
2. Or: Marcus sees Show HN post, upvotes, bookmarks (no action yet)
3. Marcus signs up FREE TIER (if it exists; if not, never signs up at all)
4. Marcus uses on a side-project for 2 weeks
5. Marcus recommends to EM
6. EM reviews + asks Priya (VP Eng) for budget
7. Procurement runs SOC 2 / SSO review (4-8 weeks)
8. Annual contract signed

Time-to-first-revenue from Show HN: realistically **3-6 months**, NOT day 30.

### M3. Pre-launch audience

**Founder's naive answer:** "200 X followers, ~50 email list."

**Challenge:** That's the raw count; what's the EM-overlap? 200 X followers of ex-Google ICs are likely 80% other engineers (peer, not buyer). Email list is personal, not professional. **For the stated B2B mid-market ICP, the effective audience is functionally zero.**

What's MISSING from the audit and should be reported:
- LinkedIn following — ex-Google should have 500-2000 default connections; this is the strongest B2B channel and was not mentioned
- GitHub stars on prior projects — if either founder shipped OSS, this is a credibility surface
- ex-Google peer network — these are the realistic "first 10" warm-intro pool, NOT "founders' friends"

**Sharpened answer:** "Effective ICP-overlap audience is zero. Latent audience (ex-Google peer network) is unknown until quantified — assignment: each founder writes a list of every engineering manager / tech lead they know personally at a 50-500 person SaaS company. Target: 30-50 names between them."

### M4. Channel honesty

**Founder's naive answer:** "We're good at building, and we can write content for the engineering management blog."

**Challenge — REFUSED.** "We can write content" is aspirational; no published writing exists. "The engineering management blog" doesn't exist (singular "the"). Building skill ≠ distribution capability. The founders have **NO demonstrated channel advantage**.

**Sharpened answer:**
- Honest "we don't have one yet" → triggers Channel-Build as the load-bearing pre-launch work item
- Realistic latent advantages: (a) ex-Google credibility for warm intros via LinkedIn; (b) technical depth for "engineering manager guide to X" long-form content (but they have no track record so it'll take 6-12 months to build)
- The actual channel advantage the founders have is **warm intro economics within the ex-Google diaspora**. That's the unfair advantage. Not a blog they haven't written.

### M5. Competitor traffic source

**Founder's naive answer:** "Linear gets traffic from Twitter and word-of-mouth, I think."

**Challenge — REFUSED.** "I think" is guess. Required: actual evidence.

**Sharpened (from web search):**
- **Linear:** organic search (Linear.app ranks for project management queries), Twitter/X (Karri Saarinen + Tuomas Artman build-in-public), product-led virality (team invite mechanic), Lenny's Newsletter feature (paid sponsorship), HN organic, design-community word-of-mouth (Dribbble/Designer Hub).
- **Notion:** TikTok virality, template gallery SEO, Lenny + product creator partnerships, community evangelism.
- **Shortcut/Height:** SEO + comparison content + paid Google ads on competitor terms.

**Founders' assignment:** Run SimilarWeb on linear.app, notion.so, shortcut.com, height.app, plane.so. Capture top-5 referrers per competitor. Map to Threadline's accessible channels.

### M6. First 10 paying customers

**Founder's naive answer:** "Founders' friends + HN cohort."

**Challenge — REFUSED.** "Friends" is unnamed; HN cohort is passive ("whoever sees the launch"). Per skill: name the 10 specific people you'd email tomorrow.

**Sharpened (what the founders should produce this week):**
- List 10 named former Google peers who are now engineering managers / tech leads / VPs Eng at 50-500 person companies
- Verify each is genuine ICP (company size, role, decision authority)
- Draft 1-paragraph personal email to each, NOT pitching — asking for 20-min product feedback call
- Of those 10: target 3-5 to become design partners (concierge onboarding, free for 6 months, in exchange for product input + reference rights at launch)
- These are the REAL first 10. The HN cohort is awareness top-of-funnel, not customer pipeline.

### M7. Time allocation

**Founder's naive answer:** "We've spent 100% on building so far. Marketing starts at launch."

**Challenge — REFUSED.** Per skill: "I'll start marketing after launch" is an anti-pattern. With zero audience and a 6-12 month content/audience build curve, audience-build needed to start 6 months ago.

**Sharpened answer:**
- Founder A: 50% on remaining product build, 50% on design-partner outreach + interviews + Pragmatic Engineer/Lenny sponsorship research
- Founder B: 70% on SOC 2 Type I kickoff + SSO build (procurement prerequisites) + 30% on technical content (one long-form "engineering manager's guide to issue tracking workflows" piece this month)
- Stop building product features the founders haven't validated with named EM interviews. The current ratio (assumed 100% product) is exactly the failure mode the skill exists to prevent.

### Completion criteria

All 7 questions answered (with sharpening from naive baseline). M3 reveals zero ICP-overlap audience. M4 reveals no demonstrated channel. M6 needs concrete list this week. M7 needs full re-allocation. Step 0B mode selection follows.

---

## Step 0B — Mode selection

**Selected: Mode A — Full Marketing Review** with Section 4 elevated to Audience-Build Sprint priority.

**Reasoning:**
- Pure Mode C (Audience-Build Sprint only) would skip the strategic motion question (free tier? bottom-up? sales-led?) which is the load-bearing decision per Step 0.5. Skipping it means the audience-build runs against an undefined target.
- Mode A covers competitive analysis (Section 1), ICP precision (Section 2), channel scoring (Section 3), pre-launch audience build (Section 4), launch playbook with gate-question (Section 5), pricing band question (Section 6), growth loops (Section 7), metrics (Section 8), risk (Section 9). All needed for a B2B SaaS fixture where the motion choice is itself unresolved.
- Mode B (Focused Review on 1, 3, 5) would skip Section 4 and Section 6, which is where the load-bearing strategic decisions live for this fixture.

Mode A locked.

---

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Competitor | URL | Founded | Pricing | Acquisition channels | User complaints | Threadline read |
|---|---|---|---|---|---|---|
| Linear | linear.app | 2019 | Free (250 issues / unlimited members), Basic $10/seat, Business $16/seat, Enterprise custom; annual billing for paid | Organic search, Twitter (founder presence), team-invite virality, Lenny's sponsorship, HN, design community WOM | "Pricing creep", "no read-only tier", "limited customization", contractors count as full seats | The category leader. Polished, opinionated, design-led. Threadline must explicitly outflank, not match. |
| Jira (Atlassian) | atlassian.com/jira | 2002 | $7-15/seat depending on tier; free up to 10 users | SEO dominance, enterprise sales, partner ecosystem | "Bloated", "slow", "configuration nightmare", "Atlassian acquired everything and broke it" | Vulnerable to "modern, fast, opinionated" alternative — but Linear already owns that pitch |
| Shortcut (née Clubhouse) | shortcut.com | 2014 | $8.50/user Team, $12 Business | Engineering content marketing, comparison-page SEO, Google Ads | "Less polished than Linear", "fewer integrations", "iteration slow" | Threadline's closest direct comparable in positioning. Shortcut is what "Linear, but for slightly different engineering teams" actually looks like — and it's middling. Cautionary tale. |
| Height | height.app | 2018 | AI-first PM; recent reports indicate the product is struggling/sunsetting in 2026 | Initial Y Combinator buzz, AI-PM positioning | "Pivoted too many times", "AI-PM didn't differentiate" | Threadline should study what FAILED here — chasing AI-PM differentiation without clear engineering-team wedge |
| Plane | plane.so | 2022 | Open-source self-host free; cloud paid (~$5-10/seat) | GitHub stars (~30k+), open-source community, HN | "Less mature than Linear", "early on enterprise features" | The open-source flank. If a team is cost-sensitive, Plane is the alternative, not Threadline. |

### 1b. Canonical-success comparables

This is the part the founders' plan skips entirely.

| Canonical | Price | Founded | Scale | Primary acquisition | Onboarding model | Launch gate | DELTA vs Threadline plan |
|---|---|---|---|---|---|---|---|
| **Linear** | $10-16/seat | 2019 | $400M+ valuation, dominant in modern PM | Bottom-up free tier → team virality + polish-as-marketing + founder presence | Self-serve PLG with free tier | PMF-signal-driven; shipped quietly, iterated 1+ year before mass-market push | Threadline has NO free tier (kills the team virality engine), NO founder content history, calendar gate (day 30) |
| **Notion** | $0-15/seat | 2016 | $10B valuation, 30M+ users | 95% organic; community evangelism, template gallery SEO, TikTok virality (2021), bottom-up adoption | Self-serve free; expand to paid via team scale | Multi-year cadence; near-collapse and re-pivot in 2018-2019 | Threadline has NO free tier (cuts off the proven motion), NO community surface area, NO multi-year content asset |
| **Slack** | $0-15/seat (similar tier) | 2013 | $27B Salesforce acquisition (2021) | Bottom-up via free tier with usage caps; team-channel virality; press coverage of "email killer" narrative; founder credibility (Butterfield from Flickr) | Self-serve free with hard caps that hit at team scale | Multi-year private beta; massive press coverage at launch via founder network | Threadline has NO free tier, NO founder press leverage, NO multi-year private beta cadence |
| **Superhuman** (different motion class but instructive — concierge B2C/B2B prosumer at $30/seat) | $30/seat | 2017 | ~$825M Grammarly acquisition (Jul 2025) | Invite-only waitlist, Vohra-personally-onboards-first-200, two-sided referral | Concierge onboarding | Vohra "very disappointed" ≥40% test — PMF-signal gate, not calendar | Threadline could borrow this gate logic for design-partner cohort instead of calendar day-30 |

### 1c. Pattern surface

**What ALL canonical successes did that Threadline's plan does NOT:**

1. **Aggressive free tier as the virality engine.** Linear, Notion, Slack — every one used free tier + usage cap → paid upgrade. Threadline's "no free tier" cuts off the proven motion for the category.
2. **Multi-year cadence before mass-market push.** Linear iterated 1+ year, Notion 4+ years (with a near-death pivot), Slack 3+ years of private beta. Threadline plans 20-22 day build + day-30 validation.
3. **Founder-as-channel.** Karri Saarinen (Linear), Ivan Zhao (Notion), Stewart Butterfield (Slack) all had founder-content presence BEFORE launch. Threadline founders have none.
4. **PMF-signal-driven gates, not calendar gates.** Superhuman used Vohra ≥40% test; Linear gated on team-retention signal; none of them said "5 customers by day N or we kill it."
5. **Bottom-up motion explicitly designed.** Every canonical success has a "single user starts, invites team, team viral-loops into org" motion. Threadline's pricing/trial structure prevents this loop from running.

**Direct competitors (Jira, Shortcut, Height) diverge from canonical-success patterns** — Jira is sales-led/enterprise-locked; Shortcut is mid-pack and stuck there because it copied Linear's positioning without the polish; Height failed by chasing AI without anchor. NONE of the direct-competitor alternatives are the right model.

**Pattern Threadline is implicitly following:** A hybrid of (a) Linear-like positioning, (b) traditional mid-market B2B SaaS pricing/procurement, (c) HN-launch tactical motion. This combination has no canonical-success precedent. The closest historical analog is "second-mover B2B PM tool that copied Linear's surface without its motion" — which is what Shortcut became, and Shortcut is not a target outcome.

**Founder action this week:** Read three pieces — (1) Lenny Rachitsky's "How Linear Builds Product" interview with Karri Saarinen; (2) the Notion "near-collapse to $10B" essay (Xiayi Sun on Medium); (3) Vohra's "How Superhuman Built an Engine to Find Product/Market Fit" essay. Extract: what gate did each use? what was the free-vs-paid mechanic? what was the cadence to first 1000 paying users?

---

## Section 2 — ICP specification

Tightened ICP — separating BUYER from USER (a separation the design doc collapsed). See also `icp.md` for the standalone artifact.

### Primary BUYER persona — "Priya"

- VP Engineering at a 100-300 person Series B/C SaaS company (Fintech, devtools, vertical SaaS — NOT marketplaces or consumer apps)
- 10-15 years experience; former tech lead at a FAANG or top-tier startup; now manages 3-6 EMs / 25-60 engineers
- Reports to CTO; controls tooling budget for engineering org ($50K-$300K/year)
- Procurement authority for sub-$50K annual contracts; routes >$50K through CFO/IT
- **Where she pays attention RIGHT NOW (≥5 specific):**
  1. The Pragmatic Engineer (paid sub)
  2. Engineering Enablement Podcast / Eng Leadership Weekly
  3. LeadDev conference (annually); LeadDev London/SF newsletter
  4. Private "VP Eng peers" Slack of ~30-80 senior eng leaders
  5. LinkedIn — actively reads/comments on posts from peers and respected eng leaders (Gergely Orosz, Will Larson, Charity Majors)
  6. Twitter/X — light usage, mostly via Gergely / Will Larson / Charity Majors threads
- **What she currently pays for (adjacent categories):**
  - Linear or Jira ($10-15/seat)
  - Datadog / Honeycomb (observability) — $20-100/seat
  - GitHub Enterprise — $21/seat
  - Pragmatic Engineer / Lenny's paid subs ($150-300/year each, personal expense or expensed)
- **What she complains about in those tools:**
  - Linear: "amazing UX but our 200-person org needs roll-up reporting and cross-team dep tracking that Linear deprioritizes"
  - Jira: "too much, too configurable, too slow"
  - GitHub Projects: "lightweight but doesn't replace a real PM tool"
- **Objections she will raise to Threadline:**
  - "Why switch from Linear/Jira? Switching cost = 2 months of team friction. Show me 3x value, not 1.2x."
  - "SOC 2? SSO? Audit logs? Data residency? If no on any of these, can't even start a procurement conversation."
  - "Who else my size uses you? Show me 3 reference customers at 100-300 person SaaS cos."
  - "Will you be around in 3 years? 2 founders, no funding stated, no revenue — high replacement risk."
- **Reasons she would convert:**
  - A specific named workflow gap in Linear that Threadline solves natively (e.g., cross-team dependency tracking with EM-level rollup views; or program management built on top of issues; or AI-driven sprint planning that actually works)
  - A trusted peer recommendation from her VP Eng Slack
  - A Pragmatic Engineer or Lenny feature with a concrete case study
  - Free design-partner program with 6-month free + concierge onboarding from a founder

### Secondary USER persona — "Marcus"

- Senior Engineer / Tech Lead at Priya's company; runs a 5-8 person sub-team
- Hands-on Linear/Jira user; sets up boards, workflows, sprints
- **Where he pays attention:** HN front page daily, The Pragmatic Engineer free tier, GitHub trending, Bluesky for tech, lobste.rs, his team's internal Slack
- **Conversion role:** discovers tools, runs side-project trials, becomes internal advocate. Does NOT control budget. Does influence purchase via "the team really likes Threadline" upward signal.
- **Marcus is reachable via HN, Bluesky, lobste.rs, GitHub. Priya is not.**

### Decider chain mapped

Marcus discovers (HN / GitHub / peer) → uses on small project (REQUIRES free tier or generous trial that doesn't burn during procurement) → advocates to EM → EM presents to Priya → Priya pre-approves → Procurement runs vendor risk assessment + SOC 2 + SSO (4-8 weeks) → contract signed → rolled out to team.

**Time from Marcus discovery to first $: 60-120 days, NOT 30.**

### Anti-persona (who Threadline should NOT chase in first year)

- Solo developers / pre-seed startup teams (2-5 people) — these are the segment a 14-day trial attracts and they will not pay $40/seat
- Enterprise (1000+ person) — procurement cycle is 6-12 months, requires AE, requires customer success team Threadline doesn't have
- Non-engineering teams (marketing, design, ops) — different positioning, dilutes wedge

---

## Section 3 — Distribution channel-by-channel

Channel scoring for THIS founders' situation (ex-Google ICs, no audience, no sales bg, $40/seat B2B).

| Channel | Reach (ICP) | Cost | Conversion | Founder fit | Effort to start | Verdict |
|---|---|---|---|---|---|---|
| Show HN | Medium (IC engineers heavy; EM light) | Low ($0) | Very low → paying for $40/seat ICP | Medium (technical founders OK at HN posts) | Low | **AWARENESS ONLY — top of funnel. Sells to Marcus, not Priya.** Use once at launch + once at major milestone. Do not over-rely. |
| Pragmatic Engineer sponsorship | High (Priya reads weekly; 800K subs; EM-heavy) | $$$$ ($5K-$15K per sponsored issue) | High (trusted recommendation context) | High (founders can produce technical case study) | Medium (need to pitch Gergely's team) | **PRIMARY CHANNEL CANDIDATE. Strongest ICP-overlap of any single channel. Save budget for 3-4 sponsorships across launch + 60d + 120d.** |
| Lenny's Newsletter | Medium-High (millions of subs but PM-skewed; some VP Eng overlap) | $$$$ ($10K-$25K) | Medium-High | Medium | Medium | **SECONDARY. Test one sponsorship; if response strong, repeat. Less ICP-tight than Pragmatic Engineer for eng-leader buyers.** |
| LinkedIn organic (founder posts) | High (Priya active there) | Free | Medium (compound over months) | Low initially (no content history) | Medium (need consistent cadence) | **MANDATORY. Founders MUST start posting weekly NOW. 6-month asset, not a launch tactic.** |
| LinkedIn warm intros (ex-Google peer network) | High (precisely ICP if mined) | Free | Very high (warm intro) | Very high (founders' actual unfair advantage) | Medium (manual) | **PRIMARY for first 10 paying. This is the founders' real channel advantage. 30-50 named contacts, 1:1 personal outreach.** |
| Engineering leadership podcasts (Engineering Enablement, Software Engineering Daily, Eng Leadership Pod) | Medium-High | Free | Medium (slow compound) | Medium (technical founders can speak well) | Medium (need to pitch, slow scheduling) | **TERTIARY but worth pursuing — 1 podcast/month founder appearance.** |
| LeadDev conference (sponsorship / speaking) | High (direct VP Eng audience) | $$$$ ($5K-$30K sponsor; speaking is "free" but selective) | High | Medium | High (multi-month lead time) | **6-month bet. Submit talk now; sponsor next event.** |
| Rands Leadership Slack | High (precise ICP) | Free | Very low for vendor self-promo (norms prohibit) | Low (must participate as person, not vendor) | High (must build presence months before pitching) | **NOT a launch channel. Founders can join, participate authentically; do NOT pitch product directly — norms ban this and bans are permanent.** |
| Twitter/X organic | Low for EM segment; medium for IC segment | Free | Low | Low (no following) | Medium | **Marcus-reach only. 200 followers won't move needle for Priya. Skip as primary; maintain as light presence.** |
| Bluesky | Low currently for EM segment | Free | Low | Low | Low | Skip for v1. |
| SEO | High over 6-12 months ("engineering project management software" type queries) | $$ (need content infrastructure) | Medium (compound) | Low (no domain authority) | Very high | **6-12 month bet. Start now: 2 long-form articles/month. Won't help launch.** |
| Cold outreach (LinkedIn DM to VPs Eng at named cos) | Medium | Free | Low (1-3% reply); higher if warm | Medium (founders haven't done it) | High (manual, time-intensive) | **OK as secondary. Layer onto warm intros — pick 50 target accounts, find 2nd-degree LinkedIn connections.** |
| Paid Google Ads | Medium (high-intent for "Linear alternative" / "Jira alternative" terms) | $$$ ($10-30 CPC on competitor terms) | Medium-Low without strong landing page | Low (founders haven't run ads) | Medium | **Premature. Run only after 5 reference customers + landing page proof.** |
| Product Hunt | Low (PH audience skews maker/IC not EM) | Free | Low for ICP | Medium | Medium (need hunter) | **SECONDARY at most. Launch 1 week after HN. Won't drive ICP signups.** |
| IndieHackers | Low (audience is solopreneurs, not mid-market eng) | Free | Very low | Low | Low | **SKIP — wrong audience for ICP.** |
| Reddit (r/ExperiencedDevs, r/devops, r/programming) | Medium for IC; low for EM | Free | Low; self-promo bans common | Low | Medium (community-first) | **NOT a launch channel. Participate as person; never self-promo.** |
| Affiliate / referral | Premature (no installed base) | Free | N/A v1 | N/A | High | **v2.** |

### Ranked surviving channels (by leverage = reach × conversion × founder fit ÷ cost ÷ effort)

1. **LinkedIn warm intros to ex-Google peer network** — highest-conversion, lowest-cost path to first 10 paying. Founders' actual unfair advantage.
2. **The Pragmatic Engineer sponsorship** — highest-reach paid channel into precise ICP. Budget for 3-4 across 6 months.
3. **Show HN at launch** — awareness only; Marcus-reach not Priya-reach. One-shot.
4. **LinkedIn founder organic content** — must start NOW; 6-month asset.
5. **Engineering leadership podcast guesting** — slow-compound, high-quality audience.
6. **LeadDev sponsorship + speaking submission** — 6-month bet for in-person credibility.

**REFUSED: "do all of them." Founders pick 3-4 to execute well. Recommendation: warm intros (#1), Pragmatic Engineer (#2), LinkedIn organic (#4), one podcast/month (#5). Skip everything else until day 90.**

---

## Section 4 — Pre-launch audience-building plan

Load-bearing. Existing audience is zero in ICP terms. See `audience_build_journal.md` for the weekly tracking template.

### Day 1-30 (start TODAY)

**Founder A — Distribution & narrative lead:**
- Week 1: Mine LinkedIn — list every ex-Google peer who is now EM / TL / VP Eng at 50-500 person SaaS co. Target 30-50 names.
- Week 1: Reach out to 20 of them with personal note (NOT pitch). Ask for 20-min product feedback / state-of-engineering-PM call.
- Week 2: Run 8-12 of those calls. Capture: what do they hate about Linear/Jira? What would make them switch? Use as raw material for both product AND content.
- Week 3: Publish 1 long-form LinkedIn post per week. First topic: "After 30 conversations with VPs Eng, the #1 PM gap I keep hearing is [X]." Cite (anonymized) interviews.
- Week 3-4: Identify 5 design-partner candidates (from the 8-12 calls). Pitch design partner program: 6 months free, founders personally onboard, feedback loop direct to product, reference rights at launch.
- Week 4: Pitch The Pragmatic Engineer team for a feature/sponsorship/guest post slot at launch (~60 days out).

**Founder B — Product & procurement-readiness lead:**
- Week 1: Kickoff SOC 2 Type I with Vanta or Drata ($5K-10K, 3-4 months to Type I report). This is the procurement-unlock.
- Week 2: Build SSO (Okta + Google Workspace at minimum). This is table stakes for mid-market.
- Week 3-4: Publish 1 technical long-form piece per month. First topic: "How we built Threadline's sync engine" (technical credibility for HN/Marcus audience).
- Week 4: Submit talk proposal for next LeadDev event.

### Day 31-60

- Continue weekly LinkedIn posts from Founder A (8 posts cumulative — start of compound)
- 2nd long-form technical piece from Founder B
- Begin podcast outreach — pitch 10 engineering leadership podcasts; target 2 appearances in Day 60-90 window
- Run 2-3 design-partner concierge onboardings (manual, founder-led)
- Apply Vohra "very disappointed" test to design partners: ≥40% answer "very disappointed if I could no longer use this"? If <40%, FIX the product before any public launch.
- Run first Pragmatic Engineer sponsorship if booked

### Day 61-90

- Integrate launch sequence (see Section 5)
- Aim for: 5 design-partner companies with concierge onboarding complete, 2 reference customer quotes, SOC 2 Type I in-progress (Type II observation period starting), Pragmatic Engineer feature scheduled, 12+ LinkedIn long-form posts published.
- Public launch ONLY if Vohra test passes AND ≥3 design partners are willing to be public references.

### Cadence summary

- LinkedIn: 1 long-form post / week from each founder (8/month combined)
- Long-form blog: 2 pieces / month
- Personal outreach: 5 net-new named contacts / week (warm intros + 2nd-degree LinkedIn)
- Podcast: 1 founder appearance / month from Day 60
- Sponsorship: 1 Pragmatic Engineer sponsorship Day 60-90

**Refused:** vague "I'll post more on Twitter" or open-ended commitments. Cadence is measurable and weekly.

---

## Section 5 — Launch playbook

### 5a. Question the launch gate

**Plan as written:** "5 paying companies by day 30." This is a CALENDAR-driven gate.

**Required question:** Is calendar the right gate for a retention-driven B2B SaaS PM tool?

**Analysis:**
- PM tools are HEAVILY retention-driven. Switching cost is high (team training, migrated data, integrations). Churn = death.
- Mid-market procurement timelines exceed 30 days BY THEMSELVES. SOC 2 reviews are 4-8 weeks. The calendar gate fires before the first procurement cycle even completes.
- Day-30 "5 companies" gate cannot be hit by the stated ICP (mid-market 50-500 person teams) because their procurement timelines exceed 30 days. The gate can ONLY be hit by small early-adopter teams (<25 seats) — i.e., the wrong segment per Step 0.5 M0d.

**Recommendation: REPLACE the calendar gate with PMF-signal gate.**

- **Primary gate (Vohra "very disappointed" test):** Run on the design-partner cohort at Day 60-75. Public launch only if ≥40% answer "very disappointed if I could no longer use this." This is the gate Superhuman used (Vohra "How Superhuman Built an Engine to Find Product/Market Fit"). It applies cleanly here.
- **Secondary gate (cohort fit):** ≥3 design partners are willing to be public reference customers. Without references, mid-market procurement stalls.
- **Tertiary gate (procurement-readiness):** SOC 2 Type I report in hand (Type II observation period started). SSO live. Without these, mid-market RFPs disqualify pre-conversation.

**If founders defend the calendar gate:** they must explain why calendar beats Vohra-style PMF signal for a retention-driven category with documented procurement timelines exceeding the gate. There is no defensible answer; the calendar gate should be replaced.

### 5b. Sequenced launch (see also `launch_playbook.md`)

Sequence assumes PMF-signal gate has passed AND SOC 2 Type I + SSO are live. If those aren't true, do NOT launch — extend Day 60-90 audience-build sprint.

| Day | Channel | Specific action | Owner |
|---|---|---|---|
| -90 | Audience-build sprint | Begin Section 4 cadence | Both |
| -60 | Design partners | Begin concierge onboarding of 5-10 named teams | Founder A |
| -30 | Pragmatic Engineer | Sponsored issue or guest essay scheduled for Day 0 | Founder A |
| -14 | Personal LinkedIn | Each founder DMs ~25 ex-Google peers: "We're launching Threadline in 2 weeks. Already 5 teams using it. Want a personal demo?" | Both |
| -7 | Reference quotes | Lock 3 design-partner reference quotes for landing page | Both |
| -3 | LinkedIn build-in-public | Long-form post: "We've been building Threadline for [N] months. Launch Tuesday. Here's what 5 design partners taught us." | Founder A |
| 0 (Tue 9am PT) | LinkedIn | Launch post from Founder A + Founder B — long-form, with 3 reference quotes, link to landing page | Both |
| 0 (Tue 10am PT) | Pragmatic Engineer | Sponsored issue / feature goes live | (scheduled) |
| 0 (Tue 11am PT) | Hacker News | Show HN post (one of the founders submits from their account; the other engages in comments) | Founder B |
| 0 (Tue 1pm PT) | Twitter/X | Thread linking to LinkedIn + HN; light, not primary | Founder A |
| 0 + 24hr | Personal email | Send personal "we're live" note to the 30-50 ex-Google peer list | Both |
| 0 + 2d | Engineering podcast appearance | First podcast guest spot (pre-booked, releases Day 2) | Founder A |
| 0 + 7d | Product Hunt | Soft launch (low priority — different audience) | Founder B |
| 0 + 14d | Lenny's Newsletter | Second sponsored issue or guest feature (different audience overlap) | Founder A |
| 0 + 21d | LeadDev / Software Engineering Daily | Second podcast appearance | Founder B |
| 0 + 30d | LinkedIn retrospective | "30 days post-launch: what worked, what didn't" — transparent metrics | Both |
| 0 + 60d | Pragmatic Engineer (3rd sponsorship) | Case study with named reference customer | Founder A |

**Risk callouts (per skill):**
- HN miss: NOT FATAL because HN is awareness-only and 3+ other channels are active simultaneously. The Pragmatic Engineer slot, LinkedIn warm-intro list, and reference customers are the real conversion engine.
- LinkedIn algorithm shift: low risk because founders have built warm-intro infrastructure independent of algorithm.
- Pragmatic Engineer pass: high impact if it happens — back up with Lenny's or Software Engineering Daily.
- All-on-warm-intros: scales slowly; need to start SEO + content compound in parallel for month 4+.

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing band

**Plan as written:** $40/seat/month, no free tier, 14-day trial.

**Required question:** Did the price BAND come from competitor anchoring, or from ICP willingness-to-pay evidence?

**Analysis:**
- Linear: $10 Basic, $16 Business. Notion: $0-15. Shortcut: $8.50-12. Plane: $5-10. Jira: $7-15.
- **Threadline at $40/seat is 2.5x-4x the direct-competitor band.**
- The doc provides NO ICP-willingness-to-pay evidence. No interviews, no adjacent-spend data, no benchmarking.
- The price is anchored on... what? Possibilities:
  - Founders' aspiration ("we'll be premium")
  - Borrowed from Superhuman-like prosumer pricing — but Superhuman is consumer, this is B2B
  - LinearB ($40-100+/seat range for engineering-metrics products) — possibly the anchor, but LinearB is METRICS, not PM
- For mid-market eng tools: adjacent-spend benchmarks include Datadog ($23-31/seat for APM), Honeycomb ($35-100/seat), GitHub Enterprise ($21/seat), Sentry ($26/seat), PagerDuty ($21-39/seat). $40 is at the HIGH end of this band but not unprecedented.
- **However:** all the comparables at $40+/seat are CRITICAL infrastructure (observability, incident, source control). PM is "important not critical." Buyers' willingness-to-pay for PM tools has historically capped around Linear's $16 band.

**Verdict on the band:**
- $40/seat is defensible IF AND ONLY IF Threadline delivers a category-defining wedge (e.g., "AI-driven sprint planning that demonstrably saves each engineer 5 hours/week" with case-study evidence). Without that wedge, $40 will be priced into oblivion vs Linear at $16.
- Without ICP-WTP evidence the band is GUESS, not strategy.
- **Recommendation: Run pricing-band validation with design-partner cohort BEFORE public launch.** Ask 5 design partners: "If this saved your team 20% on coordination overhead, what would you pay per seat?" Triangulate. The actual price might be $25, $40, $60, or $80 — but it should be evidence-based, not anchored.

**Specific anti-pattern to flag:** "We picked $40 because we want to be premium." This is the wrong direction of the anti-pattern from Section 6a (matching cheapest competitor) — overshooting WITHOUT the wedge produces the same problem from the opposite end: buyers conclude "overpriced and unproven" instead of "underpriced and commodity."

### 6b. Tier structure, trial mechanics, billing

**Strong recommendation — restructure as follows:**

**Free tier:** Yes. Cap at 10 users + N issues or N projects (TBD based on usage data). This is non-negotiable for the category and motion class per Step 0.5 M0b. Without it, no bottom-up adoption; without bottom-up adoption, no proven motion to first 100 paying customers.

**Pro/Team tier:** $25-35/seat (TBD via design-partner pricing validation). Annual billing only at this tier (15-20% retention boost). Targets 10-100 person engineering teams.

**Business tier:** $50-80/seat. SSO, audit logs, advanced admin, priority support. Targets 100-500 person engineering teams (THE STATED ICP). Annual only.

**Enterprise:** Custom (negotiated). 500+ engineers. Requires AE — out of scope for solo-founder phase.

**Trial mechanic:** Replace 14-day product trial with **design-partner program** (6 months free, founders concierge, reference rights in exchange). For inbound after launch: 30-day trial with extension on request (mid-market needs procurement runway).

**Annual discount:** 15-20% on annual billing. Document the retention evidence (annual-billing customers retain dramatically better — cite RevenueCat State of Subscription Apps or Vendr SaaS benchmarks in landing page).

**Per-seat vs per-feature:** Per-seat is correct for PM tools; matches buyer mental model and procurement norms. Don't get clever with usage-based for v1.

**Free-tier defense:** Yes, free tier means freeloaders. Cap the free tier hard enough that 50-500 person teams MUST upgrade (e.g., 10 users free, no SSO, no audit logs, no roll-up reports). The free tier is the funnel; the cap is the conversion mechanism.

**M0d revisited:** Replacing the 14-day trial with a design-partner program addresses the freebie-disqualifier finding. Cheap trial → wrong cohort. Design-partner concierge → right cohort. The trade-off: design-partner scales slower (manual founder time), but produces references the mid-market motion REQUIRES.

---

## Section 7 — Post-launch growth loops

**What compounds (if built):**
- **Team-invite virality (REQUIRES free tier):** User A invites teammates → team uses → org-wide expansion. This is the Linear/Notion/Slack motion. Cannot work without free tier per Section 6.
- **Reference customer flywheel:** First 5 reference customers → quoted in Pragmatic Engineer feature → next 20 mid-market evaluators see references → faster procurement → more references. Compounds over 12-18 months.
- **Content SEO compound:** Long-form "engineering manager's guide to X" content. 12-month ramp. By month 18, organic search drives 20-30% of inbound. Cite Linear, Notion, Ahrefs as proof.
- **Founder-as-channel compound:** LinkedIn audience accretes. By month 12, each founder has 3000-5000 followers in eng-leader segment if cadence holds. This is the long compound.

**What's linear (acquisition treadmill):**
- Paid sponsorships (Pragmatic Engineer, Lenny's): each one is a one-shot transaction; no compound effect
- Cold outreach: each outreach attempt is independent; doesn't compound
- Conference sponsorship: each event is independent

**Network effects within product (does it get better with more users?):**
- Modest — public templates, sharable workflows, integrations marketplace are weak network effects
- Strong if Threadline builds cross-org dependency tracking (one team's PRs visible to another team) — this becomes a true network effect within a multi-team customer
- WITHOUT free tier + team virality, the network effect inside the product is muted

**Retention as growth (word-of-mouth from happy customers):**
- High for PM tools historically — engineers move companies and bring tooling preferences. Linear benefited massively from this ("ex-Linear-user now at new co requests Linear")
- Threadline can play this loop IF retention is high (back to PMF gate)

**Strategic risk flag:** If the founders maintain "no free tier" + "no bottom-up motion," they cut off team-invite virality AND mute the within-product network effect AND lose the highest-compound loop (Linear's playbook). The remaining growth = linear (paid sponsorships + cold outreach + reference flywheel). This is an acquisition treadmill at $40/seat in a competitive category. **Not a winning long-game.**

---

## Section 8 — Metrics & instrumentation

**Measure:**

- **Acquisition by channel** (UTM-tagged everything): warm intros, Pragmatic Engineer sponsorship, LinkedIn organic, HN, podcasts, SEO
- **Cohort by company size** (THIS IS LOAD-BEARING per Step 0.5 M0d): trial signups segmented by stated team size. Watch for the wrong-cohort trap (10-25 person teams dominating signups while 50-500 ICP doesn't show up).
- **Activation rate** (definition: team of 3+ created ≥10 issues in first 7 days)
- **Day-7 / Day-30 retention** at team level (not user level — teams convert/churn)
- **Trial→paid conversion** segmented by cohort size
- **Time-to-first-revenue per cohort** (mid-market should be 60-120 days; if it's 14 days, you're closing the wrong segment)
- **Vohra "very disappointed" survey** monthly on active users → tracks PMF over time
- **Reference customer count** (how many will publicly endorse?)
- **NPS** per quarter
- **LTV / CAC** once enough data (probably month 6+)

**DON'T measure (vanity):**
- Twitter follower count (the ICP isn't there for the buyer persona)
- HN upvotes (well-known weak correlation with revenue; HN is awareness only)
- Total trial signups WITHOUT cohort segmentation (will mislead because wrong-cohort dominates)
- LinkedIn post reactions without click-through to landing page

**Dashboards (weekly):**
- Pipeline by company-size cohort (segmented)
- Channel attribution roll-up
- Design-partner health (concierge cohort retention, advocacy, Vohra score)
- Procurement-stage tracking for active mid-market deals (early/SOC 2 review/contract/closed)

---

## Section 9 — Risk analysis

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Motion-choice paralysis (sales-led or PLG?) | High | Catastrophic | Force the decision in week 1. Recommend PLG + free tier + bottom-up. Don't try both. |
| SOC 2 / SSO blocks mid-market procurement | Very High | High | Start SOC 2 Type I week 1. Build SSO before launch. Without these, $0 mid-market revenue for 12+ months. |
| Wrong-cohort validation (small teams trial, ICP doesn't) | Very High under 14-day trial mechanic | High (mis-tunes product) | Segment all metrics by cohort size; replace trial with design-partner program for ICP cohort. |
| Pricing band overshoot without wedge ($40 vs Linear $16) | High | High | Validate price with design partners BEFORE public launch; name the wedge or drop the price. |
| Show HN miss = no awareness | Medium | Medium | Multi-channel launch — Pragmatic Engineer + LinkedIn + podcasts independent of HN. |
| Channel concentration on Pragmatic Engineer | Medium | Medium | Diversify across Pragmatic Engineer, Lenny's, LeadDev, podcasts. No single channel >40% of inbound. |
| No founder content history → slow LinkedIn ramp | High | Medium | Accept the 6-12 month compound timeline; start NOW. Don't expect month-1 results. |
| Linear ships the feature Threadline differentiates on | Medium | High | Wedge needs to be something Linear is structurally unlikely to ship (e.g., AI features that would dilute Linear's "no AI bloat" brand; or cross-team coordination that Linear's "team is the unit" model resists) |
| Founders run out of runway before PMF gate | Medium-High | Catastrophic | Validate funding for 18-month bootstrap or raise. The bottom-up + content motion is patient capital. |
| "Better than Linear" positioning is too vague to convert | High | High | Name the wedge by Week 2. Pre-launch landing page must answer "why switch?" in one sentence with proof. |
| Calendar-gated launch fires with wrong-cohort cohort | Very High under current plan | High | Replace calendar gate with Vohra PMF gate + reference-customer threshold + procurement-readiness threshold. |
| Reddit / IndieHackers / Rands ban for self-promo | Medium if founders mistake these for launch channels | Medium | Don't use these as launch channels. Participate as humans only. |
| Founders' ex-Google warm-intro pool is smaller than assumed | Medium | High (it's the unfair advantage) | Quantify in Week 1. If <30 viable ICP contacts, the warm-intro channel is overrated and the gap needs another channel. |
| Macro: Linear acquired / Notion launches engineering PM tool | Low-Medium | High | Out of founder control. Plan for competitor-counter risk: defensible wedge + customer lock-in via integrations and references. |

---

## Outside-voice critique

Simulated outside-voice (independent marketing critique pass):

**1. Single biggest risk the inside review missed:**
The inside review correctly flags motion mismatch, pricing, procurement, and dogfood mismatch — but UNDERWEIGHTS the **founder skill mismatch risk**. Two ex-Google ICs with no B2B sales experience trying to run mid-market sales is the deeper problem; the marketing plan can be perfect and they'll still fumble the discovery calls, pricing negotiations, contract terms, and customer success required at $40/seat * 100-seat deals = $48K annual contracts. They either need to (a) explicitly choose PLG to minimize sales-conversation surface area, (b) hire/contract a fractional B2B sales leader by month 3, or (c) accept the founder learning curve eats 6-12 months of pipeline. The plan touches sales-vs-PLG choice tactically but doesn't surface "founder is not equipped for the motion they're choosing" as the existential risk.

**2. Channel weaker than positioned:**
The Pragmatic Engineer sponsorship is HIGH-VALUE but the inside review may overweight it. Single-sponsor placements in newsletters typically produce 100-500 click-throughs for B2B tools; conversion to paid for a $40/seat unfamiliar brand is 0.5-2%. Math: best case 500 clicks × 2% = 10 trial signups, of which maybe 1-2 mid-market deals close after 90 days. $5K-15K sponsor cost for 1-2 deals worth $48K each is acceptable economics BUT only if the founder follow-up game is sharp. The plan should add a "post-sponsorship attribution sprint" — manual outreach to every identifiable click-through in 48 hours.

**3. Audience-claim lacking evidence:**
"Ex-Google peer network = warm-intro channel = 30-50 ICP contacts." This is asserted but unverified. Ex-Google peers tend to cluster at OTHER FAANGs and big-tech post-Google, not at 50-500 person SaaS startups. The actual mid-market eng-leader overlap from 2 ex-Google ICs is probably 5-20 contacts, not 30-50. The plan should INSIST on quantification in Week 1 — if the real number is 5-10, the warm-intro channel is too thin to be the primary engine and the strategy shifts toward Pragmatic Engineer + content + cold outreach as the actual primary.

**4. Provocative reframe:**
**Threadline shouldn't be "Linear for engineering teams." Threadline should be "the layer ABOVE Linear/Jira for VP Eng-level visibility."** Stop competing with Linear on the same surface; instead, integrate with Linear AND Jira (and GitHub Projects), pull data up, and sell EM/VP-Eng rollup dashboards, cross-team dependency tracking, and exec reporting. This shifts:
- ICP: directly to VP Eng (the buyer), not the tech lead (the user) — eliminates the buyer/user mismatch
- Pricing: per VP Eng / per team-leader (lower seat count, higher per-seat price — $200/seat for 5-15 seats per company = $12K-36K ACV, healthier than $40 × hundreds-of-seats fight against Linear)
- Competitive moat: not "switch from Linear" (high friction); instead, "add a layer ON TOP of Linear" (zero switching cost, integration play)
- Wedge: clear and ownable — the rollup/cross-team coordination view that Linear structurally won't ship because it breaks Linear's "team is the unit" opinion
- Procurement: smaller ACV unlock, faster SOC 2 path, lower stakes mid-market sale

This is the kind of reframe the inside review's Step 0.5 was set up to surface but didn't get to. Worth a serious office-hours or CEO-review pass before committing to the "be Linear, only better" plan.

---

## Three strongest action items for THIS week

1. **Make the motion choice.** Sales-led mid-market (SOC 2, AE, 12-month cycles) OR product-led with free tier and bottom-up adoption. Write a 1-pager naming the choice and the consequences. Without this decision, every other tactical decision below is wrong-question optimization. **Recommended choice: PLG + free tier**, but the founders must own the decision explicitly.

2. **Quantify the ex-Google peer warm-intro pool.** Each founder lists every former Google peer who is now EM / TL / VP Eng at a 50-500 person SaaS company. Combined target: 30+ names. If actual is <15, the warm-intro channel is too thin and the strategy must shift (more Pragmatic Engineer budget, earlier content compound, fractional sales help). This number gates the whole distribution plan.

3. **Kick off SOC 2 Type I + SSO build.** Vanta or Drata, week 1 contract. SSO via Okta + Google Workspace, week 1 dev start. These are 3-4 month assets that have to start NOW because mid-market procurement DISQUALIFIES without them. Even in the PLG path, the conversion to paid mid-market teams requires both.

---

## Handoff

- Marketing plan written: this file.
- Launch playbook: `launch_playbook.md` (separate artifact).
- ICP spec: `icp.md` (separate artifact).
- Audience-build journal template: `audience_build_journal.md` (separate artifact).
- Recommend follow-up skills:
  - `/office-hours` — the "Threadline as layer-above-Linear" reframe from outside-voice critique deserves a full positioning session
  - `/plan-ceo-review` — the motion choice (PLG vs sales-led) is a business-model decision that needs CEO-mode review
  - `/plan-eng-review` — if PLG path chosen, the product needs free-tier mechanics + team-invite virality designed in
- Re-run this skill in 30 days to measure progress against the audience-build cadence and the three action items above.

