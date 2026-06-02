# ICP Specification — TLDR-of-TLDRs (tldrof.com)

**Status:** v1 working draft (post plan-cmo-review v0.3 — premise-audit corrections applied)
**Run:** tldrof-2026-06-01-v0.3-blindC
**Date:** 2026-06-01

---

## Primary v1.0 ICP — "Priya"

(Composite. Real shape, fictional name.)

### Demographics

- 30-45 years old
- Knowledge worker in a 200-2000 person company
- Roles: Product Manager (Director-level), Marketing Lead, Finance/Strategy, Consulting Partner, Ops Lead, technical Founder-equivalent (CTO of small ops-heavy company)
- US/Canada/UK/AU primary; English-language newsletters
- Gmail account for personal (v1.0 target) OR Microsoft 365 / Outlook (v1.0.5 target once auto-forward-helper supports M365)
- Compensation: $150K-300K, can expense some productivity tools personally OR via company professional-development budget

### Newsletter behavior

- Subscribed to **≥3 newsletters**, at least 1 from an **industry/vertical publication**
- Typical mix:
  - 1-2 from work-adjacent: Lenny's Newsletter, Stratechery, Pragmatic Engineer, First Round Review, Reforge content drops
  - 1-2 general business/intelligence: Morning Brew, The Hustle, Axios AM, Axios Pro Rata
  - 1-2 vertical or premium: The Information, Substacks she pays for, premium industry publication
  - 0-2 dev TLDRs (only if she's PM/engineering-leadership-adjacent; many Priyas have ZERO dev TLDRs)
- Inbox state: chronic 1,000-5,000 unread; "newsletter shame" pile; declared "inbox bankruptcy" mentally at some point
- Currently reads: Lenny's full, skims everything else on her phone during commute, archives unread by Friday

### Attention surface (where she spends time RIGHT NOW)

(At least 5 specific places — required per M1 criteria)

1. **Lenny's Newsletter** (Substack) — reads every issue, sometimes premium
2. **Lenny's podcast** (Spotify/Apple) — listens during commute/workout
3. **LinkedIn for industry content** — scrolls evenings, follows ~30-60 thought leaders in her function
4. **Acquired / Stratechery podcast** — listens during commute
5. **One paid Substack** (Sahil Bloom, Packy McCormick, Ben Thompson, or vertical equivalent) — pays $5-15/mo
6. **Reforge community** (if PM/marketing) — paid annual membership
7. **Pragmatic Engineer / Engineering Enablement** (if engineering-leadership-adjacent) — reads weekly
8. **WhatsApp groups with peers from MBA / prior employer / industry meetups** — peer-share patterns
9. **Twitter/X** — occasional, mostly during big events; not a daily habit

NOT on her attention surface:
- Hacker News (unless she's in the dev-newsletter subsegment, which is a smaller part of the ICP)
- Reddit r/SideProject / r/Entrepreneur (occasional at best)
- TikTok/Instagram for productivity content
- Discord servers (rare for this persona unless dev-leaning)

### Current spend on adjacent productivity / attention products

- ChatGPT Plus: $20/mo
- Notion Personal: $10-15/mo
- One paid Substack: $5-15/mo
- Possibly: Lenny's Premium ($20/mo), Stratechery ($15/mo), The Information ($33/mo), Readwise ($10-13/mo), Superhuman ($30/mo if she's in the early-adopter cohort)

**Median monthly attention/productivity spend: $50-100/mo across 3-5 subscriptions.**

**$14/mo for tldrof.com is INSIDE her range. $9/mo is below median (signals commodity).**

### What she complains about in adjacent categories

- "I subscribe to too many newsletters; I keep meaning to clean up"
- "Reader apps (Pocket, Refind) collect things I never read"
- "I tried Meco / Substack Reader; never built the habit"
- "I want to read Lenny's and Stratechery in full, skim the rest, but I never have time"
- "My inbox is overwhelming and I declared bankruptcy in Q1"
- "I can't add browser extensions to my work email" (corporate-segment specific)
- "I unsubscribed but then I miss things I actually wanted to read"

### Specific objections she would raise

- "Privacy — you're reading my email?" → answer: forwarding architecture, we never touch your inbox, only what YOU forward
- "I tried Meco / Refind / Readless; didn't stick" → answer: bulk-backlog magic moment in 60s, not the slow daily-builds those other tools have
- "$9/mo for a newsletter aggregator?" → if priced $9: answer with magic-moment differentiation; if priced $14: answer with premium-positioning + concierge offer
- "I'll just unsubscribe" → answer: you've TRIED that; bankruptcy framing acknowledges previous failed solution
- "I don't want yet another subscription" → answer: $14 replaces 30+ min/day of inbox-shame; cumulative ROI in time-saved math
- "Can I integrate with [Notion / Readwise / Reader / etc.]?" → v1: no; v1.1+: yes via MCP/API (but DON'T over-promise in launch copy)

### Specific reasons she would convert

- The magic-moment demo (60s) is visceral; she feels relief
- Inbox-bankruptcy framing names her exact lived experience
- A peer / Lenny / colleague mentioned it (trust transfer)
- She's already paying $50-100/mo for adjacent tools; $14 fits the budget
- Concierge-intake offer (founder personally walks her through setup) = high-trust mechanic
- Annual pricing discount + retention math = "I'll lock this in for the year"

---

## Adjacent ICP — defer to v1.0.5

### Corporate-locked-out segment

Same persona shape but on M365 / Outlook with corporate IT policies. Requires v1.0.5 auto-forward-helper expansion to M365 / Outlook / Apple Mail / Proton.

Vertical examples:
- Lawyer at AmLaw 200 firm
- Finance professional at IB / PE / hedge fund
- Healthcare admin at hospital system
- Government employee
- Agency operator with custom-domain email
- Compliance officer in regulated industry

**UNVALIDATED** assumption: this segment can forward externally despite corporate IT. Required: 5 user interviews before v1.0.5 commits to this expansion (see outside-voice critique #3).

---

## Explicit exclusions for v1.0 (DO NOT target with launch copy)

- **Pure HN-cohort dev-newsletter readers** — that's Readless's segment, $4.90 floor, comparison-shoppers, time-rich
- **"Indie hackers" as a category** — too broad, includes too many people who won't pay $14/mo for a newsletter tool
- **Power users wanting MCP/API/programmatic** — defer to v1.1 audience; would dilute the v1 positioning
- **Pure free-tier seekers** — by design, no freemium; trial only
- **Enterprise buyers** — outside skill scope and outside product capability at v1

---

## Conversion path (corresponds to M2 forcing-question discovery)

**Path A (organic, slow):** Lenny mentions tldrof.com in a Friday roundup → Priya clicks → 60s magic moment renders → signs up → trial converts → annual upgrade

**Path B (social, medium):** Colleague on Slack says "I've been using this, saved me 30 min/day" → Priya asks for link → signs up

**Path C (concierge, first cohort):** Founder emails Priya directly (warm intro) with 15-min onboarding offer → Priya accepts → onboarded live → pays immediately

**Path D (sponsorship, scaled cohort):** Lenny's Newsletter or Morning Brew sponsorship placement → Priya clicks (1-3 days post-issue) → signs up

For v1.0 launch: Paths C + B carry first 10-20 paying. Path A + D carry next 30-100.

---

## Segmentation summary

| Segment | v1.0 priority | Channel mix | Pricing |
|---|---|---|---|
| Priya (Gmail, knowledge worker, ≥3 newsletters incl. vertical) | **PRIMARY** | Concierge + Lenny's sponsorship + LinkedIn organic | $14/mo or $108/yr (annual-first) |
| Dev-newsletter HN/IH cohort | SECONDARY | Show HN, IndieHackers cross-post | Same pricing; might churn faster |
| M365 corporate-locked-out | DEFER to v1.0.5 | Vertical communities + cold outreach | $19/mo with concierge intake |
| Power users / MCP-API seekers | DEFER to v1.1 | Pragmatic Engineer / dev-tool channels | TBD |
| Teams / B2B | INVESTIGATE first (outside-voice critique #4) | Different motion entirely | $99/mo team if validated |

---

END icp.md
