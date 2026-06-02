# Threadline — ICP Specification

**Companion to `marketing_plan.md` Section 2.** Tightened from the design doc's three-roles-in-one ICP.

## Buyer/User split (this was collapsed in the design doc)

| Role | Persona | Function in deal |
|---|---|---|
| BUYER | Priya — VP Engineering | Approves budget, owns tooling decision, signs contract |
| USER (advocate) | Marcus — Senior Engineer / Tech Lead | Discovers, evaluates, recommends upward |
| INFLUENCER | EM (Marcus's manager) | Bridges Marcus and Priya; validates value before Priya time |
| GATEKEEPER | IT / Security / Procurement | SOC 2 review, SSO config, vendor risk assessment |

## Primary BUYER persona — Priya

### Demographics
- Title: VP Engineering
- Company stage: Series B/C SaaS, 100-300 person headcount (sweet spot for Threadline's ICP)
- Vertical: Fintech, DevTools, Vertical SaaS, B2B platform. NOT marketplaces or consumer-app cos (different PM needs).
- Experience: 10-15 years; former TL at a FAANG or top-tier startup; promoted to EM, then manager-of-managers
- Direct reports: 3-6 EMs / 25-60 engineers total
- Reports to: CTO
- Budget authority: $50K-$300K/year tooling budget; full authority for <$50K annual contracts; CFO/IT routes for >$50K

### Attention surfaces (where she is RIGHT NOW)
1. The Pragmatic Engineer (paid subscriber — actively reads weekly)
2. Engineering Enablement Podcast / The Pragmatic Engineer Podcast
3. LeadDev conferences (annually); LeadDev newsletter
4. Private VP Eng peers Slack (30-80 senior eng leaders, invite-only)
5. LinkedIn — reads/comments on Gergely Orosz, Will Larson, Charity Majors, Camille Fournier
6. Twitter/X — light usage, mostly tech-leader thread reading
7. Books: "The Manager's Path," "An Elegant Puzzle," "Staff Engineer"

### Adjacent-category spend (annual)
- PM tool (Linear / Jira / Shortcut): $10-15/seat × ~30-60 engineers = $4K-$10K
- Observability (Datadog / Honeycomb): $25-100/seat × eng team = $20K-$60K
- Source control (GitHub Enterprise): $21/seat = $7K-$15K
- Incident management (PagerDuty / Incident.io): $20-40/seat = $5K-$15K
- Personal subs: Pragmatic Engineer ($150/yr), Lenny's Newsletter ($150/yr) — often expensed

### Top complaints about current PM tool
- **Linear users:** "Beautiful but doesn't scale to multi-team cross-dependency tracking. We hack it with cycle-prefixes and labels."
- **Jira users:** "Bloated. Slow. Workflow config takes a quarter. Performance is bad on big projects."
- **Shortcut users:** "Less polished than Linear, fewer integrations, feels stuck."
- **GitHub Projects users:** "Lightweight; doesn't replace a real PM tool."

### Objections to Threadline
1. "Why switch? Linear works. Switching cost = 2 months of team friction."
2. "$40/seat is 4x Linear. What's the value justification?"
3. "SOC 2? SSO? Audit logs? Data residency? If no on any, can't even start a procurement conversation."
4. "Who else my size uses you? Show me 3 references at 100-300 person SaaS cos."
5. "2 founders, no funding stated. Will you be around in 3 years?"
6. "Where's the AI feature that justifies the premium?"

### Conversion triggers
1. Specific workflow gap in Linear/Jira that Threadline solves natively, with named reference customer
2. Trusted peer recommendation from her VP Eng Slack
3. Pragmatic Engineer / Lenny's feature with case study
4. Design-partner program: 6 months free + concierge founder onboarding + reference rights
5. Clear procurement-ready posture (SOC 2 Type I done, Type II in progress, SSO live, audit logs available)

## Secondary USER persona — Marcus

### Demographics
- Title: Senior Engineer / Tech Lead / Staff Engineer
- Reports to: EM (who reports to Priya)
- Leads: 5-8 person sub-team within a larger eng org
- Experience: 6-10 years; respected operator; sets up team tooling

### Attention surfaces
1. Hacker News — daily front page + Show HN scan
2. The Pragmatic Engineer (free tier or paid)
3. GitHub trending; lobste.rs
4. Bluesky for tech
5. Internal company Slack (#engineering channels)
6. Conference talks (KubeCon, RailsConf, vertical conferences)

### Conversion role
Marcus discovers tools, runs side-project trials, becomes internal advocate. Does NOT have budget authority. Does influence purchase via:
- Demo to his EM ("hey, this would solve our X problem")
- Slack message in #engineering ("we should try this")
- Direct ask to Priya in next 1:1 ("we should evaluate Threadline")

**Marcus is reachable via HN, Bluesky, lobste.rs, GitHub, technical content. Priya is not reachable via those channels.**

## Decider chain (mid-market deal flow)

```
Marcus discovers (HN / GitHub / peer recommendation)
  ↓
Marcus signs up (REQUIRES free tier or generous trial — 14 days too short)
  ↓
Marcus uses on side-project / small team for 2-4 weeks
  ↓
Marcus advocates to EM (informal demo, Slack message)
  ↓
EM evaluates with team — needs roll-up reporting, multi-team views
  ↓
EM presents to Priya in next 1:1 / staff meeting
  ↓
Priya requests evaluation — asks for references, security posture, pricing
  ↓
Procurement runs SOC 2 / SSO / vendor risk review (4-8 weeks)
  ↓
Contract signed (annual, per-seat × team size)
  ↓
Roll out to broader org
```

**Time from Marcus discovery to first $: 60-120 days for mid-market. NOT 30.**

## Anti-personas (who Threadline should NOT chase in Year 1)

- **Solo developers / pre-seed (2-5 person) startup teams** — they trial heavily, won't pay $40/seat, mistune the product to small-team needs
- **Enterprise (1000+ engineers)** — 6-12 month procurement cycle, requires AE + CSM, out of solo-founder scope
- **Non-engineering teams (marketing / design / ops)** — different positioning, dilutes wedge
- **Open-source / cost-sensitive teams** — Plane is the alternative, not Threadline
- **Heavy Atlassian-ecosystem cos (using Confluence + Bitbucket + Jira deeply)** — switching cost is prohibitive; ignore until Year 2

## Cohort segmentation (load-bearing for metrics)

Every metric in Section 8 must segment by company size:
- 1-10 person teams (anti-persona)
- 11-49 person teams (early-adopter, weak fit, allow but don't optimize)
- 50-100 person teams (ICP edge — accept and pursue)
- 100-300 person teams (ICP sweet spot — pursue actively)
- 300-500 person teams (ICP top end — pursue actively)
- 500+ person teams (enterprise — out of scope Year 1)

If trial signups concentrate in 1-10 cohort, the marketing IS attracting wrong segment. The validation signal is theater.
