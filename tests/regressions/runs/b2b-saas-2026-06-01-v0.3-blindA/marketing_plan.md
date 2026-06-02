# Marketing Plan — Threadline (B2B SaaS, $40/seat, eng-team PM)

**Skill:** plan-cmo-review v0.3.0
**Fixture:** b2b-saas-2026-06-01
**Run:** v0.3-blindA
**Date:** 2026-06-02
**Mode:** Mode A — Full Marketing Review, with Section 4 (audience-build) ELEVATED to co-load-bearing alongside Section 5 (launch playbook). Tie-breaker per SKILL.md Step 0 activation rules: mid-build B2B SaaS, hard implied launch via "Show HN," founders have effectively zero ICP-aligned audience (200 X followers + 50 personal email subs, no professional content history). Mode C alone would skip the launch playbook the founders still intend to execute; Mode A with elevated Section 4 produces both.

---

## PREMISE-LEVEL FINDINGS BLOCK (load-bearing — read before tactical sections)

Working under marketing-naive default. Founders are 2 ex-Google engineers with no prior B2B sales experience, near-zero ICP-aligned audience, and a distribution plan that reads as a single-channel lottery ticket. Premise-challenge IS the highest-value output of this review. **4 of 5 Step 0.5 premises FAILED; 1 INCONCLUSIVE-leaning-FAIL.** Cascading implications are surfaced inline in each section.

| # | Premise | Verdict |
|---|---|---|
| M0a | "Show HN at launch" is the right audience class for engineering-management buyers at 50-500-person SaaS cos | **FAILS** — HN reaches IC engineers, not the budget-holder (VPE / EM). EMs at mid-market read Lenny / Pragmatic Engineer / LeadDev / Rands Slack, not HN. HN can seed bottoms-up adoption but is NOT a buyer-acquisition channel for $40/seat tooling. |
| M0b | Plan anchors against canonical-success comparable for design-led B2B at this motion class | **FAILS** — plan anchors only on "better than Linear." Linear IS the canonical success; the plan doesn't extract Linear's actual playbook (Karri Saarinen's design-led brand, invite-only early access, founder Twitter as primary surface, ~2 years of audience-build BEFORE general availability). Plan ignores the precedent it cites. |
| M0c | All in-scope features serve the paying ICP (engineering-manager budget-holder) | **FAILS** — "Linear-style project tracking" plus "engineering-specific workflows" implies IC-engineer-facing UI surface. The paying ICP is the EM/VPE, but the daily user is the IC. Without explicit EM-facing dashboards/rollups/digests, the product is anti-featured against the buyer. Also: no free tier + 14-day trial is internally consistent, but lack of any sub-team tier blocks the bottoms-up IC-champion motion that pairs with this ICP. |
| M0d | Acquisition-mechanic selection bias (14-day trial vs paying ICP) | **INCONCLUSIVE leaning FAIL** — 14-day no-CC-required trial selects for evaluators (often IC engineers exploring tools), not budget-holders. Mid-market EMs don't trial-shop $40/seat tools; they buy on referral or analyst signal. The trial mechanic IS the right shape for bottoms-up land-and-expand (Linear's playbook), BUT only if the product narrative + onboarding explicitly courts the IC champion who then escalates. Plan does not articulate this. |
| M0e | Dogfood audience-class match (ex-Google engineers building for mid-market 50-500 cos) | **FAILS** — Google engineering culture is the LEAST representative of the 50-500 SaaS-company engineering culture. Tooling, team size, planning rituals, on-call structure, deploy cadence, and authority gradients all differ sharply. Dogfooding on personal use OR on Google-shaped imagined workflows will tune the product for the wrong segment. Required fix per M0e: pivot BOTH the dogfood subjects (recruit 5 mid-market EMs to dogfood pre-launch) AND ensure marketing materials target the paying ICP (EM/VPE), not the IC engineer the founders identify with. |

**Single highest-value finding:** The plan combines a wrong launch platform (HN for non-HN buyer), no audience-precedent extraction (ignores Linear's actual playbook), an anti-feature gap (no EM-facing surface for the EM budget-holder), and a dogfood mismatch (Google culture ≠ mid-market culture). Each compounds the others. The validation gate ("5 paying companies by day 30") is structurally unreachable under this plan; the realistic worst case is 0 paying companies and a quiet HN post that the IC champions briefly try and abandon.

---

## Step 0A — Forcing-question answers (M1–M7)

### M1. Audience reality

Founders' naive answer: "engineering managers at mid-size SaaS companies who are frustrated with Jira and Linear."

**Refused.** Demographic category. Sharpened (composite ICP):

> *Maya, 34, Director of Engineering at a 180-person Series B SaaS company in NYC. Manages 4 squad leads / 28 engineers. Currently on Jira (inherited) + Linear (one squad piloted). Reads Lenny's Newsletter (paid), Pragmatic Engineer (paid), Software Engineering Daily (podcast on commute), Rands Leadership Slack (lurker, ~6000 members), LeadDev (attended LeadDev NYC 2025). Follows @gergelyorosz, @lennysan, @karrisaarinen on X. Spends ~$300/yr on her own professional development. Budget authority for tooling up to $5K/month without VP sign-off. Pain: weekly planning meetings run long because cross-squad dependencies are invisible in Linear; quarterly OKR rollups require manual spreadsheet work.*

Cascading: this ICP is NOT on HN. She is on Lenny's Newsletter sponsor slots, Pragmatic Engineer sponsor slots, LeadDev conference floor, and reads founder-written posts shared by people she follows.

### M2. Discovery path

Naive answer: "She sees my Show HN post."

**Refused.** Specific 3-step path:

1. A squad lead on Maya's team (IC engineer, lurks r/programming + HN) sees Threadline on HN, tries it on a side project, recommends it in a Slack DM to Maya: "this is what we should be using instead of Linear for cross-squad."
2. Maya sees the same product referenced in a Pragmatic Engineer paid issue (sponsored or organic mention) or in a Lenny's Newsletter "tools EMs use" roundup.
3. Maya books a 20-minute demo via an "EM-specific tour" CTA on the landing page (NOT "start free trial"), founder personally walks her through cross-squad dependency view + OKR rollup. Trial seeded with her real data during the call.

Time-to-discovery: 2-6 weeks from first IC exposure to EM demo. This is the actual mid-market B2B motion, not a viral consumer flip.

### M3. Pre-launch audience

200 X followers, ~50 personal email subs, no professional content history.

**This is effectively zero ICP-aligned audience.** Followers are likely friends + ex-Google network (some overlap with target IC engineers, near-zero overlap with mid-market EM budget-holders). Cascading: triggers Section 4 elevated status. The current audience cannot deliver 5 paying companies by day 30 under any realistic conversion assumption.

### M4. Channel honesty

Naive answer: "We're good at engineering blog posts."

**Refused.** No published writing track record. Honest answer: *"We don't have a credible distribution advantage yet. Ex-Google credential carries some signal among IC engineers (HN crowd) but limited signal with mid-market EMs who don't index on FAANG resumes."* First work item: build one. Candidate: technical blog post series on engineering-team coordination at mid-market scale, pitched to Pragmatic Engineer / LeadDev as guest pieces. Gergely Orosz syndication is the highest-leverage single channel for this ICP.

### M5. Competitor traffic source

Naive answer: "I don't know."

**Refused as terminal answer.** Pre-session assignment + actual research below in Section 1. Short version: Linear's primary traffic is direct + brand search (mature). Jira gets traffic via Atlassian's enormous SEO footprint + integrations marketplace. Shortcut gets traffic via SEO comparison pages + content. Height gets traffic via design-led founder presence + Product Hunt + Twitter. None of these primary channels are HN.

### M6. First 10 paying customers

Naive answer: "Founders' friends + HN cohort."

**Refused.** "HN cohort" is not a list. Sharpened: name the 10 people you would email tomorrow. Naive founders cannot name 10 mid-market EMs by name — that IS the problem. Real path:

- 3-5 warm intros from ex-Google network who are now EMs at mid-market SaaS cos (must enumerate)
- 3-5 cold outreach to EMs whose teams the founders have observed via public engineering blogs (Pinterest Eng, Notion Eng, Linear's own customer list, etc.)
- 2-3 from a Lenny's Newsletter / Pragmatic Engineer sponsored placement or guest post

If founders cannot enumerate 10 names within 1 week, that is the work-item before any launch.

### M7. Time allocation

Naive answer: "We're 90% on building until launch."

**Refused.** Ratio is wrong. Required: minimum 40% on audience-build + customer-development for the next 60-90 days, with named activities: 2 EM customer-development calls per week, 1 blog post per week on Maya-facing topics, weekly Rands Slack presence (helpful answers, not posts), 1 podcast pitch per week.

---

## Section 1 — Competitive landscape

### 1a. Direct competitors

| Product | URL | Founded | Pricing (USD) | Apparent traffic | Public complaints | Position vs Threadline | Winning? |
|---|---|---|---|---|---|---|---|
| Linear | linear.app | 2019 (exited private beta Jun 2020) | Free (250 issues, 2 teams), $8-10/user Standard, $14-16/user Business/Plus, Enterprise custom (reports $16-25/user); 20% annual discount [src: linear.app/pricing, comparetiers, vendr] | Direct + brand search; founder Twitter (Karri Saarinen, build-in-public daily changelog); polish-as-marketing; product-led; ~$400M reported valuation per Thoughtlytics writeup | "Too rigid for cross-team work"; "lacks reporting depth"; "no good portfolio view"; "weak Gantt / roadmap" | Threadline claims "better for engineering-specific workflows" — Linear's whole brand IS engineering-specific. Direct head-on collision. | Yes — category leader in design-led B2B PM. |
| Jira (Atlassian) | atlassian.com/software/jira | 2002 | Free (≤10 users), $7.91-8.15/user Standard, $14.54-16.00/user Premium, Enterprise quote-based (~$20-25/user) [src: atlassian.com/software/jira/pricing, costbench, ones.com]; volume discount drops avg to ~$6.82 at 500 users | Atlassian SEO juggernaut; marketplace; enterprise sales | "Bloated", "slow", "configuration hell" | Threadline competes on "not Jira" — crowded positioning; everyone does this | Yes by inertia; losing share at startup end, holding at enterprise |
| Shortcut | shortcut.com | 2014 (as Clubhouse; rebrand Sep 2021) | Starts ~$8.50/user [src: softwareadvice, getapp]; variable up to enterprise | SEO comparison pages, content, partnerships | "Lack of integrations with productboard/Notion"; "no AI/smart suggestions"; "smaller ecosystem" | Mid-market eng-focused; closest direct competitor to Threadline's stated positioning | Mid — steady but not breaking out |
| Height | height.app | 2018 | $6.99/user Team, $11.99/user Business | Design-led, founder Twitter (Michael Villar), Product Hunt | "Feature gaps vs Linear", "smaller community" | Adjacent — Height is more cross-functional, Threadline claims eng-specific | Mid — well-regarded but not dominant |
| Plane | plane.so | 2023 | Free OSS, paid cloud tier | GitHub (large star count for category), OSS community, dev-Twitter | "Less polished than Linear", "early" | Open-source alternative; different motion than Threadline | Growing — strong OSS pull |

**Honest assessment:** Linear is winning. Threadline's claim ("better than Linear for engineering-specific workflows") is the SAME claim Linear makes against Jira. Threadline needs a sharper, narrower wedge — not "better Linear" but "the thing Linear doesn't do for EMs at 50-500 cos." Candidate wedge: cross-squad dependency visibility + EM-facing rollups + on-call/incident-aware planning. Without a narrower wedge, Threadline is a feature, not a product.

### 1b. Canonical-success comparables (the part most plans skip)

Motion class: design-led B2B SaaS, bottoms-up adoption, $5-25/seat (sometimes higher with mission-critical positioning), sold to engineering orgs at mid-market.

| Canonical | Approx price | Founded | Scale (public reports) | Primary acquisition | Onboarding | Launch gate | Delta vs Threadline plan |
|---|---|---|---|---|---|---|---|
| Linear | $8-23/seat | 2019 (private beta started ~2019, exited Jun 2020) | ~$400M+ valuation per Thoughtlytics writeup; category leader | **Founder Twitter (Karri Saarinen) executing a daily build-in-public changelog strategy**, polish-as-marketing, term-of-art positioning ("issue tracking" filters out non-engineering buyers by design) | Self-serve + concierge for design partners early | **Invite-only private beta for ~12-18 months; waitlist grew to 10,000+ signups via founder build-in-public Twitter BEFORE public availability.** Took ~3 years before hiring their first marketer. PMF-signal + design-partner gate, NOT calendar. [src: First Round Review, Sequoia spotlight, Thoughtlytics] | Threadline plans calendar launch with no waitlist, no design-partner cohort, and no founder-brand surface. Linear's entire moat is the OPPOSITE of "Show HN on day N." |
| Notion | $10-15/seat | 2016 | Decacorn-scale valuation, very large user base | Community-led + template ecosystem + founder presence (Ivan Zhao); long beta; word-of-mouth | Self-serve + community templates | Multiple iterations + ~2 years of beta before breakout | Threadline has no community surface, no template/integration ecosystem story, and no founder narrative. |
| Vercel | $20/seat Pro | 2015 | $100M+ ARR, multi-billion valuation per 2024 reports | Developer relations (Lee Robinson et al), docs as marketing, OSS leadership (Next.js), conf sponsorship | Self-serve via OSS funnel | OSS adoption → paid conversion; gradual | Threadline has no OSS hook, no DevRel surface, and no docs-as-marketing motion. |
| Superhuman | $30/seat | 2014 | Acquired by Grammarly in 2025 (large multi-hundred-million headline figure widely reported) | Concierge + waitlist + Vohra "very disappointed" 40% gate; founder presence | **Manual concierge onboarding; founder personally onboarded early cohort** | **Vohra PMF score ≥40% "very disappointed" gates the next growth investment**; Superhuman started at 22%, segmented to the lovers, hit 33% then 47% [src: First Round Review, Business of Software, Coda public PMF doc] | Threadline plans no concierge cohort, no PMF gate, no manual founder onboarding. Calendar gate + self-serve trial is the opposite playbook. |

### 1c. Pattern surface

**What canonical successes share that Threadline's plan lacks:**

1. **Founder-as-distribution-surface** — Karri Saarinen, Ivan Zhao, Lee Robinson, Rahul Vohra. Each canonical success had a founder with public craft-narrative on Twitter/blog/talks BEFORE the product was for sale. Threadline founders are anonymous to the ICP.
2. **PMF-gated launch, not calendar-gated** — invite-only beta, design-partner cohort, Vohra 40% gate. Threadline has a calendar implied by "Show HN at launch + 5 paying companies by day 30."
3. **Concierge onboarding for first cohort** — Vohra explicitly, Linear via design-partner program. Threadline has self-serve 14-day trial.
4. **Long pre-launch audience-build** — Linear: ~2 years of invite-only; Notion: ~2 years; Vercel: years of Next.js OSS leadership before Vercel-the-product. Threadline has weeks.
5. **Narrow wedge, not "better than X"** — Linear was "the issue tracker that respects your taste," not "better Jira." Threadline currently is "better Linear" — a feature, not a wedge.

**Which pattern is Threadline implicitly following?** None. The plan is closest to a generic "build then Show HN" indie-dev launch playbook, which is the wrong motion class for $40/seat B2B SaaS sold to engineering management at mid-market.

---

## Section 2 — ICP specification

See `icp.md` (separate artifact).

Headline: **Maya, Director of Engineering at a 180-person Series B SaaS in NYC/SF**. NOT IC engineers; NOT VPEs at 1000+ cos; NOT startup founders at 10-person cos. The narrow band is mid-market SaaS with 4-8 engineering squads where cross-squad coordination is the documented pain.

Critical correction from M0e: founders MUST recruit 3-5 EMs in this profile for paid dogfood/design-partnership BEFORE further build. Building on Google-shaped intuition for 6 more months ships the wrong product.

---

## Section 3 — Distribution channel-by-channel

### Channel table (Threadline-specific scoring, 1-5)

| Channel | Reach (1-5) | Cost | Conv | Founder fit | Effort | Verdict |
|---|---|---|---|---|---|---|
| **Show HN** | 4 (if hits) | Low | 1 for buyer / 3 for IC champion | 2 (no rep) | Low | KEEP as awareness + IC champion seeding, NOT as customer acquisition |
| **Pragmatic Engineer NEWSLETTER sponsorship** | n/a | n/a | n/a | n/a | n/a | **NOT AVAILABLE** — newsletter (>1M readers per pragmaticengineer.com/about) does NOT accept sponsorships, partnerships, or affiliates (creator policy, blog.pragmaticengineer.com/sponsor). Plan around this. |
| **Pragmatic Engineer PODCAST sponsorship** | 3-4 (large eng-leadership listenership) | $$$ | 4 | 5 (audience-perfect) | Low | TOP PRIORITY — this is the ONLY paid surface in the Pragmatic Engineer orbit |
| **Pragmatic Engineer guest content / Gergely Orosz mention (organic)** | 4 | Free (editorial) | 5 | 5 | High (need to earn it) | TOP PRIORITY — pitch a deeply-researched piece; Gergely-organic mention is the highest-signal surface for this ICP and the only free path into the newsletter audience |
| **Lenny's Newsletter / Podcast sponsorship** | 4 (377K+ free subs, 18K+ paid per growthinreverse.com; PM-heavy with EM overlap) | $$$ (not publicly disclosed; "not cheap") | 3 | 3 (PM-skewed) | Low | Tier 2 |
| **LeadDev conference / sponsorship** | 3 (in-person EMs, high intent) | $$ ($10-25K booth) | 4 | 4 (audience-perfect) | Medium | TOP PRIORITY |
| **Rands Leadership Slack** | 3 (~6K+ EMs) | Free | 4 (if non-spammy) | 3 (must build rep first) | High (months of helpful presence) | Long-build, start now |
| **Software Engineering Daily podcast guesting** | 3 | Free | 3 | 3 (need narrative) | Medium | Tier 2 |
| **Engineering blog (own) + SEO** | 3 (compounds) | Low | 3 | 3 (no track record yet) | High (6-12 mo ramp) | Start now, payoff Q3-Q4 |
| **Show HN follow-up — Lobsters, r/ExperiencedDevs** | 2-3 | Low | 2 | 2 | Low | Auxiliary |
| **Twitter/X organic** | 2 (no audience) | Free | 2 | 2 | Medium | Build slowly; not a launch channel |
| **LinkedIn (founders + company)** | 3 (EMs lurk here) | Free | 3 | 3 | Medium | Underrated for B2B EM buyers |
| **Cold outreach (EM-to-EM)** | 2 | Free | 4 (high signal) | 3 | High | Mandatory for first 10 customers |
| **Product Hunt** | 2 (PH crowd skews indie/PM, not eng mgmt) | Free | 1 | 2 | Low | Skip or auxiliary |
| **Paid Google ads ("Linear alternative")** | 2 | $$ | 2 | 3 | Medium | Defer until post-PMF |

### Motion-class rules applied (B2B SaaS mid-market — per SKILL.md Section 3)

- Pragmatic Engineer, Lenny's Newsletter, LeadDev, Rands Slack, Software Engineering Daily are the named vertical surfaces. They are PRIMARY, not auxiliary.
- HN is NOT primary for budget-holder acquisition; it is auxiliary for IC champion seeding (which can then bubble up).
- Dev-tool tonal rule applies partially — IC engineers will read the HN post and the docs. Marketing-speak in launch copy will tank IC trust, which kills the champion-bubble-up path. Refuse superlatives in launch copy: no "best-in-class engineering project tracking," no "enterprise-grade workflows," no "seamless." Lead with concrete architecture/UX decisions and honest "this is worse than Linear at X" comparisons.

### Three prioritized channels (forced cut)

1. **Pragmatic Engineer ecosystem (editorial-first)** — earn an organic Gergely Orosz mention via a deeply-researched piece on cross-squad coordination at mid-market scale; pitch the Pragmatic Engineer Podcast for a paid sponsorship slot. NOTE: the newsletter itself does NOT take sponsorships — many founder marketing plans assume it does and burn time on a dead-end pitch.
2. **EM-to-EM cold outreach + Rands Slack helpful presence + LeadDev conference floor** — direct path to first 10 customers; high-trust segment-matched.
3. **Show HN + founders' technical blog for IC champion seeding** — feeds bottoms-up adoption; supports #1 and #2.

---

## Section 4 — Pre-launch audience-build (ELEVATED — load-bearing)

See `audience_build_journal.md` for 30/60/90 detail. Headline cadence:

### Days 1-30 (NOW — June 2026)

- **Customer dev:** 2 EM interviews/week (16 total). Recruit via warm intros + LinkedIn cold + Rands Slack. Topic: cross-squad coordination pain, current tooling stack, willingness-to-pay anchors.
- **Content:** 1 founder-bylined post per week (4 total) on Maya-facing topics. Examples: "Why cross-squad planning breaks at 100 engineers," "OKR rollups in Linear: what we built when it didn't work," "On-call-aware sprint planning." Cross-post to LinkedIn + Substack + cohost on personal X.
- **Community:** weekly helpful Rands Slack presence (answers, NOT posts). One LeadDev meetup attendance.
- **Outreach:** pitch 1 podcast/week (Software Engineering Daily, Pragmatic Engineer pod, Lenny's, Engineering Enablement).
- **Design partners:** lock 3-5 paid design partners ($1-3K/yr commitment) from interview cohort by day 30.

### Days 31-60

- Scale content to 2 posts/week if engagement signal positive (>100 LinkedIn reactions or >5 inbound DMs/post).
- Begin Pragmatic Engineer sponsorship conversation (slots typically book weeks ahead).
- First podcast appearances air.
- Design partners using product weekly; founders manually onboard.

### Days 61-90

- Pragmatic Engineer sponsorship lives.
- First public case study from design partner.
- Begin formal launch sequence (see Section 5).
- Vohra "very disappointed" survey to design partners — if <40%, do NOT launch publicly; iterate.

---

## Section 5 — Launch playbook

### 5a. Question the launch gate FIRST

Founders' plan: calendar gate ("Show HN at launch, 5 paying companies by day 30").

**Refused.** Threadline is retention-driven B2B SaaS. The right gate is PMF-signal-driven:

- **Vohra 40% gate**: ≥40% of design partners say "very disappointed" if Threadline went away. If <40%, the public launch ships a product that won't retain — guaranteed validation-gate failure.
- **Cross-squad dependency engagement threshold**: ≥3 squads at ≥1 design-partner company use cross-squad view weekly for 4+ weeks.
- **Unprompted referral**: at least 2 design partners introduce Threadline to a peer EM unprompted.

If these gates fire by day 60-90, launch. If they don't, the product is not yet indispensable; launching publicly burns the first-impression budget. The "5 paying companies by day 30" gate should be REPLACED with "5 paid design partners by day 30 + Vohra ≥40% by day 60 + 10 paying companies by day 120." Linear's playbook (~2 year beta) is the precedent; matching even 10% of that discipline (60-90 day gated beta) is the floor.

### 5b. Sequenced launch (assuming PMF gate fires ~day 90)

See `launch_playbook.md` for hour-by-hour. Headline sequence:

| Day | Channel | Action |
|---|---|---|
| -60 | Pragmatic Engineer Podcast | Book sponsorship slot for launch week (newsletter does not take sponsors; podcast does) + parallel pitch a guest essay to Gergely |
| -30 | Personal network | Soft pre-announce email to ~100 ex-Google + warm contacts |
| -14 | LinkedIn | Founders post "what we've built and why" (Maya-facing framing) |
| -7 | Design partners | Public case study from 2-3 paid design partners (logos visible) |
| -3 | Twitter/X | Build-in-public thread series; tag Karri Saarinen, Gergely Orosz, Lenny tastefully |
| 0 AM PT | Hacker News | Show HN: "Threadline – cross-squad project tracking for engineering teams" — code-first, link GitHub examples, name where it's WORSE than Linear |
| 0 + 2h | Twitter | Thread with HN link, technical-spec lead, screenshots |
| 0 + 4h | LinkedIn | Long-form founder post — buyer-facing framing (Maya's POV) |
| 0 + 24h | Rands Slack | Brief, non-spammy mention IF community rules permit; otherwise DM specific people who'd find it useful |
| 0 + 24h | r/ExperiencedDevs | Cross-post with appropriate framing |
| Launch week | Pragmatic Engineer | Sponsored placement runs |
| 0 + 7d | Product Hunt | Separate event (lower priority for this ICP) |
| 0 + 14d | Podcast tour | Software Engineering Daily, Engineering Enablement appearances air |
| 0 + 30d | Retrospective post | Cross-post on LinkedIn + Substack with traction numbers |

### Dev-tool tonal rules applied (load-bearing)

Refuse from launch copy:
- "Revolutionary," "best-in-class," "enterprise-grade," "world-class," "game-changing," "seamless," "robust."
- Generic benefit-led hero: "Threadline transforms how engineering teams collaborate."

Recommend:
- "Threadline is a project tracker we built because Linear's cross-squad model breaks past ~4 squads. Here's the architecture, here's where it's worse than Linear, here's the GitHub: [link]."
- Honest "we lose at": Linear's polish per-screen, Jira's ecosystem breadth, Shortcut's pricing.

### Risk callouts

- HN miss → no recovery if it's the only channel → mitigated by Pragmatic Engineer + design-partner case studies + pre-built personal network email.
- Pragmatic Engineer sponsorship under-converts → mitigated by parallel direct outreach to 50 named EMs that week.
- Design-partner case study has no proof points → if PMF gate didn't fire, DO NOT LAUNCH; iterate.

---

## Section 6 — Pricing & packaging

### 6a. Question the pricing BAND first

$40/seat/month is anchored where? Founders presumably reasoned: "Linear is $14-23, we're premium, so $40." That's BAND-FROM-COMPETITOR thinking.

**ICP willingness-to-pay evidence to gather:**

- What does Maya already pay per seat for tooling? Linear $14-23, Jira $13.53, GitHub Enterprise $21/user, PagerDuty $21-41/user, Datadog $15-23/host, Notion $15-18/seat. The eng-team tooling band at mid-market sits $15-25/seat for most categories, $20-40/seat for specialized/critical tools.
- $40/seat is at the TOP of the band — closer to Datadog or PagerDuty (mission-critical) than to Linear (preference-driven). The pricing implies a mission-critical positioning. Does the product narrative justify mission-critical positioning? Currently: no. The narrative is "better Linear."
- **Specific failure mode flag:** $40 is neither cheapest nor anchored on documented WTP. It's a vibes-premium over Linear. Two coherent alternatives:
  - **(A) Anchor at $20-25/seat** with strong free tier for <10-seat teams (matches Linear/Shortcut band, makes IC champion → EM expansion frictionless, sacrifices margin for adoption).
  - **(B) Anchor at $40-50/seat** with mission-critical narrative (cross-squad dependency = production-incident-prevention, OKR rollup = exec-reporting-replacement). This requires the narrative to back the price.

Founders should explicitly pick (A) or (B), not split the difference. $40/seat with "better Linear" positioning is the worst of both.

### 6b. Standard pricing coverage

- **Tier structure:** missing. Single $40 seat with no free tier and no team/enterprise tier leaves money + adoption friction on the table. Recommend: free for <5 seats (IC champion seeding), $40/seat for 5-50 seats, contact-sales for 50+ (enterprise SSO, audit log, dedicated support).
- **Trial mechanics:** 14-day no-CC is fine for IC champion seeding (bottoms-up). For the EM buyer specifically, also offer "EM Demo" CTA (concierge, founder-led 30-min) — different mechanic for different segment.
- **Annual discount:** strongly recommend. Annual billing is broadly documented (e.g., RevenueCat State of Subscription Apps) to improve retention meaningfully at this band. Default to 15-20% annual discount.
- **Per-seat is correct model** for this category; consider per-squad add-ons later (cross-squad dependency module, OKR rollup module) if value-based pricing supports.

---

## Section 7 — Post-launch growth loops

- **Referral mechanics:** in-product invite for cross-squad workflows is natural (you literally can't use cross-squad without inviting other squads). High loop potential — design this in v1, not v2.
- **Content compounding:** founder blog + Pragmatic Engineer ecosystem syndication compounds over 6-18 months. Real.
- **Network effects:** within an org, yes (cross-squad gets more useful as squads adopt). Between orgs, no (no marketplace, no shared content).
- **Brand compounding:** weak today (no founder brand). Building it is Section 4's job. Realistic 12-24 month build.
- **Retention as growth:** strong potential IF the cross-squad wedge is real. Maya recommending Threadline to peer EMs at LeadDev is the realistic engine. Requires PMF gate to fire first.

If PMF gate doesn't fire, none of these loops engage and Threadline becomes acquisition-treadmill. Acknowledged risk.

---

## Section 8 — Metrics & instrumentation

Measure:
- Acquisition by channel (UTMs on every link, including podcast show-notes)
- Activation: % of trial accounts that invite ≥2 other squad-members within 7 days (cross-squad wedge engagement)
- Day-7 / Day-30 retention by cohort
- Trial → paid conversion (segment by IC-champion vs EM-direct)
- Cohort LTV by acquisition channel (Pragmatic Engineer cohort vs HN cohort vs cold-outreach cohort) — this will decide budget allocation
- Vohra "very disappointed" score, monthly, on active users
- Unprompted referral count

Do NOT measure (vanity):
- HN upvotes (correlation with revenue near zero for B2B SaaS)
- X follower count
- Total signups without activation

Dashboards: weekly funnel review; monthly cohort review.

---

## Section 9 — Risk analysis

| Risk | Severity | Mitigation |
|---|---|---|
| Channel concentration on HN if it lands | High | Section 5 sequence forces 3+ channels; Pragmatic Engineer sponsorship is parallel to HN, not dependent on it |
| Channel concentration on Pragmatic Engineer if HN misses | Medium | Direct outreach to 50 named EMs parallel; LeadDev presence; founder blog compounding |
| Founders have no name recognition with ICP | High | Section 4 is the mitigation — build founder narrative on Maya-facing topics over 60-90 days |
| Product anti-featured for EM buyer (Linear-style UI is IC-facing) | High | Add EM-facing surface (cross-squad rollup, OKR dashboard) BEFORE launch; this is a Section 4 + product spec issue |
| Pricing-band mismatch ($40 with "better Linear" narrative) | High | Pick (A) or (B) in Section 6a; do not split |
| Calendar launch gate fires before PMF | Critical | Replace with Vohra ≥40% gate; defer public launch if gate doesn't fire |
| Dogfood mismatch (Google culture ≠ mid-market) | High | M0e mandate: paid design partners at mid-market cos dogfood for 60-90 days BEFORE launch |
| Linear counter-launches or feature-copies cross-squad wedge | Medium | Defensible only via tighter wedge + ICP relationship; speed-to-market matters less than relationship depth |
| Ex-Google founders interpret early HN traction as PMF | High | Discipline: only Vohra gate + paid design-partner retention counts; HN upvotes do NOT count |
| Validation gate (5 paying / day 30) becomes panic gate | High | Replace with "5 paid design partners / day 30 + Vohra ≥40% / day 60 + 10 paying / day 120" |

---

## Outside-voice critique (simulated subagent pass)

Independent reviewer findings:

1. **Biggest missed risk:** The plan treats Linear as competitor when Linear is, more importantly, the SUBSTITUTE the ICP already has. Maya is not unhappy with Linear — she's mildly inconvenienced. "Mildly inconvenienced" is not a buying trigger for $40/seat tooling. Threadline needs to find an ICP for whom Linear is ACTIVELY FAILING, not just suboptimal. Candidate: post-merger eng orgs combining two tracking systems; orgs scaling past Linear's hierarchy model (>8 squads); orgs with regulated change-management needs Linear doesn't serve.
2. **Channel weakness:** Plan initially over-indexed on "Pragmatic Engineer sponsorship" before verifying availability. Live web check: the Pragmatic Engineer NEWSLETTER does not accept sponsorships at all (creator policy, blog.pragmaticengineer.com/sponsor); only the podcast does. Founder marketing plans routinely assume the newsletter is buyable and waste weeks pitching. Real plays: (a) pitch the podcast slot, (b) earn an editorial mention by writing the deeply-researched mid-market-coordination piece Gergely would want to link to, (c) sponsor Lenny's Newsletter as the closest substitute reach for the EM-adjacent buyer.
3. **Audience claim lacking evidence:** Founders claim ex-Google credential helps. With IC engineers maybe; with mid-market EMs at 50-500 cos, ex-FAANG can ACTIVELY HURT (perceived as out-of-touch with mid-market resource constraints). Test the assumption in interviews; consider de-emphasizing FAANG narrative.
4. **Provocative reframe:** What if Threadline is not a Linear replacement but a Linear/Jira COMPLEMENT — the cross-squad / OKR-rollup layer that sits ON TOP of Linear and Jira, both? This collapses the "we have to win against Linear" problem into "we make Linear better for the EM who already chose Linear." Different positioning, different pricing power, different channels (integration partners), much lower switching cost. Worth a 1-day exploration before committing to head-on Linear positioning.

Update plan: incorporate (1), (2), (4) as design decisions to revisit; (3) as customer-dev question.

---

## Top 3 action items for THIS week

1. **Recruit 5 mid-market (50-500-person SaaS) EMs as paid design partners** ($1-3K/yr commitment each). Cold outreach via LinkedIn + warm intro via ex-Google network. Target: 5 contracts signed by day 30. THIS IS THE LOAD-BEARING PRE-LAUNCH WORK.
2. **Replace "5 paying companies by day 30" validation gate** with "5 paid design partners by day 30 + Vohra ≥40% by day 60 + 10 paying by day 120." Communicate the change to anyone who'd hold founders accountable.
3. **Begin Maya-facing content cadence**: 1 founder-bylined post this week on a cross-squad coordination topic; publish to LinkedIn + Substack; share with 3 named EMs for feedback. This week, not "after launch."

---

## Handoff

- Artifacts in this directory: `marketing_plan.md` (this file), `icp.md`, `launch_playbook.md`, `audience_build_journal.md`, `web_search_log.md`.
- Self-check: re-run plan-cmo-review on day 30 to evaluate progress against this plan.
- Follow-up skills recommended: `/plan-ceo-review` to revisit pricing-band decision (Section 6a) and "complement vs replace Linear" reframe (outside voice #4); `/plan-eng-review` to scope EM-facing surface (cross-squad rollup + OKR dashboard) as load-bearing v1 features.
