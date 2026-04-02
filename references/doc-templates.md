# Document Templates — ProductManager Skill (v2)

All templates below embed the 95% PM standard. Audit fixes are marked with ⚠️ where they address a previously identified gap.

---

## 01. Problem Brief

```markdown
# Problem Brief: [Product Name]

**Date:** [Date]
**Author:** [Name]
**Status:** Draft / Validated / Approved
**Validation Status:** [X of Y interviews completed | Survey: N responses | Data signal: present/absent]

---

## Problem Statement (One Sentence)
> [Users] struggle to [do X] because [root cause], which causes [painful outcome].

---

## Kill-Switch Assumption ⚠️
> **If [this one thing] is not true, the product is unviable.**
> Confidence: [High / Medium / Low]
> How to validate: [Specific method]
> Deadline: [Date — this must be answered before building]

This is the most important open question. Everything else is secondary.

---

## Problem Decomposition

### Who Exactly Is the User?
- **Segment:** [Be specific — not "professionals," but "solo freelance designers aged 25–35 in tier-2 cities"]
- **Context:** [When/where does this problem occur?]
- **Behavior today:** [Named workarounds — specific, not vague]
- **Frequency:** [How often does this problem occur per week/month?]
- **Pain level:** [X/10 — justified with evidence, not asserted]
  - Evidence: [Quote, observation, or data that justifies this rating]

### Current Solutions & Their Gaps
| Solution | What it does | Why it's insufficient | Switching trigger |
|---|---|---|---|
| [Solution 1] | [Description] | [Gap] | [What would make users leave it] |
| [Solution 2] | [Description] | [Gap] | [What would make users leave it] |

### Why Now?
- [Trend 1 — with evidence or labeled [Assumed]]
- [Trend 2 — with evidence or labeled [Assumed]]
- [What's changed that creates this specific window?]
- **Competitive window:** [How long before a well-funded player closes this? Evidence or [Assumed]]

### Problem Validation Evidence ⚠️
Label every item as [Validated], [Planned], or [Assumed]:
- [ ] [Validated / Planned] Interviewed [N] users — key quotes:
  - "[Direct quote that captures the pain]" — [User type, city]
- [ ] [Validated / Planned] Observed behavior: [Specific thing observed]
- [ ] [Validated / Planned] Data signal: [Specific metric or data point]

---

## What Success Looks Like
> If we solve this completely, [specific user] will [specific behavior change], and we'll know because [measurable signal].

---

## What We Are NOT Solving
- [Out of scope item] — Reason: [Why excluded]
- [Out of scope item] — Reason: [Why excluded]

---

## Open Questions (Ranked by Kill Risk)

| Question | Kill Risk | Owner | Deadline |
|---|---|---|---|
| [Kill-switch assumption question] | Critical | [Person] | [Date — before building] |
| [Second most important question] | High | [Person] | [Date] |
| [Other open question] | Medium | [Person] | [Date] |
```

---

## 02. User Research Brief

```markdown
# User Research Brief: [Product Name]

**Date:** [Date]
**Research Goal:** [One sentence — what decision will this research inform?]
**Recruitment Plan:** [Who recruits users, how, with what incentive] ⚠️

---

## User Segments to Study

### Primary Segment — [Name]
- **Who:** [Specific description — age, income, behavior, frequency]
- **Why primary:** [Why they matter most — revenue, frequency, or signal quality]
- **Sample size target:** [N interviews + N survey responses]
- **How to recruit:** [Specific channel + incentive] ⚠️

### Secondary Segment — [Name]
- **Who:** [Specific description]
- **Relationship to product:** [How they interact — demand, supply, influencer]
- **How to recruit:** [Specific channel + incentive]

### Supply-Side Segment (if marketplace) — [Name] ⚠️
- **Who:** [Specific description of supply providers]
- **Why critical:** Supply-side is the existential risk in any marketplace. Without supply, demand can't activate.
- **Key concern to probe:** Will they see the platform as a tool that gives them more, or a threat to their direct relationships?
- **Sample size target:** [N interviews]

> ⚠️ RULE: Every segment identified here MUST appear in GTM targeting, UX requirements, and metrics tracking. No segment disappears after the research brief.

---

## Research Questions (Ranked by Priority)

| Priority | Question | Why It Matters | Segment |
|---|---|---|---|
| P0 | [Kill-switch question] | [Validates or kills the core assumption] | [Segment] |
| P0 | [Supply adoption question] | [Will supply providers join and stay?] | Supply |
| P1 | [Switching trigger question] | [What gets users to change behavior] | Demand |
| P2 | [Growth/referral question] | [How the product spreads] | Both |

---

## Interview Guide (30 min)

**Warm-up (5 min)**
1. Tell me about your [role/context] — how do you [relevant activity]?
2. Walk me through the last time you [did the thing we're solving].

**Core Questions (15 min)**
3. What went wrong? [Probe for specifics]
4. What did you try when that didn't work?
5. How did you figure out [key variable — price, timing, availability]?
6. Have you ever been in a situation where [acute version of the pain]? What happened?
7. What would "perfect" look like?

**Switching & Adoption Questions (5 min)**
8. If [our solution] existed, what would stop you from using it?
9. If it disappeared tomorrow, what would change?
10. [For supply side:] If more customers came through an app, would that be better or worse than your current setup? Why?

**Wrap-up (5 min)**
11. What did I not ask that I should have?
12. Would you test an early version?

---

## Key Hypotheses to Validate

| Hypothesis | Evidence Type | Pass Criteria | Fail Criteria |
|---|---|---|---|
| [Core demand hypothesis] | Interview + first ride | [Specific: >40% do X] | [Specific: <20% do X] |
| [Supply adoption hypothesis] | Onboarding + retention | [Specific: >60% do Y] | [Specific: <30% do Y] |
| [Pricing hypothesis] | Interview + willingness to pay test | [Specific threshold] | [Specific threshold] |
| [Growth/referral hypothesis] | Referral tracking | [Specific: >25% via referral] | [Specific: <10% via referral] |

---

## Research Deliverables
- [ ] Synthesis doc with top 5 insights per segment
- [ ] User personas (max 2 — demand + supply)
- [ ] JTBD statements for both segments
- [ ] Journey map: current state (before product) for both demand and supply
- [ ] Kill-switch assumption: [Validated / Invalidated / Still open]
```

---

## 03. Product Strategy Document

```markdown
# Product Strategy: [Product Name]

**Date:** [Date]
**Version:** [1.0]

---

## North Star
> [One sentence: what does this product ultimately do for users?]

---

## Kill-Switch Assumption ⚠️
> Same as Problem Brief. Repeated here because every strategy decision must be stress-tested against it.

---

## Strategic Context

### Market Opportunity (With Math) ⚠️
- **TAM:** [Total market — with source or [Assumed]]
- **SAM:** [Serviceable market — with logic]
- **SOM (Year 1):** [N users] × [frequency/month] × [avg transaction] × [take rate] = [Revenue]
  - Example: 50,000 riders × 4 rides/month × ₹150 avg fare × 18% commission = ₹54,00,000/year (~$65K)
  - Is this enough to sustain operations? State explicitly.
- **Why this market now:** [Specific evidence for each claim — not assertions]
- **Competitive window:** [How long and WHY — cite specific signal or label [Assumed]] ⚠️

### Competition Landscape

| Competitor | Strengths | Weaknesses | Threat Level | Our Differentiation |
|---|---|---|---|---|
| [Most dangerous competitor] | [Strengths] | [Weaknesses] | Critical/High/Med | [Specific — not "better UX"] |
| [Second competitor] | | | | |

### Most Dangerous Indirect Competitor — Deep Dive ⚠️
> The most dangerous competitor is often indirect. They don't compete on the same solution — they represent zero switching cost for the user.

**[Competitor Name]:**
- What they do: [Description]
- Why they're more dangerous than the obvious competitor: [Reason]
- Their structural weakness: [Specific gap you can exploit]
- Risk: [What happens if they directly enter your space]

---

## Value Proposition

**For** [specific user]
**Who** [has this specific problem at this specific frequency]
**Our product** [does this]
**Unlike** [most dangerous competitor — not just the most obvious one]
**We** [specific differentiator that they can't copy in <6 months]

---

## Strategic Bets (Ranked)

| Bet | Thesis | Risk If Wrong | Reversibility | Evidence |
|---|---|---|---|---|
| [Bet 1] | [Why we believe this] | [Consequence] | High/Med/Low | [Validated/Planned/Assumed] |

### Commission Rate Bet — Special Note ⚠️
> Commission rates are asymmetrically hard to change: lowering is easy (users love it), raising is nearly impossible (drivers revolt, word spreads fast in small communities). State the commission rate explicitly, show the unit economics math at that rate, and confirm it reaches sustainable margin.
>
> **At [X]% commission:** [Math showing path to sustainability]
> **If we need to raise to [Y]%:** [Honest assessment of feasibility]

---

## What We Believe Must Be True

| Assumption | Confidence | Validation Method | Status | Deadline |
|---|---|---|---|---|
| [Kill-switch assumption] | [H/M/L] | [Specific test] | [Validated/Planned] | [Date — before building] |
| [Second most critical] | [H/M/L] | [Test] | [Status] | [Date] |

---

## Strategic Moat

| Moat Type | Present? | How It Builds Over Time | How Fast Competitors Can Copy |
|---|---|---|---|
| Network effects | [Y/N] | [Mechanism] | [Timeframe] |
| Data advantage | [Y/N] | [Mechanism] | [Timeframe] |
| Community trust | [Y/N] | [Mechanism] | [Timeframe] |
| Distribution | [Y/N] | [Mechanism] | [Timeframe] |
| Technology | [Y/N — be honest] | [Mechanism] | [Timeframe] |

---

## What We Are Explicitly NOT Doing

| Decision | What We're Giving Up | Why | Trigger to Reconsider |
|---|---|---|---|
| [Decision 1] | [Cost of not doing it] | [Rationale] | [Signal that would change this] |
```

---

## 04. PRD — Product Requirements Document

```markdown
# PRD: [Feature/Product Name]

**Date:** [Date]
**PM:** [Name]
**Status:** Draft → Review → Approved
**Target Launch:** [Date or Sprint]
**Team Size:** [N developers] — Timeline is calibrated to this. ⚠️

---

## TL;DR (2 sentences)
> [What we're building and why, in plain language.]

---

## Problem We're Solving
[Reference Problem Brief — 2-sentence summary]
**Kill-switch assumption:** [Repeat it here]
**User impact if unsolved:** [Specific pain — not vague]

---

## Goals & Non-Goals

### Goals
- [Specific, measurable outcome #1 — with target number]
- [Specific, measurable outcome #2 — with target number]

### Non-Goals
- [What this explicitly won't do — with reason]
- [Scope boundary — with reason]

---

## User Stories

| As a... | I want to... | So that... | Priority | Acceptance Criteria |
|---|---|---|---|---|
| [User] | [Action] | [Outcome] | P0 | [Specific: "Given X, when Y, then Z"] ⚠️ |
| [User] | [Action] | [Outcome] | P1 | [Acceptance criteria] |

---

## Functional Requirements

### P0 — Must Have (Launch Blockers)
For each requirement, include:
- Description: [What it does]
- Acceptance Criteria: [Specific, testable condition] ⚠️
- Performance Target: [Specific number — not "fast"] ⚠️

**Example format:**
- [ ] **Real-time driver tracking**
  - Description: Rider sees driver location on map as driver moves
  - Acceptance Criteria: Driver location updates every [X] seconds; visible on map within [Y] seconds of ride acceptance
  - Performance Target: Location refresh ≤ [X]s; map load ≤ 2s on 4G connection

> ⚠️ CONSISTENCY RULE: All performance numbers must match across PRD, technical constraints, and success metrics. Before finalizing, cross-check: match time, load time, refresh rate, completion rate — every number that appears more than once must be identical.

### P1 — Should Have
- [ ] [Requirement + acceptance criteria]

### P2 — Nice to Have
- [ ] [Requirement]

---

## UX Requirements
- **Primary language:** [Language-first approach]
- **Onboarding:** [Maximum N screens — specify]
- **Core flow:** [Max N taps from open to value — specify]
- **All user segments from Research Brief must be addressed:** ⚠️
  - [Segment 1] UX consideration: [What makes it work for them]
  - [Segment 2] UX consideration: [What makes it work for them — including segments like elderly]
- **Edge cases:**
  - [No supply available]: [Specific handling]
  - [Payment failure]: [Specific handling with fallback]
  - [GPS inaccurate]: [Specific fallback]
- **Error states:** [Language and tone requirements]
- **Empty states:** [What users see on first open]

---

## Technical Constraints
- **Platform:** [Why this platform, what's excluded and when it will be added]
- **Third-party dependencies:** [List with free tier limits — flag when you'll hit them]
- **Performance:** [Every number here must match success metrics section]
  - App launch: < [X]s
  - Map load: < [X]s
  - Driver match: < [X] minutes (not seconds — be consistent) ⚠️
  - Location refresh: every [X] seconds
- **Offline behavior:** [Specific]
- **Security:** [Specific requirements]

---

## Success Metrics

| Metric | Baseline | Target | Measurement | Consistency Check |
|---|---|---|---|---|
| [Primary metric] | [Value] | [Target] | [Method] | [Matches PRD section: Y/N] ⚠️ |

> ⚠️ Before finalizing: every number in this table must match the corresponding number in the technical constraints and functional requirements sections.

---

## Timeline Reality Check ⚠️
> **[N] developers, [X] weeks, building [list what's being built]**
> Is this realistic? Flag aggressive timelines explicitly rather than pretending they're achievable.
> Risk if timeline slips: [Specific consequence]
> What gets cut if we're 2 weeks behind: [Pre-decided scope cuts]

---

## Launch Criteria
- [ ] [Specific condition — testable]
- [ ] [Minimum supply threshold met before any demand activation]

---

## Open Questions & Decisions Needed

| Question | Kill Risk | Owner | Deadline |
|---|---|---|---|
| [Most critical — kill-switch level] | Critical | [Person] | [Date] |
```

---

## 05. MVP Scope Definition

```markdown
# MVP Scope: [Product Name]

**Date:** [Date]
**Time Constraint:** [N weeks]
**Team Constraint:** [N developers / founder]
**Budget Constraint:** [$X]

---

## MVP Hypothesis
> If we build [X] for [specific user], they will [specific behavior], which proves [specific assumption].
> This hypothesis is **falsifiable** — we will kill the product if [specific No-Go signal].

---

## What Makes This an MVP
- **Not a prototype** — works in production, real users, real money
- **Not a v1.0** — minimum needed to learn, not to be proud of
- **Definition of Done (specific):** [N users have done Y action without assistance, within Z days] ⚠️

---

## MVP Feature Set

### IN Scope

| Feature | Why It's Essential (hypothesis it tests) | Build Effort | Acceptance Criteria |
|---|---|---|---|
| [Feature] | [Without this, we can't test X] | S/M/L | [Specific test] |

### OUT of Scope (Explicitly)

| Feature | Why Excluded | When to Revisit |
|---|---|---|
| [Feature] | [Specific reason] | [Specific trigger signal] |

---

## What We're Faking / Manually Doing ⚠️
> This section is mandatory. If you're not faking anything, you're over-building.

| Manual Process | What We're Avoiding Building | Automate When |
|---|---|---|
| [Process] | [What it replaces] | [After X signal] |

---

## Validation Plan

**Who will use the MVP:** [N specific users — named or described — recruited how?]

**Minimum Supply Threshold (marketplaces):** ⚠️
> Do NOT activate any demand-side marketing until [N supply providers] are live and active.
> Launching with insufficient supply is the fastest way to poison word-of-mouth in small markets.

**Core user action we're watching:**
> [The single most important action — the one that validates the whole thesis]

**Timeline:**
[Week-by-week with specific deliverables]

**Go / No-Go Decision Framework:**

| Signal | Go | No-Go |
|---|---|---|
| [Metric 1] | [> X] | [< X] |
| [Metric 2] | [Observed] | [Not observed] |

**No-Go Pivot — What We Actually Do Next:** ⚠️
> If No-Go: we do NOT just "do less of the same thing." We pivot to [specific alternative model].
> The pivot must be genuinely different — a new hypothesis, not a scaled-down version of the failed one.
> Pivot option: [Describe the specific alternative — e.g., concierge model with human dispatch]
> Why the pivot is viable: [Specific reason]
> Why it's not just giving up: [What we'd learn from it]
```

---

## 06. Competitive Analysis

```markdown
# Competitive Analysis: [Market/Category]

**Date:** [Date]
**Purpose:** [What decision does this inform?]

---

## Most Dangerous Competitor — Deep Dive ⚠️
> Before the comparison table, identify and deeply analyze the most dangerous competitor. This is often NOT the most obvious one. It's the one with the lowest switching cost for your users.

**[Competitor Name]:**
- What they do: [Description]
- Why they're the most dangerous: [Reason — usually: they require no behavior change from users]
- Their real advantage: [Not just "they're free" — what specifically makes them sticky]
- Their structural weakness: [The specific gap you can exploit]
- What you must do differently to beat them: [Specific — not "better UX"]
- Risk scenario: What if they add [one feature]? Does your moat hold?

---

## Competitive Landscape Map

### Direct Competitors
| Company | Solution | Pricing | Strengths | Weaknesses | Threat Level |
|---|---|---|---|---|---|
| [Name] | [How they solve it] | [Price] | [What they do well] | [Gap] | Critical/High/Med/Low |

### Indirect Competitors
| Company | How users solve it today | Real advantage (not just "free") | Their weakness |
|---|---|---|---|
| [Name] | [Method] | [Why users actually prefer it] | [Exploitable gap] |

---

## Feature Comparison Matrix

| Feature | Us | [Comp 1] | [Comp 2] | [Comp 3] |
|---|---|---|---|---|
| [Feature] | ✅ | ❌ | ✅ | 🔶 |

Legend: ✅ Strong | 🔶 Partial | ❌ Missing

---

## Multi-Homing / Dual-Listing Risk ⚠️
> For marketplaces: supply providers will be on multiple platforms simultaneously. This is not a risk to mitigate — it is a certainty to design for.

| Supply behavior | Likelihood | Impact | How to design for it |
|---|---|---|---|
| Drivers stay on WhatsApp groups while using app | High | Medium — reduces exclusivity | Design for coexistence; position app as "more rides, not different rides" |
| Drivers cherry-pick high-value rides from app | High | Medium | Acceptance rate tracking; gentle nudges, not punishments |
| Drivers direct repeat customers off-platform | Medium | High — revenue leakage | Build loyalty features that make app-based repeat booking easier than off-platform |

---

## Where We Win
1. [Specific advantage — traceable to a user behavior, not a feature claim]
2. [Specific advantage]

## Where We Lose (Be Honest)
1. [Honest assessment]
2. [Resource or brand disadvantage]

---

## Competitive Moat Assessment

| Advantage | Copyable? | Timeframe to Copy | Why | Our Response Time |
|---|---|---|---|---|
| [Advantage] | Hard/Med/Easy | [Time] | [Reason] | [How fast we can reinforce] |

---

## Strategic Implications
1. [Implication — specific enough to change a product decision]
2. [Implication]
```

---

## 07. Go-to-Market Plan

```markdown
# Go-to-Market Plan: [Product Name]

**Launch Date:** [Target]

---

## Launch Objective (One Sentence)
> [What does success look like 30 days post-launch — specific and measurable]

---

## PART 1: SUPPLY ACQUISITION (Comes First) ⚠️
> For any marketplace, supply acquisition is the GTM plan. Without supply, demand activation is guaranteed to fail and will poison word-of-mouth in small, tight-knit markets.

### Minimum Supply Threshold
> **Do not begin any rider/demand marketing until [N supply providers] are live and active.**
> Rationale: [Why this specific number is the minimum viable supply]

### Supply Acquisition Channels

| Channel | Strategy | Expected Supply | Cost | Priority |
|---|---|---|---|---|
| [Direct outreach — founder's network] | [Specific approach] | [N providers] | [Cost] | P0 |
| [Community/union partnership] | [Specific approach] | [N providers] | [Cost] | P0 |
| [Referral from onboarded supply] | [Specific approach — stress-tested] | [N providers] | [Cost] | P1 |

### Supply Referral Reality Check ⚠️
> "Each driver invites 5 customers" assumes drivers want to share their customer relationships with the platform. Many supply providers will see this as a threat to their direct relationships.
> Honest assessment: [Will this channel actually work? Under what conditions?]
> Alternative if it doesn't: [Specific backup]

### Supply Onboarding Plan
- How you onboard the first [N] providers: [Specific steps]
- What they're promised: [What's in it for them — specific]
- How you maintain supply engagement: [Specific mechanism]
- What you do when a supply provider goes inactive: [Specific protocol]

---

## PART 2: DEMAND ACTIVATION (Starts After Supply Threshold Met)

### Target Audience
**Primary segment:** [Specific — not "professionals"]
**Why them first:** [Reason]
**Where to find them:** [Specific channels]
**All segments from User Research Brief must be addressed here:** ⚠️
- [Segment 1] acquisition: [Specific]
- [Segment 2 — e.g., elderly] acquisition: [How you reach them — they likely don't download apps themselves]

### Positioning
**Headline:** [One sentence]
**Tagline:** [Short phrase]

### Demand Acquisition Channels

| Channel | Strategy | Expected Reach | Cost | Priority |
|---|---|---|---|---|
| [Channel] | [Specific tactic] | [N users] | [Cost] | P0/P1/P2 |

---

## Launch Phases (With Math) ⚠️

> Each phase must have supply × rides-per-day math that supports the phase objective.

### Phase 1: Supply Buildout (Before Public Launch)
- **Who:** [N supply providers only]
- **Goal:** Hit minimum supply threshold
- **Math:** [N drivers × X rides/day = Y rides available]
- **Exit criteria:** [Specific supply threshold met]

### Phase 2: Soft Launch
- **Who:** [N supply + N demand — closed beta]
- **Goal:** Validate end-to-end flow
- **Math:** [N drivers × X rides/day = capacity for N riders]
- **Success criteria:** [Specific]

### Phase 3: Limited Launch
- **Who:** [Broader demand cohort]
- **Goal:** Validate retention signal
- **Math:** [N drivers × X rides/day = capacity for N riders]
- **Success criteria:** [Specific — retention metric]

### Phase 4: Public Launch
- **Who:** Open access in pilot market
- **Goal:** Scale to launch objective
- **Success criteria:** [Specific — matches launch objective]

---

## Launch Checklist
- [ ] Supply: [Minimum N providers live and active — this gates everything else]
- [ ] Product: [Both apps live on distribution platform]
- [ ] Analytics: [All key events tracked]
- [ ] Support: [Protocol live]
- [ ] Legal: [Compliance items complete]
- [ ] Safety: [Protocol documented — what happens on day one of a safety incident]

---

## Risk: What Could Kill the Launch?

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Insufficient supply before demand activation | High | Critical | Hard gate: no demand marketing before supply threshold |
| Supply providers share customers off-platform | High | High | Design for coexistence; build switching costs over time |
| [Other risk] | [H/M/L] | [H/M/L] | [Specific plan] |
```

---

## 08. Metrics & Success Framework

```markdown
# Metrics Framework: [Product Name]

**Date:** [Date]

---

## North Star Metric ⚠️
> **[Metric name]** — [Definition that includes BOTH completion AND payment]
>
> For marketplace: A "completed ride" only counts if the payment is processed through the platform. Rides that complete but are paid in cash off-platform are revenue leakage and must be tracked separately.

**Why this metric (and not alternatives):**
- It measures user value AND business health
- It captures supply (providers available) AND demand (users booking) working together
- It cannot be gamed without actually delivering value

**Current baseline:** 0
**Target:** [N/week at Month 1, Month 3, Month 6, Month 12]

---

## Metric Hierarchy

```
North Star: [Metric — with payment completion in definition]
│
├── Demand Metrics
│   ├── New [demand users] per week
│   ├── [Demand user] signup → first transaction conversion
│   └── 7-day [demand user] retention
│
├── Supply Metrics  
│   ├── New [supply providers] onboarded per week
│   ├── [Supply provider] daily active rate
│   └── Transactions per [supply provider] per day
│
├── Marketplace Health
│   ├── Average match time
│   ├── Request timeout/unfulfilled rate
│   └── Transaction completion rate
│
└── Guardrail Metrics (must not decline)
    ├── Payment completion rate (% of completed transactions paid through platform) ⚠️
    ├── [Supply provider] churn rate (must stay < X%)
    └── Safety incident rate (must stay at 0 for MVP)
```

---

## Funnel Metrics

| Stage | Metric | Current | Month 1 Target | Month 6 Target | Owner |
|---|---|---|---|---|---|
| Acquisition | [Demand signups/week] | 0 | [N] | [N] | [Person] |
| Acquisition | [Supply onboards/week] | 0 | [N] | [N] | [Person] |
| Activation | [Signup → first transaction] | 0% | [X%] | [X%] | Product |
| Engagement | [Transactions/active user/week] | 0 | [N] | [N] | Product |
| Retention | [7-day demand retention] | 0% | [X%] | [X%] | Product |
| Revenue | [GMV/week] | 0 | [₹/$/X] | [₹/$/X] | Finance |
| Revenue | [Platform revenue/week (GMV × take rate)] | 0 | [₹/$/X] | [₹/$/X] | Finance |
| Referral | [% new demand from referral] | 0% | [X%] | [X%] | Growth |

---

## What Good Looks Like

| Metric | Bad | OK | Good | Great |
|---|---|---|---|---|
| [Demand signup → first transaction] | <15% | 15-30% | 30-45% | >45% |
| [Supply daily active rate] | <30% | 30-50% | 50-70% | >70% |
| [Match/connect time] | >[X min] | [X-Y min] | [Y-Z min] | <[Z min] |
| [Transaction completion rate] | <60% | 60-75% | 75-85% | >85% |
| [Payment through platform rate] | <40% | 40-60% | 60-75% | >75% |

---

## Anti-Metrics (What Not to Optimize For)
- **Total [demand user] registrations** — meaningless without first transaction
- **Total [supply provider] signups** — meaningless without active usage
- **App store ratings** — lagging and gameable; fix issues, don't chase ratings
- **Requests submitted** — inflates with failed/timeout requests; track completed only
- **[Any metric that can be hit without delivering user value]**

---

## Experiment Framework

For every feature shipped:
1. **Hypothesis:** If we do X, then Y will happen because Z
2. **Primary metric:** [Specific movement that confirms hypothesis]
3. **Guardrail metric:** [What must not drop — especially payment completion rate] ⚠️
4. **Duration:** [Minimum run time]
5. **Decision criteria:** Ship / Kill / Iterate

### Template Experiments

**Experiment: [Free first transaction]**
- Hypothesis: [If free first, then signup → first transaction increases by X% because cost is barrier]
- Primary: Signup → first transaction rate
- Guardrail: Transaction completion rate AND payment platform rate must not drop ⚠️
- Duration: 2 weeks minimum
- Decision: Ship if >[X%]; kill if <[Y%]

**Experiment: [Supply online reminders]**
- Hypothesis: [If reminders at peak hours, then supply daily active rate increases by X% because...]
- Primary: Supply daily active rate
- Guardrail: Supply churn must not increase
- Duration: 2 weeks
- Decision: Ship if >[X%]
```

---

## 09. Risk & Trade-off Register

```markdown
# Risk & Trade-off Register: [Product Name]

**Date:** [Date]
**Last Updated:** [Date]

---

## Risk #1: Kill-Switch Assumption ⚠️
> [The kill-switch assumption from the Problem Brief] — if this assumption is false, the entire strategy fails.
> **This is the first risk to validate, before any other risk mitigation matters.**

| ID | Risk | Category | Likelihood | Impact | Early Warning Signal | Mitigation |
|---|---|---|---|---|---|---|
| R0 | Kill-switch assumption: [State it] | Market | [H/M/L] | Critical | [Specific signal] | Validate in Week [X] before build begins |

---

## Critical Risks

| ID | Risk | Category | Likelihood | Impact | Early Warning Signal | Mitigation Plan |
|---|---|---|---|---|---|---|
| R1 | [Supply doesn't adopt platform] | Market | High | Critical | [<30% active weekly] | [Specific: in-person training, incentive for first N transactions] |
| R2 | [Demand doesn't switch behavior] | Market | Medium | High | [<20% signup→first transaction] | [Specific: free first transaction, personal follow-up] |
| R3 | [Insufficient supply → long wait times] | Execution | High | High | [Match time >X min] | [Hard gate: cap demand until supply threshold met] |
| R4 | [App crashes / poor performance] | Technical | Medium | Critical | [Crash rate >2%] | [Staged rollout: 10%→50%→100%; crash reporting live before launch] |

### Safety Risk — Special Note ⚠️
> Safety risks must NEVER be rated below "Medium" likelihood when supply providers are unverified in MVP.
> "Low likelihood" on safety is wishful thinking, not risk management.

| ID | Risk | Likelihood | Impact | **Day-One Protocol** |
|---|---|---|---|---|
| R_Safety | Safety incident in early days | **Medium** (not Low) | Critical | [Specific: who to call, what to post, how to support user, insurance status] |

> **Day-One Safety Protocol must include:**
> - Who handles the incident (named person, not "the team")
> - What communication goes to the affected user within [X hours]
> - What communication goes to the market within [X hours]
> - What makes the platform go offline vs. continue operating
> - Insurance status: [Current coverage / gap / planned date to have coverage]

---

## Payment & Supply Relationship Risks ⚠️

| ID | Risk | Likelihood | Impact | Early Warning Signal | Mitigation |
|---|---|---|---|---|---|
| R_Pay | Supply providers dispute commission or feel cheated | Medium | High | Complaints in community channels; departure of early adopters | Personal settlement for early disputes; transparent payment dashboard; lock-in of rates before onboarding |
| R_Leak | Supply providers direct repeat customers off-platform | High | High | Payment-through-platform rate drops below [X%] | Build features that make on-platform repeat booking easier than off-platform; loyalty for demand users |
| R_Multi | Supply multi-homes across platforms simultaneously | High (Certainty) | Medium | [Can't prevent — design for it] | Accept multi-homing; compete on volume of bookings, not exclusivity |

---

## Key Trade-offs Made

| Decision | What We Chose | What We Gave Up | Why | Reversible? | Notes |
|---|---|---|---|---|---|
| [Commission rate] | [X%] | [Lower rate attractiveness] | [Unit economics require it] | **Difficult — lowering is easy, raising is nearly impossible** | ⚠️ This is asymmetric: model unit economics at this rate before locking in |
| [Platform exclusivity] | [Non-exclusive] | [Cleaner marketplace] | [Can't enforce exclusivity with unorganized supply] | Yes | Design for multi-homing |

---

## Assumptions at Risk

| Assumption | Confidence | Validation Method | Status | Deadline |
|---|---|---|---|---|
| [Kill-switch assumption] | [H/M/L] | [Specific test] | [Validated/Planned] | [Before build] |
| Commission rate acceptable to supply | Low | [Test with first N providers; track churn] | Planned | [Week X] |
| [Other critical assumption] | [H/M/L] | [Test] | [Status] | [Date] |

---

## Dependency Risks

| Dependency | Owner | Risk If Delayed | Contingency |
|---|---|---|---|
| [Third-party service] | External | [Impact] | [Specific fallback] |

---

## What We're Watching Weekly
- **Supply active rate** — if below [X%], marketplace is failing
- **Demand signup → first transaction** — if below [X%], UX or value prop is broken
- **Payment through platform rate** — if below [X%], revenue leakage is happening ⚠️
- **Match/connect time** — if above [X min], insufficient supply
- **Community sentiment** (WhatsApp groups, reviews) — any spike = systemic issue
```

---

## 10. Execution Roadmap

```markdown
# Execution Roadmap: [Product Name]

**Date:** [Date]
**Planning Horizon:** [N months]
**Team:** [N people — all roles named]

---

## Roadmap Philosophy
> Speed of learning over speed of shipping. Every phase ends with a **decision**, not just a delivery. If a phase doesn't produce a clear signal, we **stop and reassess** — not push forward.

---

## Phase Overview

| Phase | Name | Duration | Objective | Exit Criteria (Go/No-Go) |
|---|---|---|---|---|
| 0 | Discovery | [N weeks] | Validate kill-switch assumption | Kill-switch: Validated OR Invalidated (not still open) |
| 1 | Build | [N weeks] | Working product end-to-end | [N test transactions completed without assistance] |
| 2 | Pilot | [N weeks] | Validate core loop with real users | Go/No-Go criteria from MVP Scope met |
| 3 | Iterate | [N weeks] | Fix and improve | [Specific metric threshold] |
| 4 | Scale | [N weeks] | Replicate in new markets | [Supply gate met in each new market before launch] |

---

## Phase 0: Discovery — [Date Range]

**Objective:** Validate kill-switch assumption before writing a single line of code.
**Exit Criteria:** Kill-switch assumption [Validated / Invalidated] — binary. No ambiguity.

| Week | Focus | Deliverable | Owner |
|---|---|---|---|
| Week 1 | Kill-switch validation | [Specific interviews/tests] | [Person] |
| Week 2 | Supply commitment | [N supply providers committed in writing] | [Person] |

**Do not proceed to Phase 1 if kill-switch assumption is not resolved.**

---

## Phase 1: Build — [Date Range]

**Objective:** Build minimum working product.
**Exit Criteria:** [N test transactions end-to-end, no critical bugs]
**Team Size Reality Check:** ⚠️ [N developers building X, Y, Z in N weeks] — flag if aggressive.
**Pre-decided scope cuts if behind schedule:**
1. [First thing to cut]
2. [Second thing to cut]

---

## Phase 2: Pilot — [Date Range]

**Objective:** Validate or kill the core hypothesis.
**Exit Criteria:** Go/No-Go criteria from MVP Scope (exact copy here)

| Signal | Go | No-Go |
|---|---|---|
| [Metric 1] | >[X] | <[X] |
| [Metric 2] | >[X] | <[X] |

**Supply gate before demand activation:** ⚠️
> Demand marketing does not begin until [N supply providers] are live and active.

---

## Phase 3: Iterate — [Date Range]

**Objective:** Fix what's broken, improve core loop.
**Rule:** Only ship what moves the North Star metric. Nothing else.

---

## Phase 4: Scale to New Markets — [Date Range]

**Objective:** Prove replication.

### New Market Entry Gate ⚠️
> Every new market/city requires this gate before launch. Do NOT apply a blanket "same playbook" without meeting supply minimums.

| Gate Criterion | Threshold | Status |
|---|---|---|
| Supply providers committed (in writing) | ≥ [N] | [Met/Not Met] |
| Supply providers onboarded and active | ≥ [N] | [Met/Not Met] |
| Demand seed users identified | ≥ [N] | [Met/Not Met] |

**Market 2 does not launch until these gates are met. No exceptions.**

---

## What's NOT on the Roadmap (Intentionally)

| Item | Why Excluded | Trigger to Add |
|---|---|---|
| [Feature/initiative] | [Specific reason] | [Specific signal — not just time] |

---

## Resource Requirements

| Phase | Team | Skills | Budget | Revenue at End |
|---|---|---|---|---|
| [Phase] | [N people] | [Skills] | [$X] | [$X — or "pre-revenue"] |

**Unit Economics Check:** ⚠️
> At end of Phase [X]: [N transactions/week] × [avg transaction] × [take rate] = [Revenue/week]
> Monthly ops cost: [$X]
> Runway: [N months at this burn rate]

---

## Decision Log

| Date | Decision | Rationale | Made By | Reversible? |
|---|---|---|---|---|
| [Date] | [Decision] | [Why] | [Who] | Yes/No |
```
