# Regression test fixture — B2B SaaS (synthetic) / plan-cmo-review

**Skill under test:** `plan-cmo-review`
**Fixture type:** synthetic (no real founder; constructed product scenario)
**Purpose:** exercise the skill against a B2B SaaS motion (high-touch sales, longer cycle, multi-stakeholder buyer) — different from the tldrof consumer-subscription motion. Ensures the skill doesn't apply consumer-product patterns to B2B contexts.

## Synthetic input scenario

A fictional founder is building **"Threadline"** — a Linear-style project tracking tool specifically for engineering teams at 50-500 person companies. Their design doc says:

- **Pricing:** $40/seat/month, no free tier, 14-day trial
- **Target users:** engineering managers, tech leads, IC engineers at mid-size SaaS companies
- **Distribution Plan:** "Show HN at launch + content marketing on the engineering management blog"
- **First 10 customers:** "Founders' friends + HN cohort"
- **Validation gate:** 5 paying companies by day 30
- **Product differentiation:** "Better than Linear for engineering-specific workflows"
- **Founder background:** 2 ex-Google engineers, no prior B2B sales experience
- **Existing audience:** 200 followers on X, ~50-person personal email list, no professional content history

The skill is run against this design doc with no additional context.

## Why this fixture exists

The tldrof fixture tests the skill against consumer-subscription product patterns. B2B has fundamentally different dynamics:

- **Buyer ≠ user** (the EM or VPE buys; ICs use)
- **Procurement gates** (security review, IT involvement, vendor approval)
- **Pricing per-seat dynamics** (not consumer ARPU)
- **Sales cycles measured in weeks-months**, not minutes-hours
- **Reference customers / case studies** matter more than product virality
- **Bottom-up vs top-down adoption** is its own strategic question
- **HN is right audience for dev tools and engineering managers** — different category-error analysis than tldrof

A skill that surfaces consumer-product insights for a B2B product is misfiring. This fixture catches that failure mode.

## Expected insights (7 items)

Pass condition: ≥5 of 7 surfaced.

### Insight 1: HN is partially right audience for this product (correctly distinguish from tldrof)

**What we expect:** The skill recognizes HN reaches engineering managers and tech leads (the actual buyer for this product) and does NOT apply the "HN is wrong audience class" pattern blindly. HN works for dev tools / engineering-management products in a way it doesn't work for consumer-habit products.

**Why this matters:** Catches the failure mode where the skill over-generalizes the tldrof insight. HN is wrong audience for some products and right audience for others. Category-error analysis must be product-specific.

**Acceptable variations:**
- Explicit "HN works better here than for consumer products because audience overlap is higher"
- Implicit treatment: keeps HN as a primary channel (high leverage score), doesn't flag as category error
- At minimum: doesn't apply the tldrof HN-is-wrong-audience pattern as a universal rule

### Insight 2: Buyer ≠ user dynamics surfaced

**What we expect:** The skill surfaces that the person paying ($40/seat/mo budget approval) is typically the EM, VPE, or finance person — NOT the IC engineer who uses the product daily. Implication: marketing motion needs to address BOTH audiences with different messages; bottom-up adoption (ICs love it → manager has to buy) is its own strategy distinct from top-down (EM evaluates → IC must use).

**Why this matters:** B2B-specific dynamic that consumer-product skills miss entirely. The marketing plan must address both audiences.

**Acceptable variations:**
- Direct buyer-vs-user analysis with named personas for each
- Bottom-up vs top-down adoption strategy choice surfaced
- At minimum: ICP includes multiple stakeholder roles, not single buyer

### Insight 3: Sales cycle and procurement gates surfaced

**What we expect:** The skill flags that B2B procurement adds gates the consumer playbook ignores: security review (SOC 2 / SSO requirements), vendor approval processes, IT involvement, possibly legal review for $40/seat × team-size deals. Time-to-revenue extends from hours/days (consumer) to weeks/months (B2B).

**Why this matters:** The design doc's "5 paying companies by day 30" gate may be unrealistic given typical procurement timelines. Skill should surface this.

**Acceptable variations:**
- Explicit security/SOC 2/SSO requirement flagged
- Procurement timeline estimates
- At minimum: flags that the day-30 gate is aggressive for B2B procurement cycles

### Insight 4: Reference customer / case study marketing motion

**What we expect:** The skill surfaces that B2B marketing depends heavily on social proof — case studies, named customers, testimonials from people the buyer recognizes. Implication: first-customer strategy isn't just about revenue; it's about getting REFERENCEABLE customers whose logos can be used in future marketing.

**Why this matters:** Consumer plans optimize for user count; B2B plans optimize for reference quality. Different North Star metric for early customers.

**Acceptable variations:**
- Explicit "land referenceable customers first" framing
- Case study production planned as part of customer success motion
- At minimum: first-10 strategy includes "must be willing to share logo / give testimonial" criterion

### Insight 5: Community / content channels match this audience class

**What we expect:** The skill identifies the right channel mix for engineering managers and tech leads at mid-size SaaS companies: specific publications (Lenny's Newsletter, Pragmatic Engineer, ChiefOfStaff.com), specific Slack communities (Lenny's, Rands Leadership), specific conferences (LeadDev, QCon), specific podcasts (Software Engineering Daily, Engineering Manager Podcast). These overlap heavily with the ICP and convert well.

**Why this matters:** B2B has specific publication / community channels that consumer products don't use. Skill should know them.

**Acceptable variations:**
- Names ≥3 specific publications or communities serving engineering management
- Identifies podcast guesting as high-leverage for this ICP
- At minimum: channel mix is B2B-shaped (specific communities and publications), not consumer-shaped (HN + Twitter + Substack only)

### Insight 6: Pricing analysis — per-seat dynamics

**What we expect:** The skill examines the pricing model itself, not just the price point. Surfaces questions like: $40/seat × 50-seat team = $24K/yr ACV (real B2B revenue per customer); $40/seat × 5-seat startup = $200/mo (much weaker). Implication: customer-size targeting matters more than per-seat price. Different from consumer plans where price point dominates.

**Why this matters:** Per-seat pricing changes the entire economics. Targeting larger companies with same per-seat price = different business than targeting startups.

**Acceptable variations:**
- ACV analysis surfaces customer-size targeting question
- Pricing model alternatives surfaced (per-seat vs per-org vs feature-tier)
- At minimum: flags that customer-size strategy is a load-bearing pricing decision

### Insight 7: Bottom-up vs top-down adoption is a strategic choice

**What we expect:** The skill surfaces that B2B products typically pick a primary adoption path: bottom-up (free / cheap individual use → spreads to team → org buy) like Slack/Notion/Linear, OR top-down (sell to VPE/CTO → mandate cascades down) like enterprise tools. Each requires different marketing motion. Threadline's design doc doesn't specify; skill should force the choice.

**Why this matters:** Consumer products don't have this strategic split. B2B does. Skill must surface it.

**Acceptable variations:**
- Direct bottom-up vs top-down analysis with recommendation
- Identifies which incumbents in the space won via which path
- At minimum: surfaces it as a strategic question the founder must answer

## Pass criteria

- **PASS:** ≥5 of 7 surfaced
- **STRONG PASS:** 7/7 with strong B2B-specific depth
- **FAIL:** ≤4 of 7 — investigate which skill change degraded B2B coverage

## Failure modes this fixture catches

- Skill applies tldrof's consumer-subscription patterns (HN as category error, freebie-disqualifier, ICP as individual buyer) to B2B uncritically
- Skill produces generic channel scoring without B2B-specific channels (specific publications, communities, conferences)
- Skill misses procurement / sales-cycle realities
- Skill ignores buyer-vs-user distinction

## Notes for adding more B2B variants

This fixture covers mid-market B2B SaaS. Consider adding variants for:

- **Enterprise** (>1000 seats, RFP-driven sales, security questionnaire heavy)
- **SMB / self-serve B2B** (≤10 seats, credit card, no sales touch)
- **Vertical SaaS** (industry-specific — different community / publication landscape)

Each motion has different expected-insights rubric. Don't try to make one fixture cover all B2B; specialize.
