# ICP Specification — TLDR-of-TLDRs

Two distinct ICPs, treated separately (their conflation in the design doc is the largest unforced error per Step 0.5 M0e + M0d findings).

---

## Persona A — "Devin" (HN-cohort segment, dogfood-aligned, lower-leverage)

**Demographics:**
- 32, senior engineer at mid-size tech co, $160-200K base
- US-based; remote or hybrid; reads on phone + laptop interchangeably
- Time profile: time-pressured but does experiment with tools

**Attention surface (where they currently spend time):**
1. Hacker News — daily ~7-8am, scans front page, ~5-10 comments/week
2. X / Twitter — follows ~150-300 (mostly engineering / AI / startup voices); reads in 5-min bursts throughout day
3. Lenny's Newsletter, Pragmatic Engineer, Latent Space — paid subscriber
4. AlphaSignal, TLDR, Bensbites — free subscribers (the daily digests they're drowning in)
5. Slack groups: PM-focused, eng-focused, AI-focused (3+)
6. Podcasts: Latent Space, Lenny's Podcast, occasional Acquired
7. /r/programming, /r/MachineLearning (passive lurker)

**Current adjacent-category spend:**
- ChatGPT Plus $20/mo
- Claude Pro $20/mo (yes, both)
- Readwise $10/mo
- Notion $10/mo
- Sometimes: Linear / Cursor / Raycast Pro

**What they complain about in adjacent tools:**
- Newsletter overload (THE pain)
- "Too much noise, not enough signal" in AI-tool content
- Tool sprawl; want consolidation
- "I have 12,000 unread emails and I just keep ignoring them"

**Specific objections to tldrof:**
- "Why pay $9 when Readless is $4.90?" — answer: bankruptcy flow + power-user features (justify; Section 6 recommends $12 to widen the gap)
- "Can it really replace my reading? I might miss something important." — answer: digest is opt-in; original always available
- "Forwarding-address pattern is unfamiliar / extra step" — answer: 60-second magic moment lands inside that anxiety
- "Yet another subscription" — answer: time-saved math + annual billing

**Reasons they would convert:**
- Bankruptcy magic-moment shows tangible value in 60s of zero-friction trial
- Daily-ritual after week 1 creates loss-aversion lock
- Time-saved math compounds visibly week over week
- $9 (or $12) fits their accepted band

**Reachable via:**
Show HN, IndieHackers, /r/SideProject, X (build-in-public), Lenny's-adjacent podcast guesting, dev / AI Twitter, Substack technical content, personal network.

**Acquisition mechanic fit:** Free trial works. Stripe Checkout works.

---

## Persona B — "Maria" (corporate-locked-out segment, differentiated, higher-leverage)

**Demographics:**
- 41, finance director at Fortune 500 (substitute: GC at law firm, hospital CIO, agency operator — same shape)
- $250-450K total comp; senior IC or first-level manager
- M365 corporate email; IT explicitly forbids OAuth into work inbox (or strongly discourages)
- Time profile: severely time-poor, schedule-driven, money-easy
- Buys tools via approved vendor list OR personal credit card OR peer recommendation

**Attention surface:**
1. Axios Pro (sector-specific edition) — paid subscriber
2. Sector publications: American Banker / Treasury & Risk / CFO Dive (for finance); Above the Law (legal); Healthcare Dive / Becker's (healthcare); etc.
3. WSJ + FT (passive, daily skim)
4. LinkedIn — industry voices, not founder voices; reads 10-15 min/day; comments rarely
5. Industry Slack groups (1-2; may be small private)
6. Trade-association events — 2-3 per year; primary in-person network
7. Bloomberg Briefs (4 sector-specific) — paid
8. SMS / text threads with industry peers
9. Internal corporate digest (mandatory; adds to overload)

**Current adjacent-category spend:**
- Bloomberg Briefs ~$400/yr (~$33/mo)
- Industry analyst services $1K-2K/yr
- WSJ $150/yr
- Personal productivity tools: usually minimal — work tools are employer-funded
- May personally pay for: Calendly, occasional ChatGPT Plus

**What they complain about in adjacent tools:**
- "I can't OAuth my work email; tools that need it don't work for me"
- "Newsletters arrive faster than I can read; I miss things weekly"
- "I forward important things to my personal email so I can read on phone — that's already a thing I do"
- "I'd pay for someone to filter / summarize but I don't trust SaaS with my work email"

**Specific objections to tldrof:**
- "Can I actually use this with my corporate email? IT will flag any tool needing inbox access." — answer: YES, forwarding-architecture is OAuth-free, that's the structural advantage
- "Is the summary good enough to trust? I can't miss something important." — answer: dedup + cross-source attribution + originals always available
- "$9/mo feels cheap-and-suspect; is this a real product?" — answer: this is real (annual billing + concierge onboarding fix the signal); $19 tier might actually convert this segment BETTER than $9
- "Is it secure? I forward sensitive briefings sometimes." — answer: data not used for training, 30-day raw email retention, never resold (need explicit security page)

**Reasons they would convert:**
- Forwarding-architecture is the ONLY workable shape for their use case (paid newsletters tied to work-email identity; corporate-account constraints)
- Concierge onboarding signals premium / trust
- Time-saved is more valuable to them than to Persona A (their hour is worth more in absolute terms)
- Peer recommendation from another senior-role person closes the deal

**Reachable via:**
Vertical industry publications (paid placement / sponsored mentions), LinkedIn industry-voice content + warm-intro DM, peer referral in industry Slack groups, trade-pub coverage, industry events.

**Acquisition mechanic fit:** Free trial is wrong mechanic; concierge waitlist + 1:1 demo + paid is right. Annual billing default.

---

## Why two ICPs matter (synthesis)

These are different audiences with different acquisition channels, different price-tolerance, different trust mechanics, different copy, and different validation paths. The design doc names both ("HN-cohort + M365 corporate-locked-out users") but plans as if they're one launch. **They are not.**

Plan implication: split-cohort launch (HN-cohort calendar-gated; corporate-cohort PMF-gated) is the correct shape. See `marketing_plan.md` Section 5 + `launch_playbook.md`.
