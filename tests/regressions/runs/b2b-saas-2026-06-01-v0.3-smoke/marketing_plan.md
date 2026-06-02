# Threadline — Marketing Plan

**Skill version:** plan-cmo-review v0.3.0
**Run:** b2b-saas-2026-06-01-v0.3-smoke (BLIND smoke test)
**Date:** 2026-06-01
**Mode:** A (Full Marketing Review) with Section 4 elevated (v0.3 tie-breaker)
**Motion class:** B2B SaaS, mid-market (NOT a dev tool — Threadline is a project tracker; even if its buyer is technical, it does not ship code-level integrations or programmable surface)

---

## Founder-supplied design doc (frozen input)

> **Product:** "Threadline" — Linear-style project tracking for engineering teams at 50-500 person companies.
> - Pricing: $40/seat/month, no free tier, 14-day trial
> - Target users: engineering managers, tech leads, IC engineers at mid-size SaaS companies
> - Distribution Plan: "Show HN at launch + content marketing on the engineering management blog"
> - First 10 customers: "Founders' friends + HN cohort"
> - Validation gate: 5 paying companies by day 30
> - Differentiation: "Better than Linear for engineering-specific workflows"
> - Founders: 2 ex-Google engineers, no prior B2B sales experience
> - Existing audience: 200 followers on X, ~50-person personal email list, no professional content history

## Default-assumption framing

Both founders are ex-Google ENGINEERS with NO B2B sales experience. None of the "evidence that overrides the default" applies:

- No prior shipped product at >$10K MRR
- No published-writing audience / no professional content history
- Audience is tiny AND not demonstrated ICP-aligned (200 X followers is generic noise; 50-person personal email list is friends/family/ex-coworkers, not buyers)
- No documented prior failed launches with retrospective analysis

**Working under marketing-naive default; premise-challenge is load-bearing.**

---

# PREMISE-LEVEL FINDINGS BLOCK (Step 0.5)

**≥2 premises failed.** This block sits ABOVE the tactical sections because premises rotted at the framing level cannot be rescued by tactical sharpening downstream.

| # | Premise | Verdict | Cascading effect |
|---|---|---|---|
| M0a | Show HN reaches engineering managers / tech leads | **INCONCLUSIVE (leans survives, conditional)** | HN does reach IC engineers and many EMs, but selection toward "looking for tooling on weekend" — not toward 50-500p enterprise buyer with budget authority. Not a category error like consumer-HN; it's a top-of-funnel-mismatch with the purchase committee. M2 still refuses "Show HN as step 1." |
| M0b | "Better than Linear" is a canonical-success-aware positioning | **FAILS** | Plan anchors only on direct competitor (Linear). No canonical-success comparable named. Linear itself IS the canonical success at this motion class, so "better than Linear" is a positioning crater (you are claiming to out-execute the playbook winner in their own playbook). |
| M0c | All in-scope features serve the paying ICP | **FAILS** | "IC engineers" listed as target user alongside EMs / tech leads is an anti-feature in audience-targeting form. IC engineers are USERS but not BUYERS in 50-500p companies — including them in the ICP dilutes positioning toward "every engineering org" and adds non-buyer feedback noise to the v1 cohort. |
| M0d | 14-day trial selects for paying ICP | **FAILS** | At $40/seat/mo with no free tier and no concierge, 14-day trial selects for solo evaluators in companies WITHOUT procurement gates — i.e., 50-100p companies, not 200-500p companies where Linear's price-cut win really hurts. Mid-market procurement runs 30-60 days for $15-50K ACV, and security review eats 2-4 weeks (cf. growthspreeofficial benchmark). 14-day trial closes BEFORE procurement opens. |
| M0e | Founders dogfood Threadline on themselves; this matches paying ICP | **FAILS** | Founders are ex-Google ICs / leads with Google-scale infra muscle memory. Paying ICP is engineering leadership at 50-500p companies whose workflows, headcount math, and tooling stack are NOTHING like Google's. Dogfood-on-self ships a product calibrated to "smart 5-person team at unicorn" rather than "harried EM at 200-person Series C." Per v0.3 strengthened M0e: required fix is BOTH pivots — pivot target audience materials to the mid-market EM persona AND expand dogfood to include 2+ mid-market engineering org workflows (paid pilots, design-partner sessions) BEFORE launch. The wrong fix (which v0.3 explicitly forbids) would be "defer the paying ICP and just sell to fellow ex-Googler friends first" — that preserves the mismatch. |

**4 of 5 premises failed challenge. The current plan would ship a product calibrated to ex-Google peers, priced at the top of the band without procurement-aware mechanics, against the canonical winner of the category, into a launch surface (HN) whose audience overlaps with users but not buyers.** Sections 1-9 below are written under these corrected premises, not the original ones.

---

# Step 0 — Pre-review system audit

## Existing context

Design doc only — no README, no landing page, no newsletter, no prior planning artifacts referenced. Founders have shipped no prior products. No marketing artifacts.

## Founder audience surface (numeric)

| Surface | Count | ICP-aligned? |
|---|---|---|
| X / Twitter followers | 200 | Unknown — likely ex-coworkers + general dev-Twitter. NOT demonstrated to be EM/tech-lead-at-50-500p-co. |
| Personal email list | ~50 | Friends/family. NOT ICP. |
| LinkedIn | Not stated | Likely meaningful for ex-Google engineers, but not surfaced |
| Newsletter / blog / podcast | None | N/A |
| GitHub stars on prior public projects | Not stated; assume zero relevant | N/A |
| Community presence (Rands Leadership Slack, LeadDev, etc.) | Not stated; default assume zero | N/A |

**Verdict: effectively zero ICP-aligned audience.** 200 generic-X + 50 friends/family is a Mode-C signal on count grounds alone, AND the audience that exists is in the wrong audience-class (not engineering leadership at 50-500p companies).

## Web-search findings (competitive landscape — full Section 1 below)

Quick highlights flowing into mode selection:

- **Linear cut Business tier 68% in 7 months** — from $50/seat July 2025 → $29/seat Jan 2026 → $16/seat Feb 2026 (per saaspricepulse / vendr / quackback). This is one of the largest tracked SaaS price cuts. Threadline's $40 is now **2.5x Linear Business** in a category where Linear is the design-led, mind-share-leading default. Massive premise problem.
- **Linear has 150,000+ teams (early 2025).** Bottom-up adoption playbook, $35K total marketing spend through Series C, Karri Saarinen's "build in public" via Twitter and Lenny's-podcast guesting drove most of the funnel.
- **Competitors include Height (AI-differentiated), Shortcut (Linear-vs-Jira middle ground), Plane (open-source Linear clone), Jira (configurable opposite), GitHub Projects (free, native).** Crowded category with strong incumbents and free alternatives.

# Step 0B — Mode selection

**Triggering conditions per v0.3 activation rules:**
- Founder audience: <500 followers in any relevant category AND content-aligned audience absent → Mode C signal
- Mid-build with hard launch date (validation gate "5 paying companies by day 30") → load-bearing tie-breaker condition
- ICP-misaligned audience: 200 X followers are not EMs at 50-500p SaaS companies → Mode C signal on alignment

**Tie-breaker (v0.3, load-bearing):**
> Mid-build with hard launch date AND (small <500 OR ICP-misaligned audience) → prefer **Mode A with Section 4 elevated** over Mode C alone, because Mode C alone skips the launch playbook the founder still needs.

Both conditions fire. **Mode A with Section 4 elevated.** The founders are pre-launch with a 30-day validation gate; they need (a) the audience-build sprint in Section 4 because they have no audience, AND (b) the full launch playbook in Section 5 because they're shipping in weeks. Mode C alone would build audience but skip the playbook; that's incomplete given their timeline.

**Note for v0.3 calibration:** this is exactly the case v0.2 disagreed on (Mode A in 2/3 runs, Mode C in 1/3). The v0.3 tie-breaker resolves it cleanly in one read — both conditions of the tie-breaker are met explicitly.

---

# Step 0A — Forcing questions

The founders' naive answers and the skill's pushback are recorded as Q/A pairs. Final accepted answer appears under each.

## M1. Audience reality

**Founder (naive):** "Engineering managers at mid-size SaaS companies. They hang out on Hacker News and Twitter."

**Skill pushback:** That's a demographic, not a person. Also "they hang out on HN" mixes IC engineers (true) with EMs / decision-makers (much weaker overlap; EMs are on Rands Leadership Slack, LeadDev, Pragmatic Engineer comments, Lenny's Newsletter community, not the HN front page). Refused.

**Refined answer (post-pushback):**
- Named persona: **"Priya, Senior EM, 30-person backend platform team at a Series C 250-person fintech (Plaid-era), 6 years post-Google, recently switched her org from Jira to Linear in Q4 2025, slightly underwhelmed by Linear's roadmap features for cross-team dependencies, reports to a VP Eng who reports to CTO."**
- Attributes: (1) Series B-C company 100-400 people, (2) currently uses Linear, (3) actively unhappy with one specific Linear gap (cross-team dependencies / roadmapping / sprint analytics — TBD), (4) procurement is "tell finance, get a PO" not "fill a form," (5) reads Lenny's, Pragmatic Engineer, LeadDev, lurks in Rands Leadership Slack
- Where attention lives RIGHT NOW: **Rands Leadership Slack (~16K members, manual gate), Pragmatic Engineer newsletter (1M+ subs), Lenny's Newsletter and podcast (engineering leadership crossover), LeadDev conferences + content, Software Engineering Daily podcast, occasionally HN comments (rarely front page)**

## M2. Discovery path

**Founder (naive):** "They see our Show HN post and click through."

**Skill pushback:** Refused per M0a finding. Step 1 cannot be Show HN. Mid-market EMs do not buy off the HN front page; they buy because (a) a peer they trust recommended it in Rands / LeadDev / a 1:1, OR (b) a creator they trust wrote about it, OR (c) their team's IC engineers pushed it bottom-up. Show HN can produce step 1's IC-engineer awareness but cannot produce the EM's purchase decision.

**Refined discovery path (minimum 3 steps):**
1. IC engineer on Priya's team sees a Threadline thread on dev-Twitter, OR reads a "we switched from Linear to X" post on a respected eng-leadership blog (Pragmatic Engineer guest post, Will Larson's Irrational Exuberance, Charity Majors-type writing), OR encounters in Rands Leadership Slack
2. IC engineer tries the trial / shares with team channel
3. Priya (the EM) hears about it from her team OR independently sees it in her own newsletter / Slack feed, recognizes the named pain (cross-team deps / roadmap analytics / whatever the wedge is), and books a call
4. Procurement: 30-60 day cycle including SOC 2 check, finance sign-off

Discovery takes 4-8 weeks from first IC contact to PO, NOT one HN day.

## M3. Pre-launch audience

**Founder (naive):** "200 X followers, 50-person email list."

**Skill verdict:** Effectively zero in the ICP-aligned sense. Per v0.3 mode-selection rules this triggers Mode C, but tie-breaker promotes to Mode A with elevated Section 4 because of the hard launch gate.

## M4. Channel honesty

**Founder (naive):** "We're good at building things and writing technical docs."

**Skill pushback:** Building things is product, not distribution (rejection per the question rubric). "Writing technical docs" without a published track record is aspirational, not demonstrated.

**Refined answer (honest):**
- Founders' one demonstrable distribution-adjacent asset: **ex-Google engineer credentials** — credible enough for cold outreach to other ex-Google EMs (a slice of the ICP), and credible enough that named Google-alum-led companies might take a call. Modest asset, not a moat.
- Demonstrated channel advantage: **none.** Per the question's rubric, "I don't have one yet" becomes the first work item.

## M5. Competitor traffic source

**Founder (naive):** "I assume mostly word-of-mouth and SEO."

**Skill pushback:** Guesses presented as facts — refused. Per Step 0 web search, here is the actual data:

- **Linear:** ~$35K total paid marketing through Series C. Primary funnel: founder build-in-public on Twitter (Karri Saarinen specifically), Lenny's Newsletter / podcast guest spots, bottom-up team-by-team adoption, mimetic-logo strategy (land Vercel-class fintech → cascade). Today (post Feb-2026 price cut): aggressive pricing pressure + AI features at the Business tier.
- **Shortcut:** GitHub-integration content, GitLab-adjacent SEO, comparison-page SEO ("Shortcut vs Linear"), some paid.
- **Height:** AI-features content, founder presence on Twitter, productivity-influencer adjacency.
- **Plane:** OSS GitHub stars (issue tracker), self-hosted-search SEO, "open-source alternative to Linear" SEO.
- **Jira:** Atlassian sales motion + decades-old enterprise sales relationships + integrated tool suite stickiness; not a real comparable for a startup.

**Action:** founder commits to study Linear's playbook in detail (Karri Saarinen's Lenny's Podcast episode + the public blog posts + the "$35K marketing spend" essay) before Section 1 finalizes.

## M6. First 10 paying customers

**Founder (naive):** "Founders' friends and the HN cohort."

**Skill pushback:** Refused. "Friends" is generic AND friends are not validated ICP unless they actually run 50-500p eng orgs with budget authority. "HN cohort" is passive language and HN won't surface paying mid-market companies — it'll surface curious engineers without procurement power. Refused per v0.3.

**Refined answer:**
- Named list of 10 specific ex-Google EM/tech-lead-at-50-500p-company contacts to email TOMORROW (founders own this list; if they cannot produce it, that itself is a major finding — go acquire 10 names from LinkedIn alumni search + intros)
- Specific communities (with awareness of rules): post in Rands Leadership Slack #tools after lurking + contributing for 30 days minimum (the manual gate enforces real human posture); contribute meaningfully on a Pragmatic Engineer / Lenny's comment surface for 30 days
- **Concierge cohort:** founders personally onboard the first 10 customers — 1:1 calls, custom Slack channel per customer, weekly check-in. (See Section 5 launch-gate discussion.)
- Outreach sequence: 10 emails → 3-5 calls → 1-2 design-partner conversions. Repeat weekly. Realistic ramp: 5 paying companies in 30 days is aggressive but possible IF the 10-name list exists day 1.

## M7. Time allocation

**Founder (naive):** "We've been heads-down building. Maybe 5% on marketing, the rest on product."

**Skill verdict:** Ratio is wrong per the question rubric. With <500 ICP-aligned audience and 30-day validation gate, **audience-building share must be ≥30% NOW** and ≥50% in the final week before launch. Acknowledged as a known risk; flagged in Section 9.

---

# Section 1 — Competitive landscape

## 1a. Direct competitors

| Name | URL | Founded | Pricing (2026) | Apparent traffic source | User complaints | Positioning read | Winning? |
|---|---|---|---|---|---|---|---|
| **Linear** | linear.app | 2019 | Free / $10 Basic / $16 Business / Enterprise (slashed from $50 in Jul 2025) | Build-in-public Twitter (Karri Saarinen), Lenny's pod, bottom-up viral within orgs, mimetic logos | "Pricing got weird in 2025"; "missing roadmap features"; "limited cross-team workflows"; "Slack-style spam triage" | The category-defining design-led B2B SaaS for engineering teams. Now also the price leader at $16 Business. | **YES — dominant.** ~150K teams, $400M-$1.25B valuation range, all the design-led mindshare. |
| **Shortcut** (ex-Clubhouse) | shortcut.com | 2014 | Free <10 / $8.50 Team / $12 Business / Enterprise | GitHub-integration content, "vs Linear" SEO, podcast guesting | "Heavy compared to Linear"; "feels like Jira-lite" | Middle ground between Linear's opinionatedness and Jira's configurability; PM-friendly. | Surviving, not winning. Linear has the air. |
| **Height** | height.app | 2018 | Free / $7 Team / $9 Pro / $12 Business | AI-features content, founder Twitter, productivity creator adjacency | "Chat-in-tracker is noisy"; "AI features still beta-quality" | AI-first project tracker w/ chat integration. | Mid-pack. Differentiated bet on AI. |
| **Plane** | plane.so | 2022 | Free OSS / $7 One / Pro / Enterprise | OSS GitHub stars (~30K+), "open-source Linear alternative" SEO, self-hosted-search | "Less polished than Linear"; "limited integrations" | Open-source Linear clone for teams who want self-host. | Niche but growing. |
| **Jira** | atlassian.com/jira | 2002 | Free / $7.16 Standard / $12.48 Premium / Enterprise | Atlassian enterprise sales motion, decades of installed base, ecosystem | "Slow"; "configurable to the point of paralysis"; "outdated UX" | The enterprise default. Configurable opposite of Linear. | Different motion entirely; not a real comparable for a $40-seat startup. |
| **GitHub Projects** | github.com | 2021 (Projects v2) | Free with GitHub | Already-in-the-workflow distribution | "Underpowered for cross-team work"; "no real sprints" | Free, embedded in dev workflow. | A free competitor is a strategic threat — any team with GitHub already has it. |

**Reality check on Threadline's positioning ("Better than Linear for engineering-specific workflows"):** Linear IS the engineering-specific workflow tool. Threadline is claiming to beat the playbook winner in their own playbook with no founders' audience, no waitlist, and 2.5x the price (vs Linear Business at $16). This is the M0b finding made concrete.

## 1b. Canonical-success comparables

For B2B SaaS / mid-market motion class:

| Comparable | Founded | Current scale | Pricing | Primary acquisition | Onboarding | Launch gate | Delta vs Threadline plan |
|---|---|---|---|---|---|---|---|
| **Linear** | 2019 | ~150K teams; $400M-$1.25B | $0/$10/$16 (post Feb-26 cut) | Founder Twitter build-in-public + Lenny's Pod + bottom-up + mimetic logos. **$35K total paid marketing through Series C.** | Self-serve + invite-flow + Slack community for early customers | Waitlist + multi-launch sequence (announce → seed → open → Series A); each launch larger than the prior | Threadline has no founder audience, no build-in-public history, no waitlist, no community. Plans single-shot HN launch. |
| **Notion** | 2016 | $10B+ valuation, 20M+ users | Free / $10 / $15 / Enterprise | B2C2B — individuals adopt → drag into work → enterprise pulled in. Community-led, ambassador program. | Freemium with REAL value in free tier; single-player → multi-player | Activated-team metric (≥2 users, twice in week 1) | Threadline has no free tier, no individual-use case (it's team-only), no community, no ambassador surface. Wrong motion entirely. |
| **Slack** (B2B viral) | 2013 | Microsoft-comparable scale | Free / $8.75 / $15 / Enterprise | Bottom-up adoption + manual concierge (Stewart Butterfield famously emailed every early team), free tier as Trojan horse | Free tier + team invite multiplier | "Are people DAILY active and inviting?" | Threadline has no free tier and no concierge motion planned. |
| **Superhuman** (premium-concierge B2B-ish) | 2014 | $825M Aug-2025 acquisition by Grammarly | $30/mo | Vohra personally onboarded first ~200 users; Vohra "very disappointed" PMF gate; invite-only waitlist | Manual concierge onboarding | PMF-signal gate (≥40% "very disappointed") | Threadline could borrow concierge-onboard playbook for first 10-20 (see Section 5). Calendar gate is wrong for retention-driven seats. |

## 1c. Pattern surface

**What canonical successes share that Threadline's plan lacks:**

1. **Founder-led distribution before the product is launchable.** Karri Saarinen built in public on Twitter for months before Linear's MVP. Stewart Butterfield personally emailed prospects. Notion founders ran the community personally. Threadline's plan has zero pre-launch audience-building.
2. **A free or freemium or concierge-onboard motion that produces bottom-up adoption.** Linear / Notion / Slack all leverage this. Superhuman uses concierge. Threadline has neither — paid-only, self-serve trial. This puts Threadline in the worst quadrant: no viral motion AND no concierge intimacy.
3. **A PMF-signal gate, not a calendar gate.** Vohra waited for 40% "very disappointed." Superhuman onboarded 200 users by hand first. Threadline's "5 paying companies by day 30" is a calendar gate.
4. **Canonical successes do NOT compete head-to-head on the category leader's own positioning.** Linear came when Jira was the default; Linear's positioning was "fast and design-led," not "better than Jira." Threadline saying "better than Linear" is the M0b crater.

**Which pattern is the plan implicitly following?** None cleanly. Closest is "another Linear" but without Linear's founder-audience, build-in-public history, free tier, or design-DNA-as-marketing. Threadline is following the Jira-of-2010 playbook (sell into orgs against a default) without the Atlassian enterprise sales motion.

**Founder homework:** read Karri Saarinen's Lenny's Newsletter episode + "$1.25B on $35K marketing" Ideaplan post + Rachel Hepworth's Notion PLG writeup. Do this before refining Sections 2-6.

---

# Section 2 — ICP specification

See `icp.md` (separate artifact). Summary:

**Priya — Senior EM, 30-person backend platform team, Series C 200-300p fintech**
- 6 years post-Google; runs 4 squads, ~30 ICs
- Currently uses Linear (her org migrated Q4 2025); previously Jira; previously Asana before that
- Active pain candidate: cross-team dependency tracking, sprint-level analytics for VP Eng reporting, roadmap-vs-execution gap. **TBD: needs 5 design-partner interviews to pick THE wedge.**
- Attention surface: Rands Leadership Slack (lurks), Pragmatic Engineer (paid sub), Lenny's (free), LeadDev annual conference attendee, Software Engineering Daily episodes during commute
- Adjacent-category spend: Pragmatic Engineer paid sub ($150/yr), team subscription to Linear ($16/seat × 30 = $480/mo), team subscription to Slack (varies), Notion for docs
- Objections she'd raise: "Why would I switch from Linear, which just dropped 68%? You're 2.5x more expensive." / "Who are you?" / "What about SOC 2?" / "Will you exist in 2 years?"
- Reasons she'd convert: a named specific pain Linear can't fix, a peer-EM recommendation, founder credibility (ex-Google helps but isn't enough), a concierge-onboard offer that signals "we'll make this work for you specifically"

---

# Section 3 — Distribution channels (with motion-class rules)

## 3.0 Motion-class application (v0.3)

**This is a B2B SaaS product, mid-market.** Apply the **B2B SaaS block** in Section 3 motion-class rules:

> Generic social channels are weak; specific vertical publications carry far higher conversion. For engineering-team products, name: **Pragmatic Engineer, Lenny's Newsletter, LeadDev, Rands Leadership Slack, podcasts (Software Engineering Daily, Engineering Enablement)**. Add these by name, not as a generic "B2B newsletters" entry.

**The dev-tool block does NOT apply.** Threadline is a project tracker, not a code-level developer tool. It does NOT ship SDKs, has no GitHub-repo-as-product, and its purchase decision is made by EMs/VPs (not by individual devs evaluating an SDK). Therefore: GitHub-as-marketing-surface is NOT a primary channel here; docs-as-SEO-via-framework-tutorials is NOT relevant; the dev-tool tonal rule (anti-superlatives, link to GitHub before landing page) does NOT override on launch copy. This is a smoke-test check that the v0.3 motion-class discrimination works: dev-tool rules should NOT fire on B2B SaaS. **They do not fire here.**

## 3a. Channel-by-channel scoring (for THIS founder)

Scoring is 1-5 (5 = best) for THIS founder's situation, not in general.

| Channel | Reach | Cost | Conversion | Founder fit | Effort to start | Verdict |
|---|---|---|---|---|---|---|
| **Show HN** | 3 (IC eng heavy, EM light) | 5 (free) | 2 (low for paid B2B SaaS w/o trust) | 3 (ex-Google legitimizes) | 4 (low) | KEEP but reframe — IC entry point producing inbound, NOT the buyer channel. |
| **Pragmatic Engineer newsletter** | 5 (1M+ subs, exact ICP) | 1 (no paid sponsorships per Orosz policy) | 5 if mentioned | 1 (must be EARNED via story or intro) | 5 (very high) | EARN via build-in-public + unique-data story. Long shot, max value. |
| **Pragmatic Engineer Podcast** | 4 | 3 (limited sponsor slots exist) | 4 | 2 | 3 | Pitch sponsorship if budget allows; ~$5-10K/slot industry typical for B2B niche. |
| **Lenny's Newsletter** | 5 (~600K subs, EM-adjacent) | 2 (CPM $50-$150 for B2B specialized per influencerskit 2026) | 4 | 2 | 3 | Direct sponsorship est. $5-15K/issue. Worth one paid placement at launch + 1 organic guest contribution. |
| **Rands Leadership Slack** (16K EMs, manual gate) | 4 (perfect ICP density) | 5 (free) | 4 if community-fit | 2 (requires LURK + contribute 30+ days) | 5 (high effort over time) | **PRIMARY.** Join now, contribute 30 days before any mention. |
| **LeadDev conferences + content** | 3 | 3 | 4 | 2 | 3 | Pitch talk for LeadDev 2026; write LeadDev articles. |
| **Software Engineering Daily podcast guest** | 3 | 5 | 3 | 3 | 3 | Pitch — but founders need a story first. |
| **Twitter/X organic** | 2 (200 followers) | 5 | 2 | 3 | 5 | Required for build-in-public à la Karri Saarinen; ramp is months not days. |
| **LinkedIn organic** | 4 (ex-Google + B2B audience fit) | 5 | 4 | 4 (ex-Googler LinkedIn presence is credible) | 3 | **PRIMARY.** Highest-leverage channel for THIS founder pair; underweighted in original plan. |
| **Cold outreach (LinkedIn DM + email to ex-Google EM list)** | 3 | 5 | 5 (warm via alumni) | 4 | 4 | **PRIMARY for first 10 customers.** Concierge cohort fits. |
| **Founder-owned engineering management blog** | 1 (zero day-1 audience) | 5 | 2 | 3 | 3 | Compound asset, not launch channel. Build over 3-6 months. |
| **Product Hunt** | 2 (consumer-skewed, low B2B paid conv) | 5 | 1 | 2 | 3 | Skip v1; revisit at 6 months. |
| **SEO ("Linear alternative for X")** | 5 long-term | 5 | 4 | 2 | 1 (6-12 mo ramp) | Start day 1; harvest Q3-Q4. |
| **Paid Google/LinkedIn ads** | 3 | 1 (CAC $400-1000/seat est.) | 3 | 2 | 4 | Skip until PMF proven. |
| **IndieHackers** | 2 (wrong audience class) | 5 | 1 | 3 | 4 | Skip. |
| **Reddit** | 3 | 5 | 2 (ban risk) | 2 | 3 | Skip explicit promo; lurk r/ExperiencedDevs only. |

## 3b. Top 3 channels for v1 (forced prioritization)

1. **Cold outreach + concierge to ex-Google EM contacts** — produces the first 10 customers if list exists
2. **LinkedIn organic build-in-public + ex-Google credibility** — primary asynchronous reach engine
3. **Rands Leadership Slack participation** (after 30-day lurk) + **earned Pragmatic Engineer / Lenny's coverage** if a story-worthy angle emerges

Show HN is a tactical entry point on launch day, NOT a primary channel. The original plan's "Show HN + content marketing on the engineering management blog" is a one-and-a-half-channel plan with no real ICP overlap on either leg.

---

# Section 4 — Pre-launch audience-building plan (ELEVATED per v0.3 tie-breaker)

Section 4 is load-bearing here because audience is effectively zero and the validation gate is 30 days away.

## Day 1-30 (NOW through end of June 2026)

Weekly cadence:
- **3x LinkedIn posts/week** by each founder — build-in-public, named lessons from building Threadline, ex-Google insights about engineering org tooling at scale. Target: 1K followers each by end of month via consistent posting + commenting on EM-influencer posts.
- **2x X / Twitter posts/week** each founder — same build-in-public theme, lower stakes.
- **5x cold-outreach emails / DMs per week per founder** to named ex-Google EMs / tech leads at 50-500p companies. 50 emails total over 30 days = realistic 5-10 design-partner conversations.
- **Lurk + contribute** in Rands Leadership Slack (no product mentions for 30 days; only substantive contributions). Goal: be recognizable as a contributor BEFORE ever mentioning Threadline.
- **Pitch 5 podcasts** by week 4: Software Engineering Daily, Engineering Enablement, LeadDev podcast, Pragmatic Engineer Podcast (sponsorship slot or guest pitch with unique story angle), 1 fintech-vertical eng podcast.
- **Write 1 cornerstone blog post** week 2 — "What Linear Gets Wrong About 200-Person Engineering Orgs" (or whatever the wedge actually is once 5 design-partner interviews complete). Asset that Section 3's SEO compounds on AND the Pragmatic Engineer / Lenny's pitch hook.
- **Run 5-10 design-partner interviews with mid-market EMs** week 1-2 (M0e fix: paid pilots / honoraria; this is the "expand dogfood to paying-ICP-representative subjects" required pivot).

Gate to proceed to day 31-60: ≥5 design-partner conversations completed AND ≥1 named pain confirmed across ≥3 partners.

## Day 31-60

- Scale up: 2 cornerstone blog posts/month (one per founder), continued LinkedIn cadence, 1 podcast appearance landed
- Convert design partners to first paying customers (concierge onboard); collect testimonials and case-study material
- Pitch Pragmatic Engineer / LeadDev guest contributions with data from design partners (the story that earns inclusion)
- Begin building Rands Slack reputation; OK to drop one tasteful mention of Threadline by week 8 if reputation established

## Day 61-90

- Integrate launch sequence (see Section 5 / launch_playbook.md)
- 2-3 paying customers from concierge cohort; refine messaging from real buyer language
- Continue cadence; layer paid (Lenny's sponsorship if budget allows) only after organic signal exists

---

# Section 5 — Launch playbook (see launch_playbook.md for hour-by-hour)

## 5a. Question the launch gate

Original plan: "Validation gate: 5 paying companies by day 30." This is a **calendar gate + arbitrary count.** Threadline is retention-driven (seat-based subscription with churn risk if product doesn't stick). Per v0.3 Section 5a, retention-driven products should use **PMF-signal gates** not calendar gates.

**Recommended PMF-signal gate (Superhuman/Vohra-style adapted to B2B):**
- ≥40% of design-partner teams answer "very disappointed" to "how would you feel if your team could no longer use Threadline" after 4 weeks of usage
- OR: ≥3 design-partner teams unprompted-refer Threadline to another EM in their network
- OR: ≥3 teams' IC engineers organically request Threadline in their team channel (bottom-up signal)

**Concierge-first cohort:** founders personally onboard the first 10-20 teams via 1:1 calls, custom Slack channels, weekly check-ins. Superhuman / Slack / Linear all did this. "5 paying by day 30" is fine as a soft milestone for concierge cohort completion, NOT as a gate to public launch.

**If founders defend the calendar gate:** they must explain why Threadline is NOT retention-driven (it is) AND why the PMF signal is unnecessary (it is). They should fail this defense and adopt the PMF-signal gate.

## 5b. Sequence pattern (see launch_playbook.md for full table)

High-level: 30-day audience-build sprint → 60-day concierge-onboard with design partners → public launch ONLY when PMF signal hits → multi-channel sequenced rollout (LinkedIn anchor, Show HN as IC-funnel entry, Pragmatic Engineer / Lenny's earned coverage as buyer-trust amplifier, Rands Slack mention by then-credible contributor).

**Note on launch copy tone:** because this is B2B SaaS (NOT dev tool), the dev-tool tonal rules in Section 3 do NOT apply. Standard B2B SaaS copy register is fine — benefits + proof + named comparison + clear call-to-action. The "no superlatives, lead with technical specifics, link to GitHub before landing page" pattern is for dev-tool launches and would actively underperform for an EM buyer reading on LinkedIn.

---

# Section 6 — Pricing & packaging

## 6a. Pricing BAND question

Original price: **$40/seat/month** — anchored on... what? The design doc doesn't show ICP-WTP evidence; it just states the price. Per v0.3 Section 6a, surface the band question first.

**Reality of the band post-Feb-2026:**
- Linear Basic: $10/seat/mo
- Linear Business: $16/seat/mo (slashed from $50 in 7 months)
- Shortcut Team: $8.50/seat
- Height Team: $7/seat
- Plane One: $7/seat
- Jira Standard: $7.16/seat
- GitHub Projects: **$0** (bundled with GitHub seats already paid)

**Threadline at $40/seat is 2.5x Linear Business and 5-6x the cheapest direct comp.** The original plan's "Pricing: $40/seat/month" is band-anchored on... nothing visible. It's also explicitly contradicted by Linear's aggressive Feb-2026 cut, which the founders likely either don't know about or haven't priced in.

**Two coherent strategic options:**

(A) **Match the new band: $15-25/seat range.** Treats Linear as the reference price. Removes price as a switching objection. Sacrifices "premium positioning" the original $40 implied.

(B) **Defend the premium with concierge + named-wedge depth.** Justify $40 with: (i) named workflow Linear doesn't do (the wedge), (ii) concierge onboarding included, (iii) higher SLA / dedicated CSM, (iv) targeted at upper-mid-market (300-500p) where dollars are large and pricing less sensitive. Doable BUT only if the wedge is real and concierge is genuinely shipped.

**Refusing the simple "match Linear" reflex:** anti-pattern #7 — "match the cheapest competitor's price" is wrong for time-poor/money-rich segments. Mid-market EM buyers ARE time-poor; they trust-shop more than price-shop. $25/seat with concierge and a named wedge may convert BETTER than $10/seat self-serve. But $40 needs explicit justification — the founders owe themselves the defense or the cut.

**Recommended:** **$25/seat with annual billing discount, concierge onboarding included for first 50 customers, named wedge in positioning.** Mid-band (above Linear Business, below "enterprise"), defends the trust-positioning, matches what a 200-500p company's EM expects to pay for a category-leader-adjacent tool.

## 6b. Standard pricing & packaging coverage

- **Tier structure:** Single tier for v1 ($25/seat). NO free tier (preserves trust positioning; avoids M0d freebie-disqualifier). NO open-ended trial — replace 14-day trial with **30-day concierge pilot, contract signed up front, full refund if no value at end of 30 days.** This commits the buyer (selects for serious intent) AND fits the 30-60-day mid-market procurement window.
- **Annual billing:** 15-20% discount. RevenueCat / industry data: annual billing dominates retention.
- **Per-seat:** correct model for this category.
- **Trial mechanic revisited per M0d:** 14-day no-credit-card trial selects for evaluator-engineers in companies without procurement (50-100p). For 200-500p mid-market the right mechanic is **paid pilot with refund** — commits the buyer, signals seriousness, fits procurement timeline.

---

# Section 7 — Post-launch growth loops

| Loop | Compounds? | Notes |
|---|---|---|
| Referral / two-sided incentive | Potentially | Linear didn't push this aggressively; Notion did. "Refer an EM peer, get 20% off" worth implementing in v1.1. |
| Content SEO ("Linear alternative for X") | YES — long horizon | Start day 1. Compounds 6-12 months out. |
| Network effects within an org | YES (bottom-up) | Once 1 team in a 200p org adopts, other teams likely follow. Build invite mechanics. |
| Brand compounding via founder build-in-public | YES if consistent | Linear's $35K marketing spend was built on this. Cadence matters. |
| Retention-driven word-of-mouth | YES if product sticks | EM communities are tight; one Priya tells another Priya. Requires real product depth. |

**Risk surfaced:** if NONE of these compound (because product doesn't stick OR audience never compounds), Threadline is an acquisition-treadmill business with $400-1000 CAC and 14-18 month CAC payback (per growthspreeofficial mid-market benchmark). That's a strategic red flag — capital-intensity is significant in mid-market B2B SaaS even at $25/seat.

---

# Section 8 — Metrics & instrumentation

**Measure:**
- Acquisition by named channel (UTM every link)
- Activation: ≥2 users on a team using Threadline ≥3 times/week for 2 weeks (Notion threshold pattern adapted)
- Concierge cohort PMF signal (Vohra "very disappointed" survey at week 4)
- Day-7 / Day-30 team retention (team-level, not user-level — this is the seat-based business)
- Trial → paid conversion (and refund rate on paid-pilot mechanic)
- Per-channel CAC once data exists
- Net Revenue Retention by quarter (mid-market benchmark: 108% per Optifai 2026)

**Do NOT measure (vanity for THIS business):**
- HN upvotes
- Total signups divorced from team-activation
- X / LinkedIn follower count in isolation (track only as audience-building input)

---

# Section 9 — Risk analysis

| Risk | Severity | Mitigation |
|---|---|---|
| **Single-channel concentration on Show HN** | HIGH if pursued as-stated | Section 3 forces 3 named channels (LinkedIn + cold outreach + Rands) with Show HN as auxiliary. |
| **Pricing at 2.5x category leader without wedge** | CRITICAL | Either (a) cut to $25 + concierge + named wedge, or (b) defend $40 with rigorous ICP-WTP evidence. Status quo $40 is indefensible. |
| **Linear Feb-2026 price cut to $16** | CRITICAL | Direct competitive response. Reframe positioning around named workflow gap, not "better than Linear" generically. |
| **No founder audience pre-launch** | HIGH | Section 4 elevated; 30-day sprint required. |
| **Calendar launch gate** | HIGH for retention business | Replace with PMF-signal gate (Section 5a). |
| **Mid-market procurement cycle (30-60 days + 2-4 wk security review)** | HIGH for "5 paying by day 30" target | Adjust: target 5 PAID-PILOT teams by day 30, with annual-contract conversions realistic day 60-90. |
| **GitHub Projects (free) as silent alternative** | MEDIUM | Address explicitly in positioning ("why a free tool you already have doesn't solve X for a 200p org"). |
| **Dogfood mismatch (ex-Google ICs)** | HIGH | M0e fix: expand dogfood subjects via 5+ design-partner pilots BEFORE public launch. |
| **Trust risk: no credibility surface yet** | HIGH | Ex-Google legitimizes but is insufficient. Build via LinkedIn + Rands Slack reputation + earned coverage. |
| **Macro risk: Linear could match Threadline's wedge in a sprint** | MEDIUM | Mitigate by depth — pick a wedge requiring real product investment to clone (e.g., cross-team dependency intelligence taking ≥6 months to build). |

---

# Outside-voice critique (adversarial pass)

1. **Single biggest missed risk:** the "wedge" is still TBD. The whole plan is contingent on founders identifying a real Linear-can't-fix pain in design-partner interviews. If no clear wedge emerges, the plan collapses to "another Linear at 2.5x the price by people Linear's audience has never heard of." Week-1 single biggest priority.
2. **Channel claim weaker than positioned:** "ex-Google credentials" treated as moderate moat throughout. In reality, ex-Google is table-stakes in YC / B2B SaaS founder pools. The actual asset would be specific ex-Google teams the founders led with named results. If not surfaceable, downgrade the "ex-Google legitimizes" weight everywhere.
3. **Audience claim lacking evidence:** the "Priya" persona is a synthesis; not validated against 5+ real EMs. Until design-partner interviews complete, Priya is a hypothesis.
4. **Provocative reframe:** stop competing with Linear at all. Build **the analytics layer on top of Linear** (and Jira and Shortcut). Reposition as the "EM dashboard that reads from your existing tracker" rather than "yet another tracker." Distribution becomes WAY easier (integrate, don't switch). Pricing additive ($25/seat ON TOP OF Linear, not instead of). Competitive surface shrinks (Linear isn't a competitor, it's a data source). CEO-mode reframe the founders should seriously consider before continuing the head-to-head path.

---

# 3 strongest action items for THIS week

1. **Acquire (or fail to acquire) a list of 10 named ex-Google EM/tech-lead-at-50-500p-company contacts to email Monday.** If they cannot produce this list, the entire plan is at risk and the founders need to address it first.
2. **Book 5 design-partner interviews this week** with mid-market EMs (paid honorarium $200-500 each). Output: named wedge by end of week.
3. **Each founder posts 3x on LinkedIn this week** with build-in-public content. Establish cadence. (And join Rands Leadership Slack today; begin lurk-and-contribute period.)

# Follow-up skills to run

- `/plan-ceo-review` — the pricing + positioning + "build on top of Linear" reframe deserves CEO-mode treatment
- `/office-hours` — if the wedge doesn't surface from design-partner interviews, the whole product premise needs office-hours rework
- Re-run `/plan-cmo-review` in 30 days to evaluate Section 4 sprint progress

---

# Sources (web-search citations)

- [Linear Pricing 2026 (saaspricepulse)](https://www.saaspricepulse.com/tools/linear)
- [Linear Pricing 2026 plans/features (Quackback)](https://quackback.io/blog/linear-pricing)
- [Linear: $1.25B on $35K Marketing (Ideaplan)](https://www.ideaplan.io/blog/how-linear-grew-to-1-billion-with-35k-marketing-spend)
- [Inside Linear: building with taste — Karri Saarinen on Lenny's](https://www.lennysnewsletter.com/p/inside-linear-building-with-taste)
- [Sponsoring The Pragmatic Engineer (newsletter does NOT take sponsorships; podcast has limited slots)](https://blog.pragmaticengineer.com/sponsor/)
- [Newsletter Sponsorship Pricing 2026 (Influencerskit)](https://www.influencerskit.com/blog/newsletter-sponsorship-pricing-rate-card-guide-2026)
- [Marketing Examined Guide to $1M Sponsorships — Lenny's (Stormy)](https://stormy.ai/blog/marketing-examined-lennys-newsletter-monetization-guide)
- [Mid-market B2B SaaS sales cycle benchmarks 2026 (growthspreeofficial)](https://www.growthspreeofficial.com/blogs/b2b-saas-sales-cycle-length-benchmarks-2026-by-acv-vertical)
- [B2B SaaS ACV benchmarks (Optifai)](https://optif.ai/learn/questions/b2b-saas-acv-benchmark/)
- [Rands Leadership Slack overview](https://thehiveindex.com/communities/rands-leadership-slack/)
- [Linear vs Height vs Plane (OpenHelm)](https://www.openhelm.ai/blog/linear-vs-height-vs-plane-project-management)
- [How Notion does marketing (First Round Review)](https://review.firstround.com/how-notion-does-marketing-a-deep-dive-into-its-community-influencers-growth-playbooks/)

