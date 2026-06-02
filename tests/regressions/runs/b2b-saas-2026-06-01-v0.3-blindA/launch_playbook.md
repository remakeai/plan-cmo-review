# Launch Playbook — Threadline

**Plan-cmo-review run:** v0.3-blindA, 2026-06-02
**Mode:** Mode A, Section 5 sequenced.
**Launch gate:** PMF-signal-driven, NOT calendar. See Section 5a of marketing_plan.md.

---

## Prerequisites BEFORE day 0 (non-negotiable)

Do not launch publicly until ALL of the following fire:

- [ ] **PMF gate:** ≥40% of paid design partners say "very disappointed" if Threadline went away (Vohra survey). Superhuman precedent: started at 22%, segmented, iterated to 47%. If <40%, iterate, do not launch.
- [ ] **Engagement gate:** ≥3 squads at ≥1 design partner use cross-squad view weekly for 4+ weeks.
- [ ] **Referral gate:** at least 2 design partners unprompted-introduce Threadline to a peer EM.
- [ ] **Case-study gate:** 2-3 paid design partners willing to be quoted/logoed publicly.
- [ ] **Anti-feature audit:** EM-facing surface (cross-squad rollup + OKR dashboard) shipped, not just the IC-facing Linear-style UI.
- [ ] **Pricing decision:** founders have explicitly chosen pricing path (A) $20-25/seat or (B) $40-50/seat mission-critical narrative. Not "split the difference."

If launch date arrives and gates have not fired, the launch date moves. Calendar gates are refused for this product class.

---

## Day -60 — Preparation

- Book Pragmatic Engineer **Podcast** sponsorship slot for launch week. (NEWSLETTER does not accept sponsors per blog.pragmaticengineer.com/sponsor; do not waste 2 weeks pitching it.)
- Submit pitch to Gergely Orosz for a guest essay on "Cross-squad coordination at mid-market scale: 4 lessons from 12 mid-market EMs." Editorial, not paid.
- Submit sponsor inquiry to Lenny's Newsletter (sponsor@lennysnewsletter.com per their about page).
- Begin booking podcast tour: Software Engineering Daily, Engineering Enablement, Lenny's Podcast pitch.
- Identify 5 LeadDev meetups in the next 90 days; commit to attending all 5.
- Build the 100-name personal-network list (founders' ex-Google contacts now EMs at mid-market cos).
- Build the 50-name cold-outreach list (mid-market SaaS EMs identifiable via public engineering blogs, conference speaker rosters, LinkedIn).

## Day -30 — Pre-announce + content

- Personal-network soft pre-announce email to the 100 warm contacts. Tone: "we're 60 days out, here's what we've built, please don't share publicly yet, would love feedback."
- Begin weekly LinkedIn content cadence from both founders (Maya-facing topics).
- Begin twice-weekly X build-in-public posts (Karri Saarinen's Linear playbook is the model — daily changelog, design decisions, screenshots).
- Begin Rands Slack helpful presence (answers, not posts).

## Day -14 — Build narrative

- Founders publish "What we built and why" long-form on LinkedIn. Buyer-facing (Maya POV), not IC-facing.
- Cross-post to Substack. Email to 50-person email list with personalized note.
- 1 podcast appearance airs (Software Engineering Daily ideal).

## Day -7 — Design-partner case studies

- Publish 2-3 design-partner case studies (logos visible) on Threadline blog.
- Pre-brief design partners that their case will be cited on launch day; ask them to RT/share.
- Cross-link case studies on LinkedIn from both founder accounts and from design-partner EM accounts (if willing).

## Day -3 — Build-in-public surge

- Twitter/X build-in-public thread series. 3 threads over 3 days. Each thread: a specific UX or architecture decision with a screenshot and a "here's what we tried, here's what didn't work, here's where it lands." Tag (tastefully) Karri Saarinen, Gergely Orosz, Lenny Rachitsky, Will Larson.
- LinkedIn echo of the same threads, EM-buyer reframed.

## Day 0 — Launch day

### 6:00 AM PT — Hacker News

**Show HN post title:** `Show HN: Threadline – cross-squad project tracking for engineering teams`

**Body (draft):**

> We built Threadline because Linear's per-team model breaks down past ~4 squads — cross-squad dependencies become invisible and weekly planning meetings balloon. Threadline adds a cross-squad dependency view + auto-generated OKR rollup on top of a Linear-style issue tracker.
>
> Architecture: [link to short architecture write-up]. The interesting bits are the dependency-graph diffing and the rollup query language.
>
> Where Threadline is worse than Linear: per-screen polish (Linear has years on us), keyboard shortcut coverage (we've matched ~60% of Linear's), and the mobile app (we don't have one yet — desktop + web only). Where Threadline is worse than Jira: ecosystem breadth (Atlassian Marketplace has thousands of integrations; we have ~15).
>
> GitHub: [link, even if private/closed-source link to docs repo or examples repo]
> Docs: [link]
> Pricing: [link to pricing page that reflects post-Section-6 decision]
>
> Happy to answer engineering, design, and pricing questions.

**Forbidden words in copy:** revolutionary, best-in-class, enterprise-grade, world-class, game-changing, seamless, robust, transforms, reimagines, next-generation.

### 6:00 AM PT — Email blast to personal network (100)

Personal note version: "We launched today on HN: [link]. If it resonates, an upvote helps; if it doesn't, your honest feedback helps more."

### 8:00 AM PT (HN +2h) — Twitter thread

Founder posts 8-tweet thread with HN link, screenshots, technical-spec lead. Cross-RT from cofounder account.

### 10:00 AM PT (HN +4h) — LinkedIn long-form

Buyer-facing framing. "Why we built Threadline: a 180-person SaaS company we worked with spent 90 minutes a week reconciling cross-squad dependencies in spreadsheets. Here's what we did about it."

Tag design-partner EM contacts (with permission). Ask them to share with their networks.

### 1:00 PM PT (HN +7h) — Pragmatic Engineer Podcast ad goes live

Confirm ad inventory aired; if applicable, request a one-line mention from host.

### Day 0 + 12h — Cold-outreach surge

Personalized emails to the 50-name cold list. Reference launch ("we launched today on HN, here's why I think this matters specifically for [their company's situation]"). NOT a mass blast — each email custom-tailored.

## Day 0 + 24h

- Rands Slack: brief, non-spammy mention IF community rules permit (most Slacks do not allow direct promotion; default to DMing specific EMs who'd find it relevant).
- r/ExperiencedDevs: cross-post with technical framing (NOT marketing framing).
- Lobste.rs submission (if invited / on-topic).

## Day 0 + 48h — r/programming + targeted subreddits

If HN momentum sustained, cross-post to r/programming. Otherwise skip — over-posting after a tepid HN reception amplifies the tepidity.

## Day 0 + 7d — Product Hunt

Separate launch event. Lower priority for this ICP (PH audience skews indie/PM, not eng leadership) but worth the freebie reach.

## Day 0 + 14d — Podcast tour airs

Software Engineering Daily, Engineering Enablement, others air. Cross-link from launch blog.

## Day 0 + 30d — Retrospective + case study

Publish "30 days post-launch: what we learned, real numbers" on Substack + LinkedIn. Include:
- Acquisition by channel (UTMs)
- Activation rate
- Conversion rate
- Vohra score on new cohort
- What surprised us

This compounds as content AND positions for the next wave of outreach.

---

## Risk callouts (specific to this playbook)

| Risk | Mitigation |
|---|---|
| HN miss (top of /new for <2h, <50 upvotes) | Pragmatic Engineer Podcast slot + design-partner case studies + cold-outreach surge are PARALLEL to HN, not dependent. The playbook continues regardless. |
| Show HN succeeds but converts only IC engineers, not EMs | Expected. Treat HN cohort as IC champion seed; EM conversion comes via the parallel cold-outreach + Lenny's sponsorship + LeadDev floor work. |
| Rands Slack mention gets the founders banned | Default to DMing specific people, not posting. Community has explicit rules against self-promo. |
| Cold outreach lands as spam | Each email is custom-tailored to the recipient's company and a specific public signal (blog post, conference talk, public engineering practice). NOT a mass blast. |
| Pragmatic Engineer Podcast doesn't have slot available in launch window | Move launch date OR sponsor closest substitute (Engineering Enablement, Software Engineering Daily) — do not skip the paid placement. |
| Vohra gate doesn't fire by day -7 | LAUNCH DATE MOVES. Do not ship publicly on calendar pressure. |

---

## "Don't do this" list (anti-patterns to refuse)

1. Don't lead with "$30M Series B from ex-Google founders." It's category-error signaling for this ICP — see ICP note on FAANG sensitivity.
2. Don't promise "AI-powered" anything in launch copy unless the product has a specific, demonstrable AI feature with measurable outcome.
3. Don't promise "10x your team's velocity." Specific, quantified outcomes only ("4 design partners saved an average of 35 minutes per cross-squad sync; here are their names with permission").
4. Don't price-match Linear in launch copy. Either undercut deliberately (path A) or premium-position deliberately (path B); the worst case is justifying $40 with "it's like Linear but better."
5. Don't post to all platforms simultaneously. The sequence above is calibrated to feed each channel's algorithm + audience.
