# ICP Specification — tldrof.com

**Companion to:** `marketing_plan.md`

The design doc declared one omnibus persona ("Engineers, PMs, founders, AI-adjacent professionals + M365/corporate-locked-out users"). That's 2-4 distinct ICPs bundled. This doc splits them, picks one for v1.0, and defers the rest with explicit deferral rationale.

---

## v1.0 PRIMARY ICP — "Jake the saturated technical reader"

### Identity
- **Name:** Jake (composite)
- **Age/career:** 28-40, engineer / PM / founder / AI-adjacent professional at a US SaaS, AI lab, or startup
- **Location:** US-based (Stripe geography for v1.0)
- **Income:** $120-300K base; comfortable but not lavish; values time

### Subscription stack (the inbox)
- 5-15 newsletters: AlphaSignal, TLDR Tech, TLDR Newsletter, Bensbites, Lenny's Newsletter, Pragmatic Engineer, Stratechery, Latent Space, The Neuron, Morning Brew, The Hustle, plus 2-4 vertical newsletters in their specific tech sub-area
- Often signed up during a phase of "intentional learning" (~6-18 months ago) and now drowning
- Aggregate inbox volume from these: ~20-40 newsletter emails/week

### Where Jake currently spends attention (≥5 named places)
1. **Hacker News** — daily; 10-30 min/morning
2. **Twitter/X** — follows Pieter Levels (`@levelsio`), Lenny Rachitsky, Sahil Bloom, Marc Lou, Tony Dinh, Daniel Vassallo, several Anthropic/OpenAI engineers
3. **Substack apps** — for Lenny's, Stratechery, Pragmatic Engineer (some of which they paid for)
4. **Indie Hackers** — lurker, occasional comment
5. **YouTube (technical channels)** — Fireship, Theo, Primeagen, AI Explained, Lenny on YT
6. **r/SideProject + r/MachineLearning** — lurker
7. **Discord/Slack** — 2-4 founder/engineering communities (varies)

### What Jake currently pays for (adjacent categories)
- ChatGPT Plus ($20/mo) or Claude Pro ($20/mo) — often both
- Cursor or Copilot ($20-40/mo)
- Linear ($8-16/seat/mo if at a small team)
- Notion ($10/seat/mo or personal)
- 1-2 paid Substack subscriptions ($5-10/mo each)
- Possibly Superhuman ($30/mo) if executive-shaped
- Possibly Readwise / Readwise Reader ($10/mo) if avid reader
- **Total monthly SaaS subscription stack: $80-200/mo.** Jake feels saas-fatigued, defends every new $9.

### What Jake complains about in adjacent categories
- "ChatGPT rate-limits me when I bulk-paste 20 newsletters at once."
- "Mailbrew shut down. I tried to migrate to Readwise Reader but it's a different product."
- "Refind keeps recommending the same articles I've already seen."
- "My inbox is unmanageable — I declare email bankruptcy every quarter."
- "I keep meaning to read [Lenny / Stratechery / Pragmatic Engineer] but it piles up."
- "Substack Reader is okay but doesn't dedup across publications."
- "I tried Readless and it was OK — first digest took 24 hours and I'd already moved on."

### Specific objection patterns Jake will raise to tldrof
1. **"How is this different from Readless? They're $4.90."** — bankruptcy framing + 60s vs 24h + auto-forward helper + structural moat
2. **"I can do this with ChatGPT for free."** — true for 1-2 newsletters; not true for daily bulk-forward of 10+ across multiple verticals; the time-saved math + auto-recurrence is the wedge
3. **"Mailbrew got acquired. What if you do too?"** — fair concern; honest answer is data is exportable; the founder is committed; the recurring revenue model means we don't NEED to get acquired to survive
4. **"$9/mo is steep. I'm already paying $X for everything."** — true; the math should pencil at "we save you N min/week worth more than $9 of your time"
5. **"I don't want to set up forwarding rules. Too much friction."** — auto-forward setup helper (Gmail v1.0) gets it down to 1-click for the common case
6. **"What if you stop maintaining it? I'd have to migrate my subscriptions back."** — fair; honest answer + the unsubscribe extraction in v1.1 helps undo

### Specific reasons Jake will convert
1. **60-second magic moment lands on first visit.** The "you saved N minutes" footnote is shareable; Jake screenshots it and posts to Twitter.
2. **Auto-forward setup helper for Gmail is genuinely one click.** Friction-zero entry to the recurring-digest pattern.
3. **The bankruptcy framing matches Jake's actual pain.** "50 unread newsletters" is not hypothetical for Jake; he has 73 right now.
4. **Cross-newsletter dedup is a real differentiator.** Jake reads AlphaSignal + Bensbites + Latent Space + Neuron — every major AI release gets covered in all four; the dedup actually shows merge.
5. **Time-saved math is HONEST (per CEO E3 / D7 / Q3).** Doesn't claim "85% reduction"; computes from actual word counts; Jake's engineer brain trusts honest numbers.
6. **Solo-founder narrative.** Jake is in the indie-hacker / build-in-public orbit; he wants to support solo founders.

### Channels to reach Jake (per Section 3 marketing_plan)
- Show HN (lottery odds, but baseline expected reach)
- Twitter/X build-in-public (compounding, primary channel)
- Indie Hackers + r/SideProject (community fit, day +2 of launch sequence)
- Newsletter-creator placements (deferred to v1.0.5; targets the publications Jake already reads)
- Substack content compounding (long-term)

### Conversion economics for Jake (rough)
- Average LTV at $9/mo, 5% monthly churn = ~$180
- Average LTV at $86/yr annual (20% off), 20% annual churn = ~$430
- Conversion rate from HN-driven signup → paid: estimate 5-15% (HN traffic is high-curiosity, low-intent)
- Conversion rate from concierge-onboarded private-beta → paid: estimate 30-60% (high-trust, high-intent)
- **Implication: the 20-50 manually-onboarded private-beta users will likely produce more revenue than the next 500 HN-driven signups.** This is why Mode C and the Vohra pattern matter.

---

## v1.0.5+ DEFERRED ICP — "Maya the corporate professional"

### Identity
- **Name:** Maya (composite)
- **Age/career:** 40-55, managing partner at a regional law firm OR director-level at a financial-services firm OR senior healthcare exec
- **Location:** US; major metro
- **Income:** $250-700K; high; values time-saved more than money-saved by a wide margin

### Subscription stack (the inbox)
- 3-8 vertical industry newsletters
  - Law: Law360, ABA Journal, Above the Law, Bloomberg Law alerts
  - Finance: Axios Pro Rata, Term Sheet, The Information, Bloomberg Wealth, WSJ Morning
  - Healthcare: STAT News, Endpoints, Fierce Healthcare, Becker's
- Possibly 1-2 cross-vertical reads (Morning Brew, The Daily, NYT)
- Inbox volume: ~10-20 newsletter emails/week; LOW cross-source overlap compared to AI/dev verticals

### Where Maya currently spends attention (≥5 named places)
1. **LinkedIn** — heavy professional use; daily; 30 min/day
2. **Bloomberg Terminal / Bloomberg Law portal** (work tool, daily; multi-hour)
3. **Industry-specific Slack or community** (Bar Association Slack, finance-pro Discord, etc.)
4. **Trade publications** in vertical (printed or digital)
5. **Vertical-industry conferences** (annual; networking)
6. **WSJ / NYT homepage** (twice/day; brief)
7. **Assistant-forwarded emails** (Maya has an EA; many subscriptions flow through the EA's processing)

**Almost zero overlap with HN, Twitter, Indie Hackers, r/SideProject.**

### What Maya currently pays for
- Bloomberg Terminal: $24K/yr (or comparable terminal)
- Professional memberships: $1-5K/yr
- Conferences: $5-15K/yr
- Industry trade publications: $300-2K/yr each
- LinkedIn Premium: $300/yr
- M365 corporate (paid by firm; she can't choose alternatives)
- Apple-ecosystem personal subscriptions: ~$50-100/mo
- **Total professional+personal subscription stack: $30-60K/yr.** $9/mo is below the noise floor.

### What Maya complains about
- "I have 50 unread Law360 alerts from this week."
- "My EA forwards everything but I still miss things."
- "I want to use [Notion AI / Shortwave / similar AI inbox tool] but IT won't allow OAuth."
- "I don't have time to learn new tools."

### Specific objection patterns
1. **"Is this enterprise-secure? My IT department blocks anything that touches my work email."** — forwarding architecture answers this perfectly; "we never touch your inbox" is the trust story
2. **"$9/mo? I don't even know how to expense $9/mo."** — actually a real friction at this segment. Annual billing helps. So does invoicing.
3. **"I don't have time to learn another tool."** — concierge onboarding (founder personally onboards for first 20-50) addresses this directly
4. **"Can you do enterprise SSO / SOC 2 / SAML / etc.?"** — fair concern; v1.0 says no, v1.0.5 might say "in development"
5. **"Can my assistant set this up for me?"** — yes; concierge-onboarding pattern handles this; EA-friendly workflow is a v1.0.5 feature

### Specific reasons Maya might convert
1. **Forwarding architecture works on corporate M365.** No competitor in her awareness can do this.
2. **Trust-led referral from a peer.** If one managing partner at her bar association swears by it, conversion rate is ~50%+.
3. **Concierge onboarding.** Solves the "no time to learn" objection.
4. **Premium pricing signals seriousness.** $19-29/mo at the corporate path is read as "this is serious software" by Maya; $4.90 is read as "this is hobbyist."
5. **Time-saved math.** Maya's hourly value is genuinely $200-500/hr; 1 hour/week saved is $1000-2000/month value, vs $19-29/mo cost. Compelling.

### Channels to reach Maya
- Vertical-industry newsletter placements (paid; $1-5K per placement)
- LinkedIn long-form by founder (some reach if Maya's network overlaps)
- Industry-specific Slack / community presence
- Peer referrals (trust-led; hardest to manufacture but highest-converting)
- Vertical-industry trade publications (sponsored mention; expensive)
- Conferences (founder presence; expensive but high-trust)

**NOT reachable via:** HN, Twitter, Indie Hackers, r/SideProject, Product Hunt, generic SEO.

### Why Maya is DEFERRED to v1.0.5 (per M0d Option B)
1. **Acquisition channels do not overlap with v1.0 launch channels.** Building a corporate-acquisition motion is a separate program, not a v1.0 launch lane.
2. **Pricing motion is different ($19-29 vs $9).** Premature to split pricing in v1.0.
3. **Onboarding motion is different (concierge vs self-serve trial).** Premature to run both motions.
4. **Customer-development cycle for corporate is 2-6 months** (vs 1-7 days for HN-cohort). Eats the entire v1.0 measurement window.
5. **v1.0 capacity (solo founder, 20-22 day build, 1 customer-acquisition channel max) cannot serve both segments.**

**v1.0.5 motion proposal for Maya (sketched, do NOT execute in v1.0):**
- Separate landing page at `tldrof.com/corporate` (or `/professional`) with $19-29/mo pricing
- Concierge-waitlist sign-up flow
- Founder personally onboards first 20 corporate users via 30-min video call
- Outreach via LinkedIn (founder posts long-form targeting vertical professionals; reaches via LI algorithm to Maya's adjacent network)
- One paid vertical-newsletter placement test ($2-5K) in first 60 days post-launch
- Annual billing offered with invoice/PO support (Stripe Invoicing handles this with ~1 day of integration)
- Strict KPI: 10 paying corporate users within 90 days of v1.0.5 motion start, at $19-29/mo, with ≥80% retention at 60 days. If hit, scale; if not, kill the segment and refocus on Jake.

---

## Marketing copy implications (apply to v1.0 launch)

Given Jake-only positioning for v1.0:

### Above-the-fold landing-page copy (per CEO PC1 priority order, refined for Jake-only)
1. **Headline:** "50 unread newsletters? Forward them all here. Get one digest in 60 seconds. Inbox debt cleared."
2. **Sub-headline:** "Built for the AI-engineer / founder who's drowning in TLDR, Bensbites, Pragmatic Engineer, Lenny's, and 12 others."
3. **CTA:** "Start your 7-day free trial" → forward-from-inbox magic moment

### REMOVED from launch copy (per M0c + M0d findings)
- ~~"Works with Gmail, Outlook, Proton, anything. We never touch your inbox."~~ — corporate moat language; defer to v1.0.5
- ~~"400M+ M365 users locked out of OAuth tools"~~ — corporate moat; defer
- ~~Strategic Ladder mentions (Suite/Concierge/Platform)~~ — fundraising narrative; do NOT show users
- ~~MCP wrapper / API mentions~~ — power-user signal; dilutes "set and forget"
- ~~Per-newsletter slider~~ — power-user; v1.1 communication only after conversion

### Pitch deck for personal-network outreach (50-person list)
- Slide 1: Bankruptcy framing + 60s magic moment screenshot
- Slide 2: One sentence on architecture (forwarding-address, not OAuth)
- Slide 3: Honest pricing ($9/mo, $86/yr) + honest time-saved math
- Slide 4: Honest comp position ("Readless exists at $4.90; here's what's different")
- Slide 5: Ask — "would you try it for free for the next 60 days in exchange for honest feedback?"

---

## Validation checkpoints

- **End of build window (day -22 from launch):** ≥10 private-beta said-yes from cold-email outreach; ≥3 of them are using the product weekly
- **Day -7:** ≥10 private-beta active; PMF signal measured (Vohra question + filter_setup_rate)
- **Day +14 post-launch:** P6 hit (15 paying)
- **Day +30 post-launch:** P5 hit (25 paying)
- **Day +60 post-launch:** decide v1.0.5 motion (corporate path OR Jake-only depth)
