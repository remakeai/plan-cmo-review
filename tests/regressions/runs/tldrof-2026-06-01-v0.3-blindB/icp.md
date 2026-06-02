# ICP Specification — tldrof.com

**Reviewer:** plan-cmo-review v0.3.0 (blind regression run B)
**Date:** 2026-06-01

This doc is the corrected ICP — the moat segment (Maya/Daniel) promoted to PRIMARY from the doc's "secondary post-launch" framing, and Sam (the dogfood-aligned engineer) demoted to tertiary. Per skill M0e: BOTH pivots required (target audience + dogfood subjects).

---

## PRIMARY persona — Maya (corporate product marketer, M365/Outlook)

| Attribute | Detail |
|---|---|
| Name (composite) | Maya Chen |
| Age | 38 |
| Role | Director of Product Marketing |
| Company | 600-person Series C fintech, NYC |
| Email environment | Microsoft 365 / Outlook (corporate-domain); IT compliance prohibits OAuth into work mail by Gmail-based AI tools |
| Income / role context | $200-280K total comp; trust-shop pattern; values "won't get me in trouble with IT/security" highly |
| Newsletter subscriptions (~12 active) | Morning Brew, Axios AM, Stratechery, The Hustle, Lenny's Newsletter (paid Pro $228/yr), Term Sheet (Fortune), Money Stuff (Matt Levine), Marketing Brew, Tomasz Tunguz, First Round Review, Pragmatic Engineer (occasional), Reforge updates |
| Reading pattern | Skims at 8:15am train commute (~10 min); 9pm pre-sleep skim (~15 min); rarely reads on weekends; pile builds Monday-Wednesday |
| Current workarounds | Outlook folder rules to bucket newsletters into "morning reads"; manual triage at desk Friday afternoon (~30 min/wk); occasionally pastes a specific newsletter into ChatGPT for summary |
| Adjacent paid tools | ChatGPT Plus ($20/mo), Notion personal ($15/mo), Lenny's Pro ($19/mo annual), Loom Business ($14/seat) |
| Voiced complaint | "I missed the one thing in TLDR that mattered yesterday because I skipped it for the day, and then I find out my CEO saw it from somewhere else and asked me about it in standup." |
| Where she spends attention online | LinkedIn (active follower of ~8 product-marketing thought leaders including Lenny, April Dunford, Emily Kramer); Lenny's Newsletter Slack community (paid member); First Round Review and Reforge content; Stratechery podcast on commute; Substack reader for Money Stuff; occasionally on r/ProductManagement |
| **NOT where she spends attention** | Hacker News, r/SideProject, ProductHunt (knows it exists, rarely visits), IndieHackers, X/Twitter (anti-X since 2023) |
| Objections to tldrof | "Does this work with corporate Outlook?" (yes — moat); "Where does my data go?" (need a clear DPA/security one-pager); "Will my IT block this?" (need IT-friendly positioning); "Is it worth $9 when I can ignore newsletters for free?" (frame against status quo of missed signal cost) |
| Reasons to convert | (1) corporate Outlook works without IT involvement (the moat); (2) the loss-aversion at trial-end if she's reallocated the 30 min/wk; (3) a peer mentioned it on Lenny's Slack or LinkedIn |

---

## SECONDARY persona — Daniel (boutique-firm lawyer, custom-domain Exchange)

| Attribute | Detail |
|---|---|
| Name (composite) | Daniel Reyes |
| Age | 44 |
| Role | Partner |
| Firm | 30-attorney boutique commercial litigation firm, Chicago |
| Email environment | Custom-domain via Microsoft Exchange Online; firm IT runs tight ship; OAuth-to-third-party blocked at policy level |
| Income / role context | $400K+; very trust-shop; legal exposure concerns for any tool that touches work mail; reputation-conscious |
| Newsletter subscriptions (~8 active) | Law360 Daily, ABA Journal Daily News, Bloomberg Law Daily, Above the Law, Litigation Daily, The Briefcase, plus 2 personal (LitHub Daily, Marginal Revolution) |
| Reading pattern | First 2 newsletters (Law360, ABA) considered mandatory; reads 6-8am at home with coffee. Remainder pile up; reads occasionally on weekends |
| Current workarounds | Outlook folder rules; assistant occasionally flags items; otherwise: misses things |
| Adjacent paid tools | LexisNexis (firm pays), Westlaw (firm pays), personal: Bloomberg subscription ($35/mo), WSJ ($15/mo), NYT ($15/mo) |
| Voiced complaint | "I find out about a Bloomberg Law update from a court opposing counsel and feel a step behind." |
| Where he spends attention online | LinkedIn (legal-trade professional posts), Above the Law (reads almost daily), Bloomberg Law content, occasional Above the Law sponsor content, attends 1-2 ABA conferences a year |
| **NOT where he spends attention** | Hacker News, ProductHunt, IndieHackers, X (deleted account), Reddit (occasionally r/Lawyertalk) |
| Objections to tldrof | "DPA? SOC2? Where is data stored?" (formal procurement-level concerns); "Has another firm in my circle used it?" (needs peer reference); "Can I get this through firm procurement or is it personal?" (split decision) |
| Reasons to convert | Peer-firm reference; vertical-legal-newsletter sponsorship signal that the product is "made for lawyers like me"; a 30-day money-back guarantee (NOT a trial) |

---

## TERTIARY persona — Sam (engineer, dogfood-aligned, the Show HN cohort)

| Attribute | Detail |
|---|---|
| Name (composite) | Sam Park |
| Age | 31 |
| Role | Senior Engineer |
| Company | YC-backed SaaS, ~25 person, SF |
| Email environment | Gmail personal + corporate Workspace (Gmail) |
| Income / role context | $220K total comp; price-sensitive on personal SaaS tools; tinkers with new products often |
| Newsletter subscriptions (~10) | TLDR Newsletter, TLDR Tech, AlphaSignal, Bensbites, Pragmatic Engineer (free), Latent Space, TheNeuron, Lenny's Newsletter, Stratechery, Marginal Revolution |
| Reading pattern | Reads TLDR daily (mandatory); skims AlphaSignal; ignores rest most weekdays |
| Current workarounds | Gmail filters; sometimes uses Notion AI to summarize a single newsletter; tried Refind, didn't stick |
| Adjacent paid tools | ChatGPT Plus ($20/mo), Cursor ($20/mo), GitHub Pro (free with student), Notion ($10/mo) |
| Voiced complaint | "I have like 200 unread newsletters in my pile from the last month, I just hit 'mark all read' last week and felt slightly guilty." |
| Where he spends attention online | Hacker News, X tech-Twitter, GitHub trending, IndieHackers (occasional), r/SideProject, ProductHunt (daily), Latent Space Discord |
| Objections to tldrof | "Why not free Mailbrew?"; "Is Claude better than other LLMs for this?"; "Can I self-host?"; "Is there an API?" |
| Reasons to convert | (1) Show HN momentum / X-Twitter buzz; (2) bankruptcy framing resonates ("clear my 200-email backlog in one digest"); (3) technical-quality signal ("Claude-mediated dedup" reads as actually better than naive approach); (4) the founder is in his cohort and the product is clearly built by an engineer |
| Reasons NOT to convert (acknowledged risk) | Mailbrew is free; price-sensitive at $9; doesn't trust-shop, so doesn't pay a premium for trust; high probability of trial-and-churn (the M0d freebie-disqualifier in action) |

---

## ICP-by-channel mapping

| Channel | Maya | Daniel | Sam |
|---|---|---|---|
| Show HN | NO | NO | YES |
| Lenny's classified | YES (PRIMARY) | NO | YES (overlapping cohort) |
| LinkedIn organic | YES (PRIMARY) | YES (PRIMARY) | NO |
| Vertical legal newsletter sponsorship | NO | YES (PRIMARY) | NO |
| Cold LinkedIn DM | YES (PRIMARY) | YES (PRIMARY, harder to reach) | NO |
| r/ProductManagement | YES (occasional) | NO | NO |
| r/sysadmin, r/legaltech | Indirectly (the IT/ops people who would approve) | YES (vertical) | NO |
| ProductHunt | NO | NO | YES |
| IndieHackers | NO | NO | YES |
| X tech-Twitter | NO | NO | YES |
| Podcast (Lenny's, IH, Pragmatic Eng) | YES | NO | YES |

---

## Dogfood-corpus pivot (the M0e fix)

**Founder's existing dogfood (technical/tech-AI corpus):**
- TLDR, AlphaSignal, Bensbites, Pragmatic Engineer, Stratechery, Latent Space, TheNeuron, Lenny's Newsletter

**ADD by build day 8 (mandatory M0e fix):**
- Morning Brew (general business — Maya AND Daniel)
- Axios AM (general news — Maya)
- The Hustle (business+tech — Maya)
- Money Stuff by Matt Levine (Substack — finance, Daniel-adjacent)
- Term Sheet by Fortune (VC/finance — Maya)
- Marketing Brew (Maya specifically)
- One vertical legal sample if feasible (Above the Law free email — Daniel)
- One vertical healthcare/finance sample (STAT Free or The Daily Upside)

**Why this matters:** the dedup signature, the summarization tone, the "what counts as the same story" heuristics — all are currently tuned to AI/tech news. A Money Stuff item and a TechCrunch item ABOUT the same news event will have wildly different framings; the dedup pass must handle that. Tuning the system on technical-newsletter-only corpus ships the product calibrated to the wrong audience.

---

## Persona validation work item (pre-launch)

**The skill cannot verify Maya or Daniel exist.** The founder MUST run 3 interviews with real people in the persona by build day 10:

- 1 product marketer at a corporate using Outlook (Maya)
- 1 person in a legal/finance/healthcare role using corporate Exchange (Daniel)
- 1 engineer-cohort person to validate the Sam baseline (Sam — easier; founder knows people)

Capture: their actual newsletter list, what they pay for, what they currently use as workaround, what objection would block them from trying tldrof. Update this ICP doc after the interviews.
