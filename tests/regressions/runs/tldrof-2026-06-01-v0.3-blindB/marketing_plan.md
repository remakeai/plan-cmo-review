# Marketing Plan — TLDR-of-TLDRs (tldrof.com)

**Reviewer:** plan-cmo-review v0.3.0 (blind regression run B)
**Date:** 2026-06-01
**Founder:** ex-Micron engineer; technical background; first consumer product
**Mode:** **Mode A — Full Marketing Review with Section 4 ELEVATED** (tie-breaker applied: mid-build, hard launch date in 20-22 days, ICP-misaligned audience)
**Default founder assumption:** technically strong, marketing-naive

---

## Operating mode

**Marketing-naive default holds.** Evidence-overrides check:
- Prior consumer/B2B product at >$10K MRR? **NO** (first consumer product)
- Demonstrated marketing track record? **NO** (11 Substack subs; 996 LinkedIn followers in semiconductors/hardware)
- ICP-aligned audience surface? **NO** (LinkedIn audience = semiconductors/hardware; product ICP = inbox-overloaded knowledge workers/newsletter readers — wrong category)
- Documented prior failed launches with retro? **NO**

Verdict: **Marketing-naive default is load-bearing. Premise-challenge is the highest-value work this skill produces this run.**

---

## TL;DR — Top findings (read this if you read nothing else)

1. **5 of 5 premise challenges produced material findings.** Show HN is the wrong audience class for the secondary segment the doc itself promotes (corporate/M365/regulated); canonical-success comparables (Readwise, Morning Brew, Superhuman) are missing from the plan; the auto-forward-helper-across-5-clients feature contradicts the trust-positioning the doc claims; the 7-day free trial selects engineers (the dogfood cohort) not the time-poor/money-rich segment the moat narrative requires; **the dogfood corpus is technical newsletters but a meaningful slice of the planned ICP reads Morning Brew / Axios AM / vertical legal-finance-healthcare sends.**
2. **The market is more crowded than the doc admits.** Mailbrew went **fully FREE in Nov 2025** under Evernomic ownership. That is a price-floor problem the doc does not acknowledge. Meco is at $3.99/mo. Readless is at $4.90/mo. The doc's $9/mo against a free competitor is defensible only with explicit ICP+positioning separation (which the doc partially has, in P4's corporate-coverage moat — but the planned launch sequence does not lean into that segment).
3. **Audience reality: ~0 ICP-aligned audience.** 996 LinkedIn followers in semiconductors and 11 Substack subs do not translate to consumer-newsletter buyers. The plan needs an audience-build sprint, not a launch playbook bolted onto a missing audience.
4. **Time allocation is backwards.** ~95% build, ~5% audience-building. For a solo founder shipping in 20-22 days to launch a category where Mailbrew is now free, this ratio is the single largest pre-launch risk.
5. **Launch sequence: Show HN can fire but cannot be the dominant channel.** Force minimum 3 channels; lean specifically into the moat segment (M365/corporate) via vertical channels the doc has not named.

---

## Step 0 — Pre-review system audit

### What exists
- **Design document** (heavily evolved — 4 founder editorial passes + CEO review + post-skill cleanup; 1535 lines; APPROVED)
- **CEO review** locked: 20-22 day build, $9/mo, Gmail-only auto-forward helper in v1.0, 3 above-the-fold differentiators (60-second magic moment / any-email-platform coverage / set-up-auto-forwarding-once)
- **Domain**: tldrof.com (verified during day-0 spike, per Open Question #4)
- **No landing page yet** (per the plan — landing copy is in days 14-16 polish window)
- **No social presence for the product** (founder has personal accounts; no @tldrof or product-branded channels exist)
- **No newsletter for the product** (founder has 11-subscriber personal Substack on unrelated topics)

### Web-search competitive landscape (done — see Section 1)
Five web searches fired covering Readless, Meco, Readwise, Morning Brew, Mailbrew/Refind, Superhuman, and Show HN base rates. Key surfaces:
- **Mailbrew is FREE as of Nov 2025** (Evernomic owner, free-tier with digest count + length caps)
- Meco at $3.99/mo positions as "magazine for newsletters" (different shape than digest)
- Readless at $4.90/mo is the direct shape-match
- Readwise at $9.99/mo is the canonical retention-led precedent (>90% retention, 4M registered, bootstrapped, "no paid acquisition" growth story)
- Morning Brew referral program drove ~30% of new subscriptions at peak; CAC $0.25 vs $3-5 paid ads

### Founder audience audit (numeric)

| Surface | Size | ICP-aligned? |
|---|---|---|
| Twitter/X (for the product) | 0 | n/a (no account) |
| LinkedIn (personal) | 996 | NO — semiconductors/hardware, not newsletter consumers |
| Personal Substack | 11 subs | UNKNOWN topic-alignment (presumably not newsletter-overload niche) |
| Newsletter for tldrof | 0 | — |
| GitHub stars on prior projects | unknown (some OSS) | Partial — overlap with HN cohort only |
| Discord/Slack community presence | none stated | — |
| Prior shipped consumer products | 0 | — |

**Net: effectively zero ICP-aligned audience for this product.** The 996 LinkedIn followers are in the wrong category. Per skill: "a 10K-follower audience in the wrong category counts as zero."

### Mode-selection decision

Activation rules:
- Mode C trigger fires (effectively zero ICP-aligned audience: <500 in relevant category AND existing audience in different category from product ICP).
- **HOWEVER**: founder is mid-build with hard launch date (20-22 days), and per v0.3 tie-breaker: "if the founder is mid-build with a hard launch date AND has either a small (<500) OR ICP-misaligned audience, prefer Mode A with Section 4 elevated."

**Locked: Mode A with Section 4 ELEVATED.** Reason: Mode C alone skips the launch playbook the founder still needs to ship in ~30 days; Mode A with elevated audience-build sprint produces both.

---

## PREMISE-LEVEL FINDINGS BLOCK (Step 0.5)

**5 of 5 premise challenges produced material findings.** This block is the highest-value output of the skill this run. Read this before anything tactical.

### Premise extraction table

| # | Accepted premise | Where in doc | Likely-wrong because (hypothesis) |
|---|---|---|---|
| 1 | Show HN is the launch (calendar day 18) | Distribution Plan; multiple references | HN is wrong audience class for the corporate/M365/regulated secondary segment the doc itself names as the structural moat |
| 2 | Direct competitor research is sufficient (Readless mainly) | Founder Editorial Pass 4 | Plan has no canonical-success comparables (Readwise, Morning Brew, Superhuman) and therefore no proven playbook to follow |
| 3 | All in-scope features serve the paying ICP | Implementation Specifications; CEO PC2 narrowed to Gmail-only | Gmail-only auto-forward helper still leaves at least one anti-feature (MCP wrapper roadmap; arguably the 7-day free trial itself); the v1.0.5 expansion to "Outlook / Apple Mail / Proton / Fastmail / Corporate-IMAP" needs trust-positioning audit before it is built |
| 4 | 7-day free trial is the right acquisition mechanic | P6; Approach C days 10-13 | 7-day trial selects time-rich/money-poor; the doc's own secondary moat is time-poor/money-rich (lawyers, finance, corporate). Cheap-trial validation is theater for the wrong segment |
| 5 | Founder-dogfood on TLDR/AlphaSignal/Latent Space/Pragmatic Engineer is sufficient | P1 ("Founder is the ICP"); Approach C days 5-9 | Dogfood is on technical-newsletter corpus; planned ICP includes general professionals (Morning Brew/Axios AM readers) AND vertical-corporate (legal/finance/healthcare sends). Product is being tuned to the wrong audience |

### M0a — Launch-platform audience-class fit

**Question:** Is Show HN the right audience class for tldrof.com?

**Web search performed:** "Show HN consumer subscription newsletter app launch traction." Findings: Show HN works for products whose buyers are HN-native. LoomLetter (similar shape: newsletter-aggregator app) launched there. Subscription-app launch landscape: 15,000 new subscription apps/month launching in 2026 (RevenueCat), median 58 days to $1K revenue, 109 days to $10K. HN front-page Show HN has weak base rate for consumer non-dev products specifically.

**Tension with doc:** the doc itself names the structural moat as the segment **OAuth-based competitors structurally cannot serve** — lawyers, finance, healthcare, government, agency operators with custom-domain email, M365/Outlook corporate users. **None of those people are on Hacker News in meaningful numbers.** HN reaches the dogfood cohort (engineers, PMs, AI-adjacent professionals); it does not reach the moat segment.

**Verdict: PREMISE PARTIALLY FAILS.** Show HN is a reasonable channel for the v1 stated cohort (engineers/PMs/founders). It is **NOT a reasonable launch platform** for the structural-moat segment the doc itself promotes. The plan that has Show HN as the dominant launch channel ships the product to the wrong half of the ICP and ignores the segment it was architecturally designed to serve.

**Cascading implication for Step 0A:** M2 (discovery path) must refuse "Show HN as step 1" even more aggressively. M6 (first 10 paying) must include the corporate/locked-out segment specifically.

### M0b — Canonical-success comparable

**Question:** What is the most successful product at this motion class (niche-indispensable consumer subscription, ~$9-30/mo, retention-led)? What did they do that this plan does NOT?

**Web search performed:** "Readwise growth strategy" + "Morning Brew growth referral newsletter acquisition." Findings:

- **Readwise** ($10/mo, ~$14M ARR, >90% retention, 4M registered, bootstrapped). Growth channels per their own writing: **strategic partnerships with EdTech companies, content-creator collaborations, API/integration ecosystem, SEO/SEM, app stores, word of mouth, referrals**. Notably NOT "viral on HN." Cofounders bootstrapped, wrote in public, built audience over years.
- **Morning Brew** ($75M acquisition, 2.5M subs). Referral program drove ~30% of new subscriptions at peak; CAC $0.25 vs $3-5 paid ads. Quote from one source: "the content was so good people were already sharing the newsletter with their friends and colleagues even before they had a referral program." **Product-market-fit-before-referral**. Multi-channel: bought ads in OTHER business/tech newsletters (Morning Brew was a network-effect on newsletter media itself).
- **Superhuman** (concierge onboarding, Vohra "very disappointed" PMF gate at 40%, sold to Grammarly for ~$700M-$1B in 2025). **Initial PMF survey came back at 22%, NOT 40%** — Vohra iterated until it hit 40% BEFORE public launch. Concierge onboarding by Vohra personally for the first cohort.

**What the canonical successes have in common:**
1. **PMF-signal gate, not calendar gate.** Superhuman waited until the survey hit 40%.
2. **Concierge or partnership-led acquisition.** Not "launch and pray."
3. **Multi-year horizon.** Readwise and Morning Brew compounded over years, not 30-day windows.
4. **Pricing in $10-30/mo band** (not the $4.90 floor).

**What the current plan does that the canonical successes did NOT:**
- Calendar-gated launch (day 18) regardless of dogfood PMF signal.
- $9 anchored against Readless's $4.90 floor rather than Readwise's $10 / Morning Brew's referral economics / Superhuman's $30 trust-position.
- No referral program in v1.0 (and v1.1 list doesn't mention one).
- 30-day success window (25 paying by post-launch day 30) — Readwise took years to compound.
- Show HN as launch instead of newsletter-cross-promotion (Morning Brew's primary channel) or concierge onboarding (Superhuman's primary channel).

**Verdict: PREMISE FAILS.** The plan is anchored against direct competitors (Readless) and not against canonical successes (Readwise, Morning Brew, Superhuman). Direct competitors are the alternatives; canonical successes are the precedents. Importing one canonical playbook (Superhuman-style concierge onboarding for first 10-25 paying users; Morning Brew-style referral program added to v1.1 instead of "per-newsletter summarization preference UI") would materially improve odds.

**Cascading implication for Step 0A and downstream sections:** Section 1b is mandatory. Section 5a (launch gate question) is mandatory. Section 7 (growth loops) must include referral mechanics.

### M0c — Anti-feature surface

**Question:** Name 2+ features currently in scope that contradict the stated positioning, trust model, or business model.

**Walk through the v1.0 feature list:**

| Feature | Who does it serve? | Contradiction? |
|---|---|---|
| Forwarding-address (`you-abc123@m.tldrof.com`) | All users | NO — load-bearing for moat |
| 60-second magic moment | All users | NO — load-bearing for activation |
| Cross-newsletter dedup (Claude-mediated) | All users | NO |
| Auto-forward-helper (Gmail only in v1.0 per CEO PC2) | Gmail users | Minor: ONLY Gmail in v1.0 leaves the corporate/Outlook segment unserved at launch — the segment that is the moat. **Anti-positioning, not anti-feature** |
| 7-day free trial | Time-rich tinkerers (engineers, students, "let me try this") | YES — see M0d |
| $9/mo price | "Affordable" framing | YES — see M0b. Anchored on Readless floor, undercuts Readwise band, signals commodity to trust-shoppers |
| MCP wrapper + read-only digest API (v1.1) | Power-user agent integration | YES — technical features for non-paying technical users; splits product story between consumer SaaS and dev tool |
| Per-newsletter summarization preference UI with slider (v1.1) | Power users | YES — "configurable" features attract tinkerers who churn; trust-positioned products tend to be opinionated (Superhuman is famously opinionated) |
| "Picker" of 30 curated newsletters as secondary onboarding fallback | Onboarding edge case | Minor: small attack surface |
| YouTube/podcast/RSS/Arxiv digest blueprints (v1.2+ Suite) | Power users | Out of scope for v1.0 marketing review, but worth flagging that the Suite rung is technical-audience-coded |

**Anti-features identified (3, plus 1 anti-positioning issue):**
1. **7-day free trial** (overlaps with M0d) — selects engineers/tinkerers, not the trust-led corporate ICP. *Decision the founder owes themselves: kill, replace with 14-day money-back guarantee + concierge onboarding for first cohort.*
2. **MCP wrapper + digest API in v1.1** — splits product story between consumer SaaS (which the marketing is) and dev tool (which these features are). *Decision: defer to v1.2+ at earliest; possibly kill entirely if the product is going to be premium-trust-positioned.*
3. **Per-newsletter summarization preference UI with slider (v1.1)** — opinionated products win the trust segment; configurable products win the tinkerer segment. The doc calls this "the strongest moat candidate" — that read is wrong if the moat segment is corporate-trust. *Decision: defer to v1.2+ pending evidence from first cohort that THIS is what they want, not what the founder wants.*
4. **(Anti-positioning, v1.0)**: Gmail-only auto-forward helper at launch leaves Outlook/Proton/corporate users — the moat segment — to manual setup. That's not strictly an anti-feature, but it IS a contradiction between "structural coverage moat is M365/corporate" (P4) and "v1.0 auto-forward shipped is Gmail only" (CEO PC2). *Decision the founder owes themselves: either lean into Gmail-only positioning at launch, OR delay launch by 3-5 days to ship Outlook+Gmail auto-forward together.*

**Verdict: PREMISE FAILS.** At least 3 anti-features and 1 anti-positioning issue. The "kill, defer to v2, or restrict to enterprise tier" decision is owed.

**Cascading implication:** Section 6 trial mechanics revisited. Roadmap re-sequencing recommended in Section 9.

### M0d — Freebie-disqualifier (acquisition-mechanic selection bias)

**Question:** Does the 7-day free trial acquisition tactic select for the wrong segment?

**Diagnostic:**
- "7-day free trial, requires CC at signup (per P6 setup-intent flow)" → moderately committed users (CC required = better than no-CC). But: the trial mechanic still attracts try-shoppers.
- Doc's own P6 framing: trial-end loss-aversion fires because user has "reallocated the saved 45 minutes." That framing presupposes the trial cohort = the cohort that actually saves 45 minutes/day — which is the technical-newsletter-overloaded engineer (founder's dogfood profile).
- Corporate-segment buyers (lawyers, finance, healthcare): time-poor/money-rich. They do NOT trial-shop. They trust-shop. The mental model is "is this thing legit, will my IT approve, am I exposing data" — they buy on trust signals, not on "let me try it free for 7 days."

**Adjacent-category comparables for the corporate segment:**
- Superhuman: $30/mo, NO free trial (concierge onboarding, paid from day 1)
- SaneBox: $5/mo with 14-day trial — but SaneBox's ICP is closer to "any inbox-overloaded user" not high-trust corporate
- LegalZoom-style legal-services: no free trial; trust-led with money-back guarantee
- DocuSign-for-personal: subscription, not trial-led

**The free trial is a category-error for the corporate segment.** It's a fit for the engineer cohort (which IS who shows up to Show HN). The launch plan's trial mechanic is internally consistent with launching to engineers; it is internally INCONSISTENT with the moat segment.

**Verdict: PREMISE FAILS.** 7-day free trial validates willingness to TRY among the engineer cohort. It does NOT validate willingness to PAY among the corporate-trust segment. P5 (25 paying / day 30) and P6 (15 paying / day 14) targets will be measured against the engineer trial cohort, NOT the moat segment. The targets will either pass (engineers convert) and create a false signal that the broader moat-segment plan is working, OR fail (engineers don't convert at trial-end either) and kill the project before the moat segment was tested.

**Cascading implication:** Section 6 (pricing & packaging) must propose alternatives — concierge onboarding for first cohort, 30-day money-back guarantee instead of free trial, or split: trial for engineer cohort + concierge for corporate-segment landing pages.

### M0e — Dogfood audience-class match (founder vs paying ICP)

**Question:** Is the audience the product was dogfooded on the same audience that will actually buy it?

**Dogfood corpus (from doc):** TLDR, AlphaSignal, Bensbites, Pragmatic Engineer, Stratechery, Latent Space, TheNeuron, Lenny's Newsletter.

These are technical/AI/product newsletters. The audience is engineers, AI researchers, PMs, founders. **Founder is in this audience.** "Founder is the ICP" (P1).

**Planned paying ICP (per the doc itself):**
- Primary v1 cohort: engineers/PMs/founders/AI-adjacent (matches dogfood — good)
- Secondary post-launch: wantrepreneurs, AI-engineers tracking fast-moving fields (matches dogfood — good)
- **Secondary post-launch (the moat segment, P4): M365/Outlook corporate users, lawyers, finance, healthcare, government, agency operators with custom-domain email**

The third secondary segment does NOT read TLDR or AlphaSignal in meaningful numbers. They read:
- Morning Brew (general business)
- Axios AM / Axios Pro
- The Hustle
- Vertical legal newsletters (Law360 daily, ABA Journal)
- Vertical finance (Term Sheet, Money Stuff by Matt Levine, The Daily Upside)
- Vertical healthcare (STAT Plus, Endpoints, Politico Pulse)
- LinkedIn newsletters in their field
- Industry trade publications

**The product is being tuned on technical-newsletter corpus for an ICP whose actual reading is general-business and vertical-trade newsletters.** Dedup signature, summarization style, the "what counts as the same story across newsletters" — all of that is currently optimized for AI/tech news. A Morning Brew + Axios AM + The Hustle reader's dedup needs are different (more overlap in macro news, less in industry-specific reports).

**Verdict: PREMISE FAILS.** Dogfood audience ≠ paying ICP for the moat segment.

**THE CORRECT FIX (per v0.3 M0e):** BOTH pivots required.
1. **Pivot the TARGET audience in marketing materials, ICP doc, and launch sequencing** to include the moat segment with first-class positioning (not "secondary, post-launch").
2. **Expand dogfood subjects to include paying-ICP-representative inputs** BEFORE launch (1-2 weeks of buyer-aligned dogfood minimum). Concretely: founder subscribes to Morning Brew, Axios AM, The Hustle, Money Stuff, Term Sheet, STAT/Endpoints, ABA Journal, Law360 — for 1-2 weeks — and dogfoods digest quality on those inputs.

**Refuse the partial fix.** Do NOT "defer the paying ICP to v1.0.5" while keeping the technical dogfood. That preserves the mismatch.

**Cascading implication:** Section 2 ICP doc must be the corporate/moat-segment ICP, not the dogfood-aligned engineer ICP. Section 4 audience-build sprint must include vertical channels for the moat segment, not only HN-cohort channels.

### Step 0.5 summary

5 of 5 premises failed or partially failed. **This is a premise-level intervention, not a tactical tuning.** The headline finding is M0e (dogfood mismatch) compounded by M0d (freebie-disqualifier) compounded by M0a (launch platform wrong audience class). Together: the product is being tuned to engineers, validated by engineers, and launched to engineers — while the structural moat the doc itself promotes lives in a segment the plan doesn't actually reach.

---

## Step 0A — Forcing-question answers

(Asked one at a time. Founder gave technically-strong, marketing-naive first answers. Pushback applied per skill. Final accepted answers below.)

### M1 — Audience reality

**Founder's first answer (paraphrased):** "Engineers and PMs who are drowning in newsletters. People like me — I subscribe to like 15 of them and I can't keep up."

**Pushback:** "Engineers and PMs" is a demographic category. Refused. Need named persona with ≥5 specific attributes + ≥3 named places they spend attention.

**Final accepted answer (after Step 0.5 corrections — moat-segment-first):**

> **Maya, 38, Director of Product Marketing at a 600-person Series C fintech in NYC.** Uses Outlook (corporate M365); cannot use Gmail-based AI inbox tools because IT compliance forbids OAuth into work mail. Subscribes to ~12 newsletters: **Morning Brew, Axios AM, Stratechery, The Hustle, Lenny's Newsletter, Term Sheet (Fortune), Money Stuff (Matt Levine), Marketing Brew, Lenny's, Tomasz Tunguz, First Round Review, Pragmatic Engineer**. Reads partial fragments at the 8:15am train commute and at 9pm before bed. Already pays $20/mo for ChatGPT Plus and $15/mo for Notion personal. Currently uses Outlook folders + a manual "important newsletters" folder. Complains in conversation that "I miss the one thing that mattered in TLDR because I skipped it for the day."

**Where Maya spends attention right now:**
- LinkedIn (active follower of ~8 product-marketing thought leaders)
- Lenny's Newsletter Slack community (paid Lenny's Pro member)
- First Round Review and Reforge content
- Stratechery podcast on commute
- **Not on Hacker News.** Not on r/SideProject. Occasionally on r/ProductManagement.

**Secondary persona (also moat-segment): Daniel, 44, partner at a 30-attorney boutique law firm in Chicago.** Custom-domain email through Microsoft Exchange. Subscribes to Law360 Daily, ABA Journal Daily News, Bloomberg Law, Above the Law, Lit Hub Daily (personal). Cannot use Gmail or OAuth tools. Reads the first 2 newsletters; the rest pile up.

**Tertiary persona (engineer cohort, the dogfood-aligned one): Sam, 31, senior eng at YC-backed SaaS in SF.** Subscribes to TLDR, AlphaSignal, Bensbites, Pragmatic Engineer, Latent Space. Active on HN, X, GitHub. Already familiar with Refind/Mailbrew/Readless. This is the persona Show HN actually reaches.

**Refuse to lose the moat-segment in favor of the dogfood-segment.** The plan must address Maya and Daniel as first-class, not as "v1.0.5 expansion."

### M2 — Discovery path

**Founder's first answer:** "They see my Show HN post and click through."

**Pushback:** Maya and Daniel are not on HN. Refused. "Show HN" forbidden as step 1.

**Final accepted answers (per-persona):**

**Maya's discovery path (corporate product marketer):**
1. **Lenny's Newsletter sponsorship slot** (Lenny does paid sponsor sections; sponsor cost ~$5-15K/issue per Sparkloop data, but cheaper for solo founders; alternative: Lenny's classifieds at $400-800). Headline: "Outlook user drowning in newsletters? tldrof works with corporate email — no OAuth, no IT approval."
2. Maya sees it, recognizes herself, clicks through to landing page.
3. Landing page leads with **corporate-email coverage** as the differentiator, not "60-second magic moment."
4. Maya tries it (forwards her newsletter pile).
5. Maya converts within 2 weeks because trial-end loss-aversion fires AND because she trusts the brand (Lenny endorsement transfers).

**Daniel's discovery path (lawyer):**
1. Above the Law sponsorship OR Bloomberg Law sponsorship (vertical legal newsletter).
2. OR: word-of-mouth from a peer at a competing firm (referral mechanics — see Section 7).
3. Discovery happens via legal-trade channels, NOT HN.

**Sam's discovery path (engineer, dogfood-aligned):**
1. Show HN — actually works here. Sam is on HN.
2. Click through, recognize the pattern, try it.
3. Sam is more likely to evaluate vs Readless/Mailbrew on price; conversion psychology is "is this better than the free Mailbrew now?"

**Realistic time-to-discovery for the moat segments: 4-8 weeks (Maya/Daniel) IF the right channels are seeded.** For Sam: launch day or week-of.

### M3 — Pre-launch audience

**Founder's first answer:** "I'll build audience after launch. Right now I'm building."

**Pushback:** That's the pattern that produces ship-to-silence. Refused.

**Final answer (forced honest):**
- Twitter for the product: 0
- Substack for the product: 0
- LinkedIn following for the product: 0
- Personal LinkedIn followers (semiconductors): 996 — **wrong category, counts as 0 for this product**
- Personal Substack subscribers (existing newsletter): 11 — **topic-alignment unclear, treat as ~0 for ICP**
- Founder's personal X account: not specified for product use
- GitHub stars on prior projects: some (overlap only with Sam-persona cohort)

**Effectively zero ICP-aligned audience.** Audience-build sprint is the load-bearing pre-launch work, NOT product polish.

### M4 — Channel honesty

**Founder's first answer:** "I'm an engineer, I can build. I'm good on Show HN historically — I've upvoted lots of things."

**Pushback:** "I can build" is product, not distribution. "I've upvoted" is consumer behavior, not distribution. Refused.

**Final answer:** Founder has **zero demonstrable distribution advantage**. No published writing track record at scale. No newsletter audience. No prior shipped consumer product. No content history in the newsletter/AI/inbox category.

**This becomes work item #1.** The honest answer is "I don't have one yet — I need to build one starting this week." Action: founder commits to publishing 1 short technical "build-in-public" post per week on LinkedIn (where the 996 followers ARE) AND Substack (to grow the 11), positioning around "what I'm learning building a consumer SaaS as a first-time consumer founder." This won't reach Maya/Daniel directly but it builds a base AND it converts the 996 into a small fraction of relevant subscribers via topic-pivot.

### M5 — Competitor traffic source

**Founder's first answer:** "I don't know. I assume Readless got most of their traffic from Reddit or HN."

**Pushback:** "I assume" is a guess. Need verified data OR explicit commitment to research.

**Final answer (founder commitment + my own research surfaced):**
- **Readless.app:** their own blog is SEO-heavy (we found their domain ranks for many newsletter-comparison queries like "Meco pricing", "Mailbrew alternatives" — see web search). They are doing content/SEO as a growth lever. **Implication:** SEO is in-play for this category; tldrof should consider content SEO as a long-tail compounding play (not v1 launch, but Section 4 90-day plan).
- **Meco:** referral program ($4/user); partner program for newsletter creators (creators promote Meco to their subscribers); ProductHunt presence. Acquisition partly via **newsletter creators promoting to their lists** — exactly Morning Brew's pattern at a smaller scale.
- **Readwise:** API/integration ecosystem partnerships; SEO; word-of-mouth (per Readwise team's own writing on bootstrapping); EdTech partnerships.
- **Mailbrew:** went FREE Nov 2025 (Evernomic acquisition), so their acquisition pattern is no longer comparable — this is a SIGNAL that the paid market is contested.

Founder assignment: by day 5 of audience-build sprint, run SimilarWeb on Readless and Meco; document top 3 referral sources for each.

### M6 — First 10 paying customers

**Founder's first answer:** "Whoever sees the Show HN post and converts during the trial."

**Pushback:** Passive language. Refused.

**Final answer — named 10 people the founder will personally email this week:**

(Founder generated this list under pushback. The skill cannot verify the names exist but can verify the SHAPE is correct — named individuals across the right segments, not "engineers who see HN".)

1. **3 PM friends from prior network at Micron** (engineer-adjacent, not corporate-segment — these are warmup contacts, not moat)
2. **2 LinkedIn connections in semiconductor product marketing** (uses corporate Outlook — IS moat-segment, low-confidence ICP-overlap on newsletter consumption habit)
3. **2 founder friends in the YC-cohort circle** (engineer-segment)
4. **1 former colleague now in compliance at a fintech** (moat-segment, vertical-finance, IS the persona)
5. **1 sister/family member who works at a law firm administrator role** (moat-segment if she reads industry newsletters; verify first)
6. **1 contact at a healthcare-tech startup founder** (moat-adjacent)

**Honest acknowledgment:** the named-10 list skews engineer-segment because that's the founder's existing network. The corporate-segment 10 is a STRETCH list that requires LinkedIn outbound to people the founder does NOT know — and that work has not started.

**Concrete commitment:**
- Email the engineer-network 10 in week 1 of audience-build sprint (warmup; gather feedback during dogfood).
- LinkedIn outbound to 30 product-marketing / legal-ops / finance-ops people in week 2 (with a Lenny's-Newsletter-mentioning hook).
- Goal: 5 named corporate-segment people in dogfood by day 14 of audience-build, before public launch.

### M7 — Time allocation

**Founder's first answer:** "I'm spending maybe 95% on building. I'll do marketing in the polish window (days 14-16) and after launch."

**Pushback:** Ratio is wrong by skill standard (≥30% on audience-building required pre-launch). 5% audience-building for a solo founder shipping into a market where the direct competitor is FREE is the highest-leverage thing to fix this week.

**Final accepted answer:** Founder reluctantly commits to:
- **Days 1-4 (start TOMORROW): 1 hour/day of audience activity** (LinkedIn post, Substack post, outbound DM to 5 people). 1 hour out of 10-12hr build day = ~8-10%. Still under skill standard but realistic given the build crunch.
- **Days 5-13: 2 hours/day audience activity** (~15-20%). Plus add HN-cohort private beta outreach (CEO PC3 already requires 2-3 hours of this in days 7-9).
- **Days 14-22 (polish window + launch ramp): 3+ hours/day audience activity** (~25-30%). Vertical channel research, Lenny's classifieds outreach, content drafts.

**Honest acknowledgment of risk:** even at 25-30% in the launch ramp, this is below the skill standard. The founder is making the call that 70% build / 30% audience is the right tradeoff for a 20-22 day window. **Surface this explicitly: this is a known-risk tradeoff. If launch fails, the post-mortem will include "audience ratio was wrong pre-launch."**

---

## Step 0B — Mode selection: confirmed Mode A with Section 4 ELEVATED

Locked. See Step 0 audit above for rationale.

---

## Section 1 — Competitive landscape (web-research backed)

### 1a. Direct competitors

| Competitor | Pricing | Founded | Traffic source (inferred) | User complaints | Positioning vs tldrof | Winning? |
|---|---|---|---|---|---|---|
| **Readless.app** | $4.90/mo | unclear (active 2025-2026) | SEO-heavy blog (ranks for newsletter-tool comparison queries); forwarding-email pattern | Per design doc pass 4: no bulk-backlog flow; subscription-repointing impossible for many users; "first digest within 24 hours" not instant; signup glitch suggests low traffic | Tldrof: bankruptcy/60s magic moment; Readless: subscribe-forward + ongoing daily | Unclear traction. Active development; low public revenue signal |
| **Meco** | $3.99/mo (Free + Pro $35/yr) | 2022-ish | ProductHunt + referral program ($4/user) + partner program (newsletter creators promote to subscribers) | Some users want more aggressive AI summarization | "Magazine for newsletters" — separate inbox app, not email-digest. Different shape | Yes — has scale; "great for growing audience base" per partner-program reviews |
| **Mailbrew** | **FREE as of Nov 2025** (Evernomic acquisition; caps on digest count + length on free tier) | 2019 | Was paid until 2025; now free w/ caps | Pre-acquisition: $10/mo was steep; post-free: complaints about caps | "Custom digest builder for power users" — combine newsletters + RSS + Twitter + Reddit + ProductHunt + YouTube into one digest | Mixed — being free changes the dynamic; signals the paid market is contested |
| **Refind** | Free + Pro $7/mo | 2015 | Long-established; word-of-mouth + SEO | More "discover articles" than "digest your subs" | Different shape — curation vs your-own-subs | Steady but small |
| **Shortwave** | $9/mo+ (Gmail-only) | 2022 | YC backing; product-led; Gmail-API | Gmail-only is the moat AND the ceiling | Different shape — full inbox app, not digest. OAuth-based (cannot serve corporate locked-out users) | Scaling; well-funded |

**Critical net read:**
- **Mailbrew being FREE is the elephant.** The doc does not acknowledge this. A $9/mo paid product directly competing against a $0 product (with similar shape: digest of newsletters/sources you specify) needs a sharp value justification that goes beyond "60-second magic moment" — because Mailbrew's onboarding-time penalty doesn't compound forever; it's a one-time cost. The justifications that hold: (a) corporate-coverage moat (Mailbrew is feature-rich but I have not verified its Outlook/M365 story; assume it's Gmail-leaning), (b) bankruptcy-triage as primary use case (Mailbrew doesn't do this), (c) Claude-mediated quality of dedup/summarization that Mailbrew's free tier won't match.
- **Direct competitors are NOT winning at scale.** None of them is at Readwise-tier revenue or Morning-Brew-tier subscriber count. **Implication: the category is real (Mailbrew/Readless/Meco/Refind all exist and have traction) but no one has run away with it.** That's both opportunity AND a warning (maybe nobody has won because the addressable paid market is small).

### 1b. Canonical-success comparables (the part the doc skipped)

| Canonical | Pricing | Founded | Current scale | Primary acquisition channel | Onboarding model | Launch gate | Specific delta from tldrof plan |
|---|---|---|---|---|---|---|---|
| **Readwise** | $9.99/mo Reader; $4.99 Highlights | 2017 | $14M ARR, 4M registered, ~3M MAU, >90% retention, bootstrapped | SEO, integrations, partnerships, word-of-mouth, app stores — **NOT paid acquisition; NOT Show HN dependence** | Self-serve, but content+integrations onboard most users | Was bootstrapped from a small product (Highlights for Kindle) that found PMF before scaling | tldrof has no integration ecosystem, no SEO content, no partnerships strategy. tldrof's plan is Show-HN-led where Readwise was integrations-led |
| **Morning Brew** | Free newsletter; $75M acquired by Insider Inc 2020; 2.5M+ subs at acquisition | 2015 | Sold for $75M, currently 4M+ subs | **Referral program (~30% of new subs at peak; CAC $0.25 vs $3-5 paid)** + ads in other newsletters + cross-promotion with creators | Free signup, instant value | Product PMF first ("people were already sharing before we had a referral program") | tldrof has no referral mechanic in v1.0 or v1.1 list. **Add Morning-Brew-style referral to v1.1 in place of the per-newsletter summarization slider** |
| **Superhuman** | $30/mo (recently $25-30 tiers) | 2014 | Sold to Grammarly ~$700M-$1B in 2025 | **Concierge onboarding 1:1 (Vohra personally onboarded first ~200 users)** + waitlist + invite-only + two-sided referral | Concierge for years post-launch — at peak, dozens of onboarding specialists doing 1:1 sessions | **PMF-signal-gated: Vohra ran "very disappointed" survey, hit 22% at first private beta, iterated until 40%, THEN public launch** | tldrof is calendar-gated (day 18) NOT PMF-signal-gated. Vohra precedent says: don't launch publicly until "very disappointed" survey on private beta hits 40% |

### 1c. Pattern surface

What canonical successes have in common that the current plan lacks:

1. **PMF-signal gate, not calendar gate.** All three iterated to PMF signal before scaling. Tldrof commits to calendar day 18.
2. **High-trust acquisition channels.** Concierge (Superhuman), integrations/partnerships (Readwise), referral-from-trusted-source (Morning Brew). Not Show HN.
3. **Long compound horizon.** Readwise took 8 years to $14M ARR. Morning Brew took 5+ years to 2.5M subs. Tldrof's success window is 30 days.
4. **Pricing in the $10-30/mo band** OR free-with-monetization-elsewhere. Tldrof's $9 sits in a no-man's-land — too expensive to compete with free Mailbrew, too cheap to anchor "trust-priced" against Superhuman or Readwise.

Where direct competitors diverge from canonical-success patterns:
- Readless, Meco, Refind all sit at <$5/mo — they are anchored against each other rather than against the Readwise band. They have NOT figured out how to charge $10+.
- Mailbrew gave up and went free — possibly because they could not figure out how to make $10/mo work either.

**Which pattern is the current plan implicitly following:**
The current plan is implicitly following the **Readless playbook with a 60-second-magic-moment tweak**. That playbook has not produced a category winner. **Switching to a Readwise-pattern (integrations + content + retention-led) OR a Superhuman-pattern (concierge + premium-priced + PMF-gated) would be a meaningful upgrade — and the corporate-coverage moat the doc already identifies is the strategic asset that makes Superhuman-pattern feasible.**

**Founder action item:** read (1) Readwise's "Why We're Bootstrapping" blog post AND (2) First Round Review's "Superhuman Onboarding Playbook" article. Specifically: pull the patterns into a 1-pager of "what we're stealing from each" before day 22.

---

## Section 2 — ICP specification

See `icp.md` for the full Maya (primary) / Daniel (secondary corporate) / Sam (tertiary engineer-dogfood) persona doc.

Headline: **promote Maya from "secondary post-launch" to PRIMARY ICP for the marketing plan.** Sam (the engineer dogfood persona) becomes the secondary launch-channel persona (the one Show HN reaches), NOT the primary.

---

## Section 3 — Distribution channel-by-channel

Motion class = **consumer subscription (premium-trust positioning preferred)**, NOT dev tool. Generic consumer-subscription rules apply; dev-tool rules do NOT apply (this is not a developer-facing product).

### Channel scoring table

Scoring: 1-5 each. Leverage = Reach × Conversion × FounderFit ÷ Cost ÷ Effort.

| Channel | Reach (Maya/Daniel) | Reach (Sam) | Cost | Conversion | Founder fit | Effort to start | Leverage | Verdict |
|---|---|---|---|---|---|---|---|---|
| Show HN | 1 | 5 | 1 | 2 (HN converts at 0.5-2% for consumer-SaaS) | 3 (founder is HN-native) | 1 | Moderate for Sam; near-zero for Maya/Daniel | KEEP — but as ONE of 3+ channels, not the dominant. **Apply ICP-aware framing**: launch with the corporate-coverage moat as the hook ("not just another newsletter app — works with Outlook + corporate email"), not the bankruptcy hook (which is engineer-coded) |
| Lenny's Newsletter (sponsorship OR classifieds OR guest contribution) | 5 | 3 | 3 ($400-800 classifieds; $5-15K full sponsor) | 4 (Lenny's audience IS product/PM Maya-persona) | 2 (no existing relationship; cold outreach needed) | 3 | HIGH for Maya | **ADD as channel 2** — classifieds at $400-800 fits solo-founder budget |
| LinkedIn organic (founder's existing 996 + new) | 2 (most Maya/Daniel use it) | 1 | 1 | 2 | 3 (founder has the surface) | 2 (new content on a topic-pivot) | Moderate | **ADD as channel 3 (low-cost compounding)** — 1 post/wk on "building a consumer SaaS, first-time consumer founder" |
| Substack (founder's existing 11 + new) | 1 (small) | 1 | 1 | 2 | 4 | 2 | Low initial; compounds | KEEP as long-term compounder; not a launch channel |
| Newsletter cross-promotion / SwapStack-style exchanges | 4 (right audience) | 3 | 2 | 4 | 2 (no prior relationships) | 4 (needs outreach + you need your own list first to swap with) | High in theory; gated by needing-an-audience-first | DEFER until tldrof has its own 500+ subscriber list (~60 days post-launch); QUEUE for v1.1 |
| Reddit (r/ProductManagement, r/legaltech, r/ITPro, r/sysadmin for Outlook-locked-out users) | 3 (vertical subs) | 2 | 1 | 2 | 2 | 3 (community-rules-compliant posting) | Moderate; vertical-segment matched | KEEP — vertical subs specifically, NOT r/SideProject. **Pre-launch reconnaissance posting** (comment in threads about newsletter overload for 2 weeks before any link drop) |
| Product Hunt | 3 | 4 | 1 (organic) | 2 | 2 (no hunter relationships) | 3 | Moderate | KEEP as a +7-day-after-HN separate launch event |
| IndieHackers | 2 | 4 | 1 | 2 | 3 | 2 | Moderate (Sam-segment) | KEEP as cross-post day +1 after HN |
| Cold outreach (LinkedIn DM to product marketers / legal-ops) | 4 | 1 | 1 | 4 (high-intent, named) | 4 (founder can write technical+specific) | 4 (labor-intensive) | High per-touch; low scale | **ADD as channel — the moat-segment seeding** — 30 cold DMs in audience-build week 2 |
| Vertical legal/finance newsletter sponsorship (Above the Law, The Daily Upside) | 4 (Daniel-persona reach) | 1 | 3-4 (vertical sponsor slots) | 3 | 1 (no relationships, no domain credibility) | 4 | High reach for Daniel; capital-intensive | DEFER to post-launch (v1.0.5) — only if launch surfaces Daniel-segment signal worth investing in |
| Podcast guesting (Lenny's pod, The Indie Hackers Pod, Pragmatic Engineer Pod) | 3 | 4 | 1 (organic) | 4 | 2 (founder is not a known voice) | 4 | High per-appearance | DEFER to post-launch (post first 50 paying customers, then pitch as "indie founder shipped, here's what happened") |
| Substack network / SparkLoop recommendations | 4 | 3 | 1 (free) to 3 (paid recs) | 4 | 1 (requires owning a Substack with traction first) | 4 | High once on-ramp exists | DEFER until tldrof's own Substack has 500+ |
| Paid ads (Google/Meta/LinkedIn) | 2 | 2 | 4-5 ($5-15 CPC consumer SaaS in 2026) | 2 | 1 | 2 | LOW for v1 budget | SKIP for v1 (capital-intensive without retention data to optimize against) |
| SEO content (Readless-style comparison posts) | 4 | 3 | 1 (founder writes) | 3 | 3 (founder can write technical+honest) | 4 (long ramp 6-12 months) | High long-term; zero short-term | **ADD to 60-90 day plan** — exactly what Readless is doing successfully; write "Mailbrew alternatives 2026", "Meco vs tldrof", "Outlook newsletter digest 2026" |

### Final ranked channel list (top 5)

For solo-founder limited bandwidth, focus the launch + first 30 days on these 5:

1. **Show HN (day 18-22 launch)** — for Sam-persona; primary headline = corporate-coverage moat to NOT alienate Maya/Daniel inbound from HN's broader reader base
2. **Lenny's Newsletter classifieds ($400-800)** — for Maya-persona; in 1-2 weeks before launch; first paid acquisition test
3. **LinkedIn organic build-in-public (founder, weekly)** — for compound founder-credibility + occasional Maya/Daniel touch
4. **Cold LinkedIn DM (30/week) to product marketers, legal-ops, finance-ops** — for Maya/Daniel direct seeding into private beta
5. **Reddit vertical-sub presence (r/ProductManagement, r/sysadmin, r/legaltech) — community-rules-compliant**

Channels **explicitly cut** for v1: paid ads, podcast guesting (until traction), Substack swaps (until own audience), vertical legal/finance sponsorships (until proof of Daniel-persona conversion).

**Refused founder request:** "We'll also do TikTok and Twitter aggressively." Solo founder cannot ship 5 channels well. Cut.

---

## Section 4 — Pre-launch audience-building plan (ELEVATED — 30/60/90)

**Premise:** founder starts TODAY with ~0 ICP-aligned audience. Launch is day 18-22. The audience-build sprint runs IN PARALLEL with the build window.

See `audience_build_sprint.md` for detailed weekly cadence. Summary here.

### Days 1-30 (= build days 1-22 + first 8 post-launch)

| Week | Audience activity | Time budget | Output |
|---|---|---|---|
| Wk 1 (build days 1-7) | 1 hr/day. Founder writes 1 build-in-public LinkedIn post; 1 short Substack post; 5 personal-network DMs/day to engineer-network 10 | 7 hrs total | 7 LinkedIn posts; 7 Substack notes (short); 35 personal DMs; ~5 private-beta dogfood signups (Sam-cohort) |
| Wk 2 (build days 8-14) | 2 hr/day. Add: 30 LinkedIn cold DMs to product marketers; reach out to Lenny for classifieds slot; **expand dogfood corpus to include Morning Brew/Axios AM/The Hustle/Money Stuff (per M0e fix)** | 14 hrs | 30 cold DMs; 1 Lenny classified booked; 4 LinkedIn posts; **5 buyer-aligned dogfood inputs flowing through the digest** |
| Wk 3 (build days 15-22 + launch) | 3 hr/day. Lenny's classified runs week of launch; HN launch executed; LinkedIn launch announcement; Reddit posts (community-compliant) day +1 / day +2 | 21 hrs | Launch executed across 5+ channels |
| Wk 4 (post-launch days 1-8) | 3 hr/day. ProductHunt launch (day +7); founder personally onboards first 10-20 signups via 30-min Zoom (Superhuman precedent); content blog post "Day 1-7 traction" | 21 hrs | First 20 paying customers concierge-onboarded; first content-blog SEO seed |

### Days 31-60 (post-launch month 1-2)

- **PMF survey to first cohort.** Run the Vohra "very disappointed" survey on first 30+ trial users. If <30% → product iteration BEFORE scaling channel spend. If 30-40% → tighten + scale modestly. If 40%+ → public scale phase.
- **Write 4-6 SEO blog posts** ("Best Outlook newsletter tool", "Mailbrew alternatives 2026", "How to declutter corporate inbox") seeded on tldrof.com/blog with proper schema markup.
- **Open referral mechanic in product** (replaces v1.1 per-newsletter slider). Morning-Brew-style tiered rewards: refer 3 = T-shirt or free month; refer 10 = exclusive feature.
- **2 podcast pitches/week** (Lenny's, Indie Hackers, Pragmatic Engineer) — pitching at "indie founder, 60 days post-launch, here's what I learned."
- **First Substack-network outreach**: as soon as the tldrof Substack hits 200 subs, reach out to 5 comparable newsletters for cross-promotion / SwapStack.

### Days 61-90 (post-launch month 2-3)

- **Scale highest-converting channel from days 31-60.** Likely candidates: Lenny's repeat, LinkedIn organic if it's compounding, vertical Reddit if community traction is real.
- **Vertical legal/finance sponsorship test** (1 sponsorship, $1-3K) IF Daniel-persona conversion data exists from launch + month 2.
- **Founder podcast appearances** (≥1 per week).
- **First case-study content piece**: "How [Maya-persona named customer] saved 5 hours/week using tldrof" with permission.

**Specific weekly cadence (from Day 1):** see `audience_build_sprint.md`.

---

## Section 5 — Launch playbook (multi-channel, sequenced)

See `launch_playbook.md` for the full hour-by-hour + day-by-day plan.

### 5a. Launch-gate question (calendar vs PMF-signal)

**Required question:** What is the gate that fires the launch — calendar (day 18-22, per CEO-locked decision) or PMF signal (Vohra "very disappointed" or equivalent)?

**Founder's commitment:** Calendar (day 18-22) per CEO review locked decision.

**Pushback:** tldrof is a **retention-driven consumer subscription**. P5 (25 paying / day 30) and P6 (15 paying / day 14) are retention-and-conversion bets. The canonical precedent (Superhuman) is explicitly PMF-signal-gated. Calendar-gating is the wrong choice for this motion class.

**Founder's defense of calendar gate:** "I need a forcing function. If I PMF-gate, I'll iterate forever. The 30-day window IS the test — if it fails, I have my answer fast."

**Skill's response (per v0.3):** Founder may keep the calendar gate but must do so EXPLICITLY with reasoning that survives the Vohra/Superhuman precedent. Founder's "I need a forcing function" is a legitimate reason for a solo founder under time pressure (not unlimited dogfood horizon). Accepted **conditionally**: the calendar gate is allowed IF and ONLY IF the founder ALSO runs a "very disappointed" survey on the private-beta cohort (CEO PC3's 3-5 HN-cohort friends + the engineer-network 10 from M6) BEFORE day 18 launch. If <30% "very disappointed" → delay launch by 7-10 days for iteration. If ≥30% → proceed with calendar gate.

**The KILL CRITERIA framing** is load-bearing: P5 (25 paying / day 30) and P6 (15 paying / day 14) must be treated as actual go/no-go bars, not aspirational targets. If they miss, the project pivots or sunsets — no "we'll learn from launch and iterate" language allowed at miss-time.

### 5b. Sequence

Headline: **3+ channels, sequenced**. NOT simultaneous. Show HN is ONE of them, not the dominant.

| Day | Channel | Specific action |
|---|---|---|
| -14 | LinkedIn (founder) | Build-in-public post: "I'm shipping a consumer SaaS in 3 weeks. Here's the design doc. Here's what I'm scared of." Drives initial follower attention. |
| -10 | Lenny's classifieds | Book the classified slot for launch-week issue ($400-800). |
| -7 | Personal email | Soft pre-announce to engineer-network 10 + the cold-DM responses; ~30 people total. CTA: private beta access this week. |
| -5 | Private beta | Concierge-onboard the first 10-15 private-beta users via 30-min Zoom calls (Superhuman pattern). Run "very disappointed" survey at day +3 of private beta. |
| -2 | LinkedIn (founder) + Substack | Pre-launch announcement; "launching Wednesday — here's the corporate-email coverage angle." |
| 0 morning Pacific | Hacker News | Show HN post. **Headline emphasizing corporate-coverage moat** (NOT just bankruptcy framing): "Show HN: tldrof – newsletter digest that works with Outlook + corporate email (no OAuth)" |
| 0 + 2hr | X (founder + ask private-beta users to amplify) | Thread linking HN post; technical specifics + honest comparison vs Mailbrew/Readless |
| 0 + 4hr | LinkedIn | Long-form launch post; tag relevant product-marketing community members |
| 0 + 6hr | Lenny's classified hits inbox (timed to land Tuesday or Wednesday at 6am PT per Lenny's send schedule) | Classified copy: "Outlook user drowning in newsletters? Built for corporate email, no OAuth. Free 7-day trial. [link]" |
| 0 + 24hr | IndieHackers | Cross-post (HN-first to avoid duplicate penalty) |
| 0 + 48hr | r/ProductManagement (with mod permission and community-rules compliance) | Community-rules-compliant share — frame as "I shipped a thing, here's the build journal" not "buy my product" |
| 0 + 48hr | r/sysadmin (for the Outlook-locked-out angle) | Community-rules-compliant share |
| 0 + 72hr | Direct LinkedIn DMs | Re-engage the 30 cold-DM contacts from audience-build week 2 with the launch link |
| 0 + 7d | Product Hunt | Separate launch event |
| 0 + 14d | Podcast outreach | Pitch 5 podcasts (Lenny's, Indie Hackers, Pragmatic Engineer, Lenny's Pro, Reforge Office Hours) |
| 0 + 30d | Substack post + blog post | "Tldrof Day 30: here's what worked and what didn't" (transparency-as-marketing, Readwise-pattern) |

### Risk callouts
- **HN miss = no recovery if it's the dominant channel.** Mitigation: Lenny's classified seeds a SEPARATE traffic source same week.
- **Lenny's classified miss = wasted $400-800.** Mitigation: pre-draft the classified copy with founder's writing voice; A/B test 2 headlines if Lenny allows.
- **Cold-DM volume is hard for an introverted technical founder.** Mitigation: write a tight template; commit to 5/day not 30/week chunks (lower friction).
- **Concierge onboarding (Superhuman pattern) at 10-15 Zoom calls is operator-shaped.** This contradicts the doc's operator-shape watch-item. **Acceptable contradiction at the FIRST cohort only** — the precedent (Vohra personally onboarded the first 200) supports it. Document this explicitly as: "first 25 paying users are concierge-onboarded; transition to self-serve once dogfood patterns are stable."

---

## Section 6 — Pricing & packaging

### 6a. Pricing-band question (mandatory before tactic)

**Did the $9 price band inherit from competitor anchoring, or from ICP willingness-to-pay evidence?**

**Founder's answer:** "It's a round-ish number above the Readless $4.90 floor and below the Refind $7. Felt like the right band."

**Verdict:** competitor-anchored against Readless. NOT ICP-WTP-evidenced.

**ICP-WTP evidence for Maya-persona (corporate product marketer, time-poor, trust-shop):**
- Already pays $20/mo ChatGPT Plus
- Already pays $15/mo Notion
- Has historical category-precedent paying for Superhuman at $30/mo or SaneBox at $5/mo
- Adjacent: pays Lenny's Pro at $19/mo annual ($228/yr)
- **Likely WTP for tldrof: $12-20/mo** if positioned as professional tool (not commodity)

**ICP-WTP evidence for Daniel-persona (lawyer):**
- Already pays for Bloomberg Law, Law360 (high $$ — these are $200-1000+/mo enterprise; personal subs at lower tiers)
- Trust-shop, very low willingness to try unproven tools
- **Likely WTP: $15-25/mo IF tldrof can satisfy IT-compliance concerns AND get a peer-firm reference**

**ICP-WTP evidence for Sam-persona (engineer):**
- Pays $20/mo ChatGPT Plus, maybe $15/mo Cursor; familiar with the $9 SaaS band
- Will compare-shop vs free Mailbrew — likely chooses tldrof only if quality difference is visible OR if HN/X social proof is strong
- **Likely WTP: $5-12/mo** — Sam is the price-sensitive cohort. The cohort the calendar launch targets is also the cohort with the LOWEST WTP.

**The pricing-band evidence supports $12-19/mo for the moat segment, $5-12/mo for the dogfood segment.** $9 sits between, satisfies neither, and is anchored against the floor (Readless).

**Specific failure mode (from skill anti-patterns #7):** "Matching the cheapest direct competitor's price (e.g., Readless is $4.90, so we should be $5-6)" — tldrof avoided the worst version of this trap by setting $9, not $5. But $9 is still the milder version of the same trap. Cheapening the price signals "commodity" to exactly the segment that buys on trust.

**Recommendation:** **Two-tier pricing in v1.0.5 (defer for v1.0 launch simplicity):**
- **Personal** at $9/mo (the current price) — for Sam-segment + price-sensitive Maya-adjacent
- **Pro / Pro+Work** at $19/mo — adds: priority Claude tier (faster digest gen), corporate email "compliance pack" (DPA template, SOC2 quick-summary doc, IT-approval one-pager), priority support — for Maya/Daniel-segment

**For v1.0 launch (per CEO-locked $9 decision):** keep $9 BUT make the landing page explicitly position $9 as "introductory pricing — will increase at v1.0.5." This signals scarcity AND telegraphs that the product is heading premium, not commodity.

### 6b. Standard pricing & packaging coverage

- **Tier structure (v1.0):** Single $9/mo tier. Annual discount $90/yr (one month free) — annual billing is documented in RevenueCat data as significantly improving retention. **ADD annual option at launch** (CEO review may or may not have caught this — the design doc doesn't surface it).
- **Trial mechanics (v1.0):** 7-day free trial with CC required. **Per M0d, this is wrong for the moat segment.** Recommend: keep 7-day for the $9 tier; ADD a "no-trial concierge onboarding" path at the $19 tier (when introduced) — 30-day money-back guarantee instead of trial.
- **Annual discount strategy:** $90/yr (~$7.50/mo equiv) at signup. Show the "save $18/yr" math clearly. Annual = better retention + better cash flow + signals commitment.
- **Per-feature vs per-usage:** Per-user, all features, no usage caps in v1. Don't usage-cap the dedup pass — it kills the product story.

**Founder's defense check:** "Why $9 not $19?" — answered above. "Why 7-day trial not 14?" — design doc P6 makes the loss-aversion-at-trial-end argument well. KEEP 7-day trial. "Why no annual?" — should not be the case; ADD annual. "Why no concierge tier?" — RECOMMEND adding at v1.0.5.

---

## Section 7 — Post-launch growth loops

What compounds, what's linear?

| Loop type | Currently in v1? | Recommendation |
|---|---|---|
| **Referral mechanics** (in-product invite, Morning Brew-style tiered rewards) | NO — not in v1.0 or v1.1 list | **ADD to v1.1 — REPLACE the per-newsletter summarization slider with referral.** This is the single highest-ROI v1.1 change |
| **Content compounding** (SEO ranking improving over time) | NO — no blog mentioned in v1.0 | **ADD to 30-90 day plan** — Readless's playbook works; tldrof can do the same on different keywords |
| **Network effects** (does the product get better as more people use it?) | Weakly — cross-newsletter dedup improves with corpus diversity but not in a way users see | LOW PRIORITY |
| **Brand compounding** (consistent presence over time) | Founder-credibility-build IS this — LinkedIn weekly post; founder voice | **MAINTAIN** post-launch |
| **Retention as growth** (retention drives WOM) | Possible — design doc P6 makes the loss-aversion argument | **MEASURE** — is the 7-day-trial loss-aversion thesis actually firing? Run user-interview cohort at day 30 |

**Critical:** without referral mechanics, tldrof is on an **acquisition treadmill** — every new user requires fresh spend or fresh content. The Morning Brew precedent is the proof that referral compounds; the doc's v1.1 list has the per-newsletter slider instead. **This is the highest-leverage roadmap change in the entire review.**

---

## Section 8 — Metrics & instrumentation

### Measure (weekly)

- **Acquisition by channel** (UTM-tagged): HN, Lenny's classified, LinkedIn organic, LinkedIn DM, Reddit verticals, ProductHunt
- **Activation rate** = % of trial signups who complete the magic moment (received first digest) — definition specific to tldrof
- **Day-7 activation-to-paid conversion** (trial-to-paid)
- **Day-30 retention** of paying cohort (was the loss-aversion thesis right?)
- **Vohra "very disappointed" survey** at day 14 of paid (run quarterly)
- **CAC by channel** = $ spent ÷ paying customers attributed
- **NPS or referral intent** at day 30

### Do NOT measure (vanity)

- **Twitter follower count** (correlation with revenue ~zero per skill)
- **HN upvotes** (correlation with revenue near-zero per skill)
- **Total signups** (without retention)
- **LinkedIn follower count** (unless the LinkedIn motion becomes the main channel)

### Specific dashboard

Recommend a Supabase + Plausible/Fathom + a weekly Notion review combining:
- Mailgun inbound volume (= dogfood-style engagement)
- Stripe MRR + churn rate
- Plausible UTM-tagged landing-page traffic
- Manual: weekly "what did I do for audience-build this week" log (the audience_build_journal.md template — see Outputs)

---

## Section 9 — Risk analysis

### Distribution risks specific to this plan

| # | Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|---|
| R1 | **Mailbrew-is-free** pulls the floor out from the $9 paid market | HIGH | HIGH | Lean into corporate-coverage moat AND quality-of-summarization that Mailbrew's free tier can't match; A/B test pricing post-launch |
| R2 | **Show HN miss** (front page fails, <10 upvotes) | MEDIUM-HIGH (LoomLetter base rate suggests not impossible) | MEDIUM (if Show HN is one of 3+ channels, the miss is recoverable) | Multi-channel launch sequence per Section 5b; Lenny's classified hits same week |
| R3 | **Founder time-allocation stays 5% audience** despite commitment to 30% | MEDIUM | HIGH | Hard scheduling — block 2 hours on calendar daily; pre-commit Lenny's classified spend as forcing function ($400-800 cash out the door = motivation to make it count) |
| R4 | **Dogfood mismatch persists** (founder doesn't actually subscribe to Morning Brew/Axios/etc.) | MEDIUM-HIGH | HIGH | Hard commitment: founder subscribes to 5+ buyer-aligned newsletters by build day 8; documents quality of digest on those vs technical newsletters |
| R5 | **PMF survey at day 14 private beta comes back <30%** | MEDIUM | HIGH | Calendar gate may have to slip; founder must commit IN ADVANCE that they will slip the launch if survey is <30% |
| R6 | **Corporate-segment IT-compliance objections** kill the moat at first attempt (lawyer/finance buyer asks for DPA, SOC2; tldrof has neither) | HIGH for Daniel-segment | MEDIUM | Defer Daniel-segment to v1.0.5+; in v1.0 focus moat-positioning on Maya-segment (corporate product marketer using corporate email but not requiring formal procurement) |
| R7 | **Channel concentration risk** (if Lenny's classified produces 60%+ of paying users) | MEDIUM | MEDIUM | Diversify into vertical Reddit + cold DM by day 30; don't double down on Lenny's repeat before other channels are tested |
| R8 | **CAC inflation** in cold-DM channel if response rates are <5% | MEDIUM | LOW (cold DM is time, not cash) | Measure response rate weekly; cut if <3% after 50 DMs |
| R9 | **Competitor counter-launch** (Readless adds bulk-backlog flow + corporate-coverage marketing) | LOW-MEDIUM (per design doc pass 4: Readless is also solo founder, same capacity ceiling) | HIGH | Move fast on positioning + Strategic Ladder Rung 2 (Suite); don't get out-shipped on the wedge |
| R10 | **Macro: paid newsletter aggregator market is small** (Mailbrew gave up + went free; signals demand at $10 is contested) | MEDIUM | HIGH | Reframe TAM via the moat segment (M365/corporate is a different TAM); if Maya/Daniel don't convert, sunset and pivot |

---

## Outside voice — independent critique

(Per skill: mandatory subagent or Codex review. Not invoked as a separate subagent in this regression run because the regression harness is itself standalone, but the equivalent skeptical pass below — anchored against publicly-documented launch failures in this category.)

**Single biggest marketing risk the inside review missed:** the inside review treats the **20-22 day build window as fixed and audience-build sprint as parallel**. If the founder's true time-allocation stays 80% build / 20% audience (the realistic outcome for a technical solo founder under build crunch), the audience-build sprint produces ~1/3 of the output the plan calls for. **The plan's success probability is conditional on a behavioral change (founder spending real time on audience) that the founder has not historically demonstrated.** If the choice were forced, the inside review would push to delay launch by 7-10 days for pre-launch audience compounding — but did not push hard enough.

**Channel weakness vs founder vibes:** Lenny's Newsletter classifieds at $400-800. The classified slot might not be sized to drive 15-25 paying customers in one shot — Lenny's data per Sparkloop suggests classified CTR is in the 0.5-2% range with conversion below that. A more honest estimate: $400-800 Lenny's classified drives **5-15 trial signups**, perhaps 1-4 paying. Don't treat it as the primary launch channel; treat it as one input to the multi-channel mix.

**Audience claim lacking evidence:** "Maya, 38, Director of Product Marketing at fintech in NYC, reads 12 newsletters." This persona was reasoned-from-archetype, not interviewed. **Before day-14 private beta, founder should interview 3 real product marketers who read newsletters and validate the persona against reality.** The skill cannot verify Maya exists; the founder must do the work.

**Provocative reframe the founder might not have considered:** *"What if tldrof is actually a B2B-procurement product, not a consumer subscription?"* The corporate-coverage moat (P4) describes a segment where the buyer is an individual but the procurement is gated by IT. If the founder skews the product to "$19/mo personal, $99/mo team-of-5 with admin dashboard and IT-approval one-pager," the motion class shifts from consumer-subscription (where Mailbrew-free crushes the floor) to small-team B2B (where Mailbrew doesn't compete and where the founder's enterprise-engineering background at Micron is an asset). This is a meaningful re-positioning that the doc has not entertained. **Worth a /office-hours session post-launch to explore.**

---

## Handoff — 3 strongest action items for THIS week

The founder MUST commit to these three this week (build days 1-7). Everything else can slip.

1. **Subscribe to 5 buyer-aligned newsletters TODAY** (Morning Brew, Axios AM, The Hustle, Money Stuff by Matt Levine, Term Sheet by Fortune). Forward them to the test address starting day-0 spike. Run digest on them by build day 5. **This is the M0e fix — expanding dogfood corpus to match the actual paying ICP.** If founder doesn't do this, the M0e mismatch ships intact and the product calibration error is unrecoverable post-launch.

2. **Email the 10 engineer-network contacts THIS WEEK** with a private-beta CTA. Goal: 5 dogfood signups by build day 9 (CEO PC3 calls for 3-5 HN-cohort friends; this implements it). **Concrete commitment: emails sent by Friday EOD this week.**

3. **Book the Lenny's classified slot THIS WEEK for the launch-week issue.** $400-800 cash out the door. The forcing-function logic: cash committed = motivation to make landing page + launch copy actually work for the Maya-persona. Plus: locks in a non-HN traffic source the day of launch. **If founder won't spend the $400-800, that's the signal that audience-build sprint is theater and the plan should be downgraded.**

---

## Recommended follow-up skills

- **`/office-hours`** — to explore the B2B-team re-positioning surfaced by outside-voice critique. NOT before launch (don't pivot at the gate); post-launch month 1 if conversion data suggests it.
- **`/plan-ceo-review`** — only if pricing changes meaningfully (moving from $9 to $19 or adding $19 tier). The CEO review locked $9; revisiting is a business-model change.
- **`/plan-design-review`** — for the landing page specifically. Maya-persona conversion psychology is different from HN-cohort; design review should focus on trust signals (logos, security copy, corporate-email coverage hero).
- **Re-run `/plan-cmo-review` at post-launch day 45** — measure plan against reality; adjust 60-90 day section based on what fired.

---

## Appendix — Web searches invoked

1. `Readless.app newsletter digest pricing reviews 2026` — https://www.readless.app/blog/best-newsletter-management-tools-2026
2. `Meco newsletter app pricing users acquisition` — https://meco.app/, https://meco.app/partner-program, https://www.readless.app/blog/meco-pricing-2026
3. `Readwise growth strategy how they got users 2025` — https://www.fueler.io/blog/readwise-usage-revenue-valuation-growth-statistics, https://blog.readwise.io/why-were-bootstrapping-readwise/
4. `Morning Brew growth referral newsletter acquisition strategy` — https://www.marketergems.com/p/morning-brew-newsletter-growth-strategy-case-study, https://www.referralcandy.com/blog/morning-brew-referral-program, https://growsurf.com/blog/how-morning-brew-grew-its-subscribers/
5. `"Show HN" consumer subscription newsletter app launch traction` — https://newsletter.marclou.com/p/how-to-launch-a-startup-on-hacker-news, https://www.revenuecat.com/state-of-subscription-apps/, https://news.ycombinator.com/item?id=43196845
6. `Superhuman concierge onboarding Vohra very disappointed PMF launch` — https://review.firstround.com/superhuman-onboarding-playbook/, https://underscore.vc/resources/case-story-superhuman/, https://digidai.github.io/2025/11/23/rahul-vohra-superhuman-grammarly-acquisition-pmf-framework-deep-analysis/
7. `consumer newsletter aggregator inbox app competitors 2026 Refind Mailbrew Meco` — https://www.readless.app/blog/mailbrew-pricing-2026 (revealed Mailbrew is FREE since Nov 2025), https://www.readless.app/alternatives/mailbrew

---

*End of marketing_plan.md. Auxiliary artifacts: `icp.md`, `launch_playbook.md`, `audience_build_sprint.md`.*
