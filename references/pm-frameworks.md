# PM Frameworks Reference — ProductManager Skill (v2)

Quick-access frameworks for product analysis, document generation, and quality checks.

---

## Kill-Switch Assumption Framework ⚠️

Before any strategy or build work, identify the ONE assumption that, if false, makes the product unviable.

```
Kill-Switch Assumption Test:
"What is the single thing that must be true for this product to work?"

For marketplaces: usually "supply will adopt the platform and stay"
For SaaS: usually "users will pay [price] for [value]"
For consumer apps: usually "users will change [specific behavior]"

Format:
"If [assumption] is false, then [consequence that ends the product]."
Confidence: High / Medium / Low
How to validate: [Specific test — interviews, pricing test, pilot]
Deadline: [Must be answered BEFORE build begins]
```

This assumption becomes Risk #1 in every risk register. Everything else is secondary.

---

## Marketplace Cold-Start Framework ⚠️

### The Supply-First Rule
**Never activate demand before supply is live.**

```
Minimum Viable Supply = the fewest supply providers needed so that
demand users don't experience failure on first use.

If a rider opens the app and no drivers are available → they churn AND they tell others.
In tight-knit tier-2/3 communities, word of mouth is both your growth engine AND your kill switch.
One bad launch day can permanently poison a small market.
```

### Supply Acquisition Before Demand Acquisition
For any marketplace GTM plan:
1. **Supply acquisition plan** (Phase 1 — comes first)
2. **Supply minimum threshold** (gate before demand activation)
3. **Demand acquisition plan** (Phase 2 — only after gate is met)

### Multi-Homing Design Principle
Supply providers will be on multiple platforms simultaneously. This is not a risk — it is a certainty.

```
Do NOT:
- Try to enforce exclusivity (impossible with fragmented supply)
- Punish multi-homing (drives supply away)
- Assume supply referral channels work (providers may resist sharing customers)

DO:
- Design for coexistence ("more rides on top of what you already do")
- Build demand-side loyalty that makes on-platform repeat easier than off-platform
- Track payment-through-platform rate as a guardrail metric (revenue leakage signal)
- Position as "more bookings, not different bookings"
```

### Supply Referral Stress-Test
Before counting on supply referral as a GTM channel, ask:
- "Will providers want to share their direct customer relationships with the platform?"
- "Does sharing customers with us threaten their off-platform income?"
- If yes to either → supply referral is an optimistic channel, not a reliable one.

---

## Unit Economics Framework ⚠️

Every monetization claim must be traceable. No SOM number without math.

### Basic Unit Economics Model
```
Revenue per transaction = Avg Transaction Value × Take Rate
Gross Margin per transaction = Revenue per transaction - Variable Cost per transaction

CAC (Customer Acquisition Cost) = Total Marketing Spend / New Customers Acquired
LTV (Lifetime Value) = Avg Revenue per Customer per Month × Avg Customer Lifespan (months)
LTV:CAC ratio target: > 3:1 (viable), > 5:1 (healthy)

Payback Period = CAC / Monthly Revenue per Customer
Target: < 12 months for most models
```

### SOM Calculation Template
```
SOM = N users × frequency/month × avg transaction × take rate × 12
     = [fill in] × [fill in] × [fill in] × [fill in] × 12
     = $[X]/year

Monthly ops cost = $[Y]
Monthly revenue at SOM = $[X/12]
Margin = $[X/12 - Y]

Is this sustainable? Y/N
If not: at what scale does it become sustainable? [N users]
How long to reach that scale? [N months]
```

### Commission Rate Asymmetry Rule ⚠️
```
Lowering commission: easy (users and supply celebrate)
Raising commission: nearly impossible (supply revolt, word spreads in community, competitors use it against you)

→ Before locking in a commission rate, model unit economics at that rate.
→ If it doesn't work at that rate, fix the model — don't plan to raise later.
→ Always state: "At [X]% commission, we reach sustainability at [N] transactions/month."
```

---

## Prioritization Frameworks

### RICE Scoring
```
Score = (Reach × Impact × Confidence) / Effort

Reach:      # users affected per quarter
Impact:     0.25 (minimal) / 0.5 (low) / 1 (medium) / 2 (high) / 3 (massive)
Confidence: 50% / 80% / 100%
Effort:     person-weeks
```

### Impact vs Effort Matrix
```
HIGH IMPACT + LOW EFFORT  → Do First    (Quick Wins)
HIGH IMPACT + HIGH EFFORT → Plan        (Strategic Bets)
LOW IMPACT  + LOW EFFORT  → If Time     (Fill-ins)
LOW IMPACT  + HIGH EFFORT → Never Do    (Time Sinks)
```

### Kano Model
| Category | Definition | Implication |
|---|---|---|
| Must-Have | Absence = dissatisfaction; presence = neutral | Required — don't ship without |
| Performance | More = better | Core differentiator — invest here |
| Delighter | Unexpected; creates delight | Bonus — don't prioritize over Must-Haves |
| Indifferent | Users don't care | Don't build |
| Reverse | Some users hate this feature | Research before building |

---

## Problem Frameworks

### Jobs to Be Done (JTBD)
```
"When [situation], I want to [motivation], so I can [outcome]."

Functional job: What they're literally trying to do
Emotional job:  How they want to feel
Social job:     How they want to be perceived
```

Always identify all three layers. Products that only serve the functional job are easier to replace.

### 5 Whys (Root Cause)
Keep asking "why" until you hit the cause, not a symptom:
1. [Symptom]
2. Why? → [Next layer]
3. Why? → [Next layer]
4. Why? → [Next layer]
5. Why? → **Root cause found**

Stop building solutions for symptoms.

### Problem/Solution/Market Fit Triangle
```
All three must align. Most products fail because they solve a real problem
for the wrong market, or with a solution that requires too much behavior change.

         PROBLEM (real? specific? painful?)
        /                                  \
       /                                    \
  SOLUTION (10x better?)     ←→      MARKET (reachable? payable?)
```

---

## User Research Frameworks

### Lean User Persona
```
Name:             [Fictional — makes them human]
Role/Context:     [Specific — not "professional"]
Goal:             [What they're trying to achieve]
Current behavior: [Named workaround — what they do today]
Pain:             [Specific friction — not "it's slow"]
Trigger:          [What makes them seek a new solution]
Kill-switch:      [What would make them never use your product]
Quote:            "[Direct quote from research that captures their mindset]"
```

### Empathy Map
```
SAYS:    [Direct quotes from interviews]
THINKS:  [What they believe but don't say aloud]
DOES:    [Observed behaviors — not reported behaviors]
FEELS:   [Emotional state — anxiety, frustration, pride]
```

Note: DOES beats SAYS. What people do is more reliable than what they say they do.

---

## Strategy Frameworks

### Product-Market Fit Signals
```
Strong signals:
- >40% of users say "very disappointed" if product disappears (Sean Ellis test)
- NPS > 50
- >25% of new users from organic word-of-mouth
- Users ask for paid features when product is free
- Day 30 retention > 25% (consumer), > 60% (SaaS)

Weak signals (don't count these):
- Downloads / signups (vanity)
- Press coverage
- App store ratings < 1000 reviews
- Investor interest
```

### Competitive Window Evidence Requirements
Any claim that "we have X months before [competitor] enters" must be supported by:
- Public statements (earnings calls, press releases)
- Job postings (or absence of job postings)
- Market entry history (how long they took in comparable markets)
- OR explicitly labeled as [Assumed] with a confidence level

Never state a competitive window as fact without evidence.

### Blue Ocean Analysis
```
Eliminate: What factors does the industry take for granted that add cost without value?
Reduce:    What factors can be reduced below industry standard without losing demand?
Raise:     What factors should be raised above industry standard?
Create:    What factors should be created that the industry has never offered?
```

---

## Metrics Frameworks

### AARRR (Pirate Metrics) — With Supply Side ⚠️
For marketplaces, run AARRR for BOTH demand AND supply:

```
              DEMAND SIDE          SUPPLY SIDE
Acquisition:  [Demand channel]     [Supply channel]
Activation:   [First transaction]  [First job accepted]
Retention:    [Return rate]        [Weekly active rate]
Referral:     [NPS / word of mouth][Invites others]
Revenue:      [GMV generated]      [Earnings consistency]
```

The supply side AARRR is where most marketplace products fail silently.

### North Star Framework
```
North Star = the one metric that captures the core value delivered to users AND correlates with revenue

Must satisfy:
1. Measures user value (not just activity)
2. Correlates with revenue
3. Team can directly influence it
4. Leading indicator, not lagging
5. For marketplaces: INCLUDES payment completion (not just activity completion) ⚠️
```

### Retention Benchmarks (Consumer)
```
Day 1:  Good > 40%,  Great > 60%
Day 7:  Good > 20%,  Great > 40%
Day 30: Good > 10%,  Great > 25%
```

Below Day 30 retention of 10% → product does not have market fit. Fix retention before scaling acquisition.

### SaaS Health Metrics
```
NRR (Net Revenue Retention):  > 110% = strong
Monthly Churn:                < 2% = healthy
CAC Payback Period:           < 12 months = efficient
LTV:CAC ratio:                > 3:1 = viable
```

---

## MVP Frameworks

### Minimum Viable Tests (Cheapest to Most Expensive)
Run the cheapest test that can falsify your kill-switch assumption:

1. **Conversation test** — Talk to 10 people. Will they use it? Will they pay?
2. **Landing page test** — Does anyone click "sign up" before the product exists?
3. **Concierge MVP** — Do it manually for 5 users. No code needed.
4. **Wizard of Oz** — Fake automation (humans behind the scenes)
5. **Prototype test** — Clickable mockup; watch users try to complete the flow
6. **Smoke test** — Build front-end only; measure demand before building back-end
7. **Functional MVP** — Minimal working product in production

Most teams skip to #7 and spend months building before validating #1.

### The Riskiest Assumption Test (RAT)
```
Step 1: Identify the ONE assumption that would kill the product if false
Step 2: Design the cheapest possible test to validate it
Step 3: Run that test BEFORE building anything else
Step 4: If validated → proceed to build
        If invalidated → pivot the assumption, NOT the product

The RAT is always more important than any feature on the roadmap.
```

### No-Go Pivot Rules ⚠️
When a No-Go signal is hit:
```
BAD pivot: "We'll do less of the same thing" (just a smaller version of the failed model)
GOOD pivot: "We'll test a fundamentally different hypothesis about the same problem"

A good pivot:
- Changes what's being assumed, not just the scope
- Is genuinely testable in <4 weeks
- Has a specific pass/fail criteria
- Is not just "find more users" or "simplify the app"
```

---

## Decision-Making Frameworks

### Reversibility Test (Type 1 vs Type 2 Decisions)
```
Type 1 (Irreversible): Slow down. More data. More input. These include:
  - Commission/pricing model
  - Core technology architecture
  - Key partnerships
  - Market positioning

Type 2 (Reversible): Move fast. Decide in hours. These include:
  - Feature additions
  - UI/UX changes
  - Marketing copy
  - Launch sequencing
```

Most teams treat Type 2 decisions like Type 1 (too slow) and Type 1 decisions like Type 2 (too fast).

### Pre-Mortem
Before launching: imagine it's 6 months later and the product failed.
Write down every specific reason why it failed.
The top 3 reasons that come up become your top 3 risks.
If you can't mitigate them, reconsider the strategy.

### Trade-off Articulation Template
```
"We chose [X] over [Y].
This means we win at [benefit] but sacrifice [cost].
We're making this bet because [strategic rationale].
We'll know this was wrong if [specific early warning signal].
This decision is [reversible / difficult to reverse] — [implication for speed of decision]."
```
