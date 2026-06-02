# ICP Specification — tldrof.com v1.0

Companion artifact to `marketing_plan.md`. Skill: plan-cmo-review v0.2.

## v1.0 PRIMARY persona — Maya (AI Product Manager)

### Identity attributes (≥5 specific per skill M1 criteria)

- **Age:** 30-35.
- **Geography:** SF Bay, NYC, Seattle, Austin, or remote-by-policy at major tech hub company.
- **Role:** Senior PM at Series B/C AI-adjacent startup (e.g., Anthropic-adjacent, OpenAI-ecosystem, dev-tools-with-AI-features, AI-for-vertical companies).
- **Income:** $180-280K total comp; not budget-constrained at $9-15/mo SaaS.
- **Family:** ~50% have kids; time-poverty is structural.
- **Tools paid:** ChatGPT Plus ($20/mo), Lenny's premium ($5/mo), Notion ($10-15/mo), often Linear ($8-14/seat), often Loom, often Pitch or Figma. Frequently has paid for Superhuman at some point. Frequently pays for Apollo or Clay for sourcing if they touch BD.
- **Newsletter spend stack:** 8-15 paid + free newsletter subscriptions. AlphaSignal, TLDR AI, TLDR Tech, Bensbites, Lenny's Newsletter, Pragmatic Engineer (free + premium), Stratechery (paid $12/mo), Latent Space, The Information (sometimes), Axios Pro (firm-billed for some).

### Where Maya currently spends attention (≥5 specific per skill M1 criteria)

1. **X / Twitter.** Follows: Lenny Rachitsky (@lennysan), Jason Liu (@jxnlco), Eugene Yan (@eugeneyan), Swyx (@swyx), Aman Sanger (@amanrsanger), Karri Saarinen (@karrisaarinen), Andrej Karpathy, Yohei Nakajima. Spends 30-60 min/day scrolling, mostly mornings + bedtime.
2. **Lenny's Slack community.** Active member; lurks more than posts; reads daily-digest in #showandtell, #ai, #pm.
3. **Latent Space podcast.** Listens commuting / walking dog. Reads accompanying Substack.
4. **AlphaSignal daily email.** Opens 4-5 days/week; saves links to read later but rarely does.
5. **Hacker News.** Reads occasionally (weekend); comments rarely; never posts.
6. **LinkedIn.** Posts ~1/month; reads industry-news posts; doesn't engage deeply.
7. **Slack / Discord in 1-2 work communities** (Mind the Product, Reforge alumni, AI Engineer Slack).
8. **Substacks read regularly:** Stratechery, The Pragmatic Engineer (paid), Lenny's Newsletter, Latent Space, occasionally Eugene Yan's blog, occasionally Sequoia's Ascent.

### What Maya pays for in adjacent categories

- **Productivity SaaS:** Notion $10-15/mo, sometimes Linear $8-14/seat (firm-billed), Loom $12-15/mo.
- **AI tools:** ChatGPT Plus $20/mo, sometimes Claude Pro $20/mo, sometimes Perplexity Pro $20/mo.
- **Information:** Lenny's premium $5/mo, Stratechery $12/mo (sometimes), The Information $39/mo (rare).
- **Email tools:** Has paid for Superhuman ($30/mo) at some point; usually churned because $30 felt high.

### What Maya complains about in adjacent categories

- "I subscribed to AlphaSignal AND TLDR AI AND Bensbites and they cover the SAME stories."
- "I save links to Notion / Pocket / Readwise but I never come back to them."
- "I open the AlphaSignal email at 7am, scan headlines, mark as read, and feel like I learned nothing."
- "My Saturday morning is just inbox triage. I haven't read for fun in months."
- "Why am I paying $5/mo for Lenny's premium if I never read the long-form essays?"
- "I want a single email per day with everything I need to know. The Skimm tried but it's too breezy."

These complaints map *directly* to tldrof's bankruptcy + dedup + 60-second magic moment value props.

### Specific objection patterns Maya would raise

1. **"Another AI summarizer? Why not Readless / Meco / Mailbrew?"**
   - Response: 60-second magic moment + backlog-bankruptcy triage (unique vs Readless); cross-source dedup with attribution (vs Meco); active product vs deprecated (vs Mailbrew); forwarding architecture works for accounts where repointing is impossible (specific structural moat).
2. **"Do I trust forwarding all my newsletters to a 3rd party I just found?"**
   - Response: forwarding architecture — *we never touch your inbox*; you control which newsletters reach us (you forward them); transparency on data handling; founder-signed digest; SPF/DKIM/DMARC done right.
3. **"I'll forget to set it up after the trial."**
   - Response: auto-forward helper makes Gmail set-and-forget in 2 minutes. (Caveat: Outlook/Apple Mail / Proton helper is v1.0.5.)
4. **"I tried Mailbrew, didn't stick. Why is this different?"**
   - Response: Mailbrew expected ongoing curation work; tldrof is *bankruptcy-first* — your backlog is the magic moment, not a configuration project.
5. **"$9/mo is another subscription. I'm SaaS-fatigued."**
   - Response: $9 is the cost of 1 lunch + 2 lattes per month. The 45 min/day of inbox triage you reclaim is worth >$1/min of your time.
6. **"My company's AI tools / Notion AI already summarize things."**
   - Response: They summarize what you open. tldrof dedupes what you'd otherwise *miss* by deleting unread.

### Specific reasons Maya would convert

- The 60-second bankruptcy moment is *screenshot-worthy* — visceral proof of value within the first interaction.
- "Saved 3h 12min today" footer is share-worthy on X, where Maya already spends attention.
- Cross-source dedup attribution ("also covered in: AlphaSignal, TLDR AI") proves it's doing real work.
- Maya already pays $20/mo for ChatGPT Plus; $9 for a workflow-specific AI tool is well within her band.
- Auto-forward helper closes the retention loop without ongoing effort — set-and-forget product.
- Founder narrative (if invested in per Audience-Build Sprint) gives Maya someone she trusts behind the product.
- Substack ("Drowning in TLDRs") creates Maya-shaped readers BEFORE they're product users — high-intent leads.

### Conversion-likelihood signal

- Maya pays for $20 ChatGPT Plus + $5 Lenny's. **$9/mo is well within band; she will not price-shop at the bottom.** Per skill anti-pattern #7, matching Readless $4.90 would *signal commodity to Maya*. Hold $9 minimum.
- Maya is time-poor. Per M0d, no-CC trial may be the WRONG mechanic for her — she doesn't trial-shop; she trust-shops. Trial-with-CC or waitlist-to-pay are higher-signal mechanics.

---

## v1.0.5 SECONDARY persona — Karen (Big Law Associate) — DEFERRED

Karen persona is hypothesis-not-validated. Founder has NOT dogfooded the M365 / Outlook / corporate-locked-email segment. Per M0e, premature to publish landing copy targeting Karen until at least 1 paying-corporate user validates the segment.

### Karen sketch (for v1.0.5 planning context only)

- 35-45 yo Big Law associate or finance professional (Goldman, Citadel, AQR).
- M365 / Outlook locked by corporate IT (OAuth into work inbox forbidden).
- Subscribes to: Lexology, Above the Law, NY Law Journal, Bloomberg Law, FT Lex, Axios Pro Rata, Politico, Punchbowl, Semafor, Pitchbook News.
- Pays: firm-billed Bloomberg $50+, Politico Pro $$$, Lexology Pro $$.
- Active on: LinkedIn (very), legal-Slack communities, almost never HN/Reddit.
- Time-poor at extreme: billable hours target = 2000+/yr.
- $9/mo (or $15-20) is rounding error.

### Why deferred

1. **Dogfood mismatch** (M0e): founder has not tested with Karen's newsletter mix (paywalled Bloomberg/FT, Lexology, Politico Pro).
2. **Channel-of-fit mismatch**: Karen is on LinkedIn + legal-Slack + bar-association forums; founder has zero presence in any of these.
3. **v1.0 product gap**: Gmail-only auto-forward helper does NOT serve Outlook/M365 (per CEO PC2, Outlook is v1.0.5).
4. **Trust gap**: Karen's segment buys on referral + firm-endorsement, NOT cold landing pages.

### v1.0.5 plan to validate Karen

- Identify 3-5 Karen-shaped people in founder 2nd-degree network (founder lives in California, may have corporate-locked friends from prior life).
- Concierge onboard those 3-5 in v1.0.5 private beta.
- Measure: Vohra "very disappointed" %, filter setup rate (Outlook helper required), retention.
- If ≥2 of 5 convert and report retention dependence, publish corporate-coverage landing copy + open the channel.

Until then: the "M365 coverage" line is STRUCTURALLY TRUE but MARKETING-CONTAINED. The forwarding architecture works for those users (P4 truth), but the product is not yet tuned for them (M0e truth).

---

## Personas the product is NOT for (v1.0 explicit exclusion)

Per M0c anti-feature analysis, naming who the product is NOT for helps tighten v1.0 positioning.

- **Casual newsletter readers** (1-3 subscriptions, no overload pain). The bankruptcy framing requires actual bankruptcy.
- **Free-tier tinkerers** (will trial 5 SaaS products this month, convert to none). Per M0d, no-CC trial may attract these; CC-required or waitlist filters them out.
- **Power-user AI engineers who want programmatic API access** (MCP wrapper is v1.1, not v1.0).
- **Multi-tenant team buyers** (per-seat pricing is v2+).
- **Crypto / day-trader / news-trader audiences** (different urgency profile; need real-time, not daily-digest).
- **Non-English-speaking users** (LLM summarization is English-tuned at v1.0).
