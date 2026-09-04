# ABSOLUTE DOLLAR INTELLIGENCE

# TRON — MASTER PRODUCT, WEBSITE & COMMERCIAL MD

**Status:** Living Master Document
**Last Updated:** 2026-09-04
**Product:** Absolute Dollar Intelligence (ADI)
**Current Product:** TRON Alpha V1.1
**Future Product:** TRON V2
**Website:** Lovable — ADI Front Door
**Commercial Access:** Whop — Commercial / Access Door
**Community / Onboarding:** WhatsApp
**Market Intelligence Delivery:** TradingView
**Core Philosophy:** Learn. Understand. Observe. Execute.

---

# 1. PURPOSE OF THIS DOCUMENT

This is the **Master MD** for Absolute Dollar Intelligence and the TRON product ecosystem.

It is not a temporary implementation plan.

It is not a marketing brief.

It is not a generic AI-generated product description.

It is the evolving source of truth that should be used to keep:

* the website,
* TRON product positioning,
* V1.1 documentation,
* V2 planning,
* commercial access,
* community onboarding,
* campaign messaging,
* technical implementation,
* and future AI-assisted development

aligned.

Whenever there is a conflict between this document and generic assumptions made by an AI, **this document wins** unless a newer explicit product decision supersedes it.

---

# 2. CORE PRODUCT PHILOSOPHY

## Absolute Dollar Intelligence

**Learn. Understand. Observe. Execute.**

ADI is being built around the idea that traders do not necessarily need another black-box system telling them what to do.

They need a framework that helps them **read the market**.

TRON is therefore fundamentally a:

> **deterministic market-intelligence and decision-support engine.**

TRON's job is to organize observable market information into an understandable operating framework.

The philosophy is:

> **TRON DOES NOT NEED TO PREDICT PRICE.
> TRON NEEDS TO READ PRICE EXCEPTIONALLY WELL.**

The operator remains responsible for the final decision and execution.

TRON should therefore never be positioned as:

* guaranteed profit,
* guaranteed accuracy,
* a magical prediction engine,
* a black-box signal seller,
* or a substitute for operator judgment.

---

# 3. THE THREE-LAYER ADI ARCHITECTURE

The ecosystem is built around:

## ANALYSIS → CAPITAL → EXECUTION

### Analysis

TRON reads and organizes market information.

This includes:

* market structure,
* momentum,
* trend alignment,
* liquidity,
* sessions,
* PSAR context,
* liquidity trail,
* multi-timeframe context,
* and position framing.

### Capital

The operator applies the framework within their own capital/risk framework.

ADI should educate and provide structure rather than make personalized financial decisions for the operator.

### Execution

The operator decides whether and how to execute.

TRON can provide market context and execution-readiness information, but:

> **TRON provides market intelligence. The operator remains responsible for final decision and execution.**

---

# 4. CURRENT PRODUCT STATE

## TRON Alpha V1.1

**V1.1 is the current live baseline.**

TradingView product:

**Absolute Dollar Agent + ICT Killzones [EAT]**

TradingView URL:

https://www.tradingview.com/script/V1lm98sj-Absolute-Dollar-Agent-ICT-Kill-zones-EAT/

Short identity:

**TRON Alpha**

V1.1 is the product that should currently be presented publicly.

The old August 2026 positioning such as:

* FREE BETA
* Free Forever
* No Trial
* Beta-only positioning

is stale unless explicitly reintroduced as part of a future campaign decision.

V2 is **not the current product**.

---

# 5. V1.1 PRODUCT IDENTITY

TRON Alpha V1.1 is a deterministic Pine Script market-intelligence framework combining:

1. ICT Killzones & Pivots
2. Absolute Dollar Agent
3. Smart PSAR Filter
4. Unified Dashboard

The system is designed to make market state visible rather than hiding the reasoning behind a single opaque signal.

---

# 6. V1.1 CORE COMPONENTS

## 6.1 ICT Killzones & Pivots

Current EAT session structure:

| Session           |    Time EAT | Code |
| ----------------- | ----------: | ---- |
| Asia              | 03:00–07:00 | H4-1 |
| London Open       | 07:00–11:00 | H4-2 |
| London Mid        | 11:00–15:00 | H4-3 |
| London–NY Overlap | 15:00–19:00 | H4-4 |
| NY PM             | 19:00–23:00 | H4-5 |

Current V1.1 defaults:

* Asia enabled
* London Open enabled
* London Mid enabled
* London–NY Overlap enabled
* NY PM disabled

Important:

There are **five H4 session blocks**, not six.

---

# 7. MARKET STRUCTURE

V1.1 uses market structure based on:

* HH
* HL
* LH
* LL
* BOS
* CHoCH

Default swing length:

**15**

Dashboard terminology:

**MS Bias**

V1.1 must not be described as having the full V2 SMC architecture.

---

# 8. RSI MOMENTUM

V1.1 defaults:

* RSI length: 10
* Bullish threshold: 55
* Bearish threshold: 48
* Exhaustion high: 85
* Exhaustion low: 20
* Sustain: enabled
* RSI EMA length: 3
* M5 confirmation: enabled
* RSI gate: enabled

The RSI system contributes to the deterministic decision framework.

---

# 9. SMART SIGNAL

V1.1 includes:

* Smart Bull
* Smart Bear
* No Signal

The Smart Signal is based on transition/event logic.

It should not automatically be described as the overall market bias.

The distinction between:

**event**

and

**bias**

must remain clear.

---

# 10. EMA / TREND

V1.1 EMA defaults:

* EMA 21
* EMA 55

Trend Truth / Momentum Trend combines:

* M5 smoothed RSI,
* five-bar price momentum,
* EMA direction.

Each contributes:

* +1
* 0
* -1

Overall state:

* Bullish
* Bearish
* Neutral

---

# 11. LIQUIDITY TRAIL

V1.1 defaults:

* Alpha Gate: false
* MA length: 13
* ATR length: 14
* ATR multiplier: 2.0

The executable source is authoritative.

A stale code comment suggesting MA 21 must not override the actual executable default of MA 13.

The Liquidity Trail is central to TRON's visual market-reading framework.

---

# 12. ALPHA GATE

Alpha Gate is **not the V1.1 default**.

It is an optional filter.

When enabled:

* bullish trail flips are constrained by EMA21 > EMA55
* bearish trail flips are constrained by EMA21 < EMA55

There is an important distinction:

### Source truth

Alpha Gate defaults to OFF.

### Operator recommendation

From live operator experience, Alpha Gate is recommended for **M1 analysis** where the operator wants the trail to remain more resistant to counter-trend flips.

This recommendation must never be presented as:

* a universal rule,
* a guaranteed improvement,
* or the source-code default.

---

# 13. SMART PSAR

V1.1 Smart PSAR defaults:

* Start: 0.02
* Increment: 0.02
* Maximum: 0.20
* MTF: 5 minutes
* ATR length: 14
* Sweep lookback: 5
* Decay: 50

PSAR contributes:

* direction,
* momentum context,
* MTF context,
* and filtering.

---

# 14. POSITION TOOL

V1.1 Position Tool:

* Enabled
* Entry mode: Signal Change
* Pin: false
* TP1: 1R
* TP2: 1.5R
* TP3: 2R
* Extend: 30
* BUY labels: enabled
* SELL labels: enabled

Entry:

**Close**

Stop framework:

**Liquidity Trail**

The position tool is a visual framing mechanism.

It must not be represented as a guarantee that a displayed target will be reached.

---

# 15. THE V1.1 BUY / SELL LABELS

This is an important V1.1 evolution.

## Explicit BUY / SELL labels

V1.1 introduces explicit BUY / SELL labels.

These are outputs of the deterministic engine, incorporating conditions such as:

* PSAR direction,
* RSI momentum,
* and the relevant signal-state logic.

They are **not decorative arrows**.

The website should explain this distinction clearly.

However:

A BUY or SELL label must not be marketed as:

* a guaranteed winning signal,
* a prediction,
* or an instruction that overrides operator judgment.

---

# 16. V1.1 RECOMMENDED WORKFLOW

The central public workflow should be:

# H1 → M15 → M5

### H1 — Macro View

Purpose:

**Macro context**

Observe:

* broad trend regime,
* EMA relationship,
* liquidity-trail context,
* RSI momentum,
* market structure,
* higher-timeframe location,
* session context.

### M15 — Tactical / Structural View

Purpose:

**Tactical structure**

Observe:

* structure,
* BOS / CHoCH,
* EMA,
* trail,
* momentum,
* PSAR,
* MTF context,
* session relationship.

### M5 — Execution Context

Purpose:

**Execution context**

Observe:

* momentum,
* Smart Signal,
* market structure,
* trail,
* EMA,
* PSAR,
* position framing.

The wording should remain:

> H1 = macro
> M15 = tactical / structural
> M5 = execution context

This describes how TRON is intended to be read.

It is not a promise of trade outcomes.

---

# 17. M1 OPERATOR WORKFLOW

M1 is a precision view rather than the primary macro framework.

When operating on M1:

> **Enable Alpha Gate** as an operator recommendation based on live use.

The purpose is to help keep the Liquidity Trail more stable against counter-trend flips.

Smart Signals can also be used in the M1 context.

Again:

* Alpha Gate is optional.
* Alpha Gate is not the V1.1 default.
* It is an operator recommendation.
* It is not a guaranteed optimization.

---

# 18. V1.1 UPDATE LOG

## What's new in V1.1

The website should contain a dedicated section immediately after **TRON in action** and before **The Tape**.

### Explicit BUY / SELL labels

Outputs of the deterministic engine, gated by PSAR direction and RSI momentum.

They are not arrows for their own sake.

### Recommended workflow: H1 → M15 → M5

Macro context → tactical structure → execution context.

### M1 operator recommendation

For M1 analysis, enable Alpha Gate based on live operator experience. It helps hold the Liquidity Trail flat against counter-trend flips.

This must be clearly presented as an operator recommendation rather than a universal rule or source default.

### Beyond beta

Refined from real operator feedback.

Beyond beta.

---

# 19. V1.1 DASHBOARD

V1.1 dashboard contains approximately 22 information rows, including:

* RSI Momentum
* Smart Signal
* MS Bias
* Momentum Trend
* EMA Cross
* Liquidity Trail
* Smart PSAR
* PSAR Momentum
* PSAR MTF Context
* Position
* Entry / SL
* TP1
* TP2
* TP3
* Active H4 Session
* H4 Previous Close
* H4 Current Open
* H4 Current High / Low
* H1 Previous Close
* Active KZ Range

The dashboard is important to TRON's identity because it exposes the information behind the visual output.

---

# 20. V1.1 ALERTS

Current alert categories include:

* RSI Bullish Breakout
* RSI Bearish Breakout
* Smart Bull Momentum
* Smart Bear Momentum
* Trail Bull Signal
* Trail Bear Signal
* Bull Trail Retest Entry
* Bear Trail Retest Entry
* Smart PSAR Flip

Important:

V1.1 does **not** contain dedicated alert conditions named:

* Tron Buy Entry
* Tron Sell Entry

Those are V2 concepts.

---

# 21. V2

## TRON V2 IS FUTURE — NOT CURRENT

V2 is the next evolution of the TRON architecture.

It must never be presented as currently live.

V2 includes substantially deeper structure and liquidity intelligence.

### V2 modules

#### A — ICT Killzones & Pivots

#### B — Absolute Dollar SMC

Including:

* full market structure,
* BOS / CHoCH,
* order blocks,
* FVG,
* EQH / EQL,
* premium / discount,
* strong / weak highs and lows.

#### C — Liquidity Suite

Including:

* buy-side liquidity,
* sell-side liquidity,
* volume profiles,
* liquidity-area logic.

#### D — Smart PSAR & Agent

Including:

* RSI Momentum,
* Smart Signals,
* PSAR,
* Liquidity Trail.

---

# 22. V2 DIFFERENCES

V2 has:

* SMC Bias rather than V1's MS Bias
* deeper market structure
* internal and swing order blocks
* equal highs/lows
* optional FVG
* premium/discount
* liquidity suite
* dedicated TRON Buy Entry
* dedicated TRON Sell Entry

V2 default Position Tool BUY/SELL labels are false.

These V2 features must **never be retroactively attributed to V1.1.**

---

# 23. V2 COUNTDOWN

Current planned release:

> **September 28, 2026 — provisional.**

This is a planned target, not a guaranteed release date.

V2 remains:

* not live,
* not included in V1.1,
* and subject to development/testing.

### Founding 50

Current planned founding pricing:

> **$49 lifetime**

The exact final founder terms must remain subject to explicit confirmation.

---

# 24. COMMERCIAL ARCHITECTURE

The product ecosystem now has a deliberate separation of responsibilities.

# Lovable = ADI FRONT DOOR

Lovable exists to:

* introduce ADI,
* explain TRON,
* establish trust,
* demonstrate the product,
* educate,
* guide visitors into onboarding,
* and direct them toward the appropriate next step.

Lovable should **not become the checkout system**.

---

# WhatsApp = ONBOARDING / COMMUNITY DOOR

WhatsApp is where the prospective operator can:

* enter the community,
* receive onboarding,
* ask questions,
* understand the framework,
* receive support,
* and progress through the evaluation/onboarding journey.

---

# TradingView = V1.1 PRODUCT DELIVERY

TradingView is where TRON Alpha V1.1 is actually experienced.

Current TradingView product:

**Absolute Dollar Agent + ICT Killzones [EAT]**

---

# Whop = COMMERCIAL / ACCESS DOOR

Whop should own:

* commercial purchase,
* entitlement,
* access management,
* paid-product experience,
* and eventually the transition into premium access.

Lovable should not try to duplicate Whop's commercial function.

---

# 25. TARGET FUNNEL

The intended ecosystem is:

**Instagram / Facebook / WhatsApp Status**

↓

**ADI / Lovable**

↓

**WhatsApp onboarding**

↓

**TRON Alpha V1.1 evaluation**

↓

**TradingView V1.1 experience**

↓

**Whop commercial access**

↓

**V2 evolution**

The fundamental distinction is:

> **Lovable is the front door.
> Whop is the commercial/access door.**

---

# 26. THE 7-DAY V1.1 EVALUATION

A planned onboarding journey includes a **7-day free V1.1 evaluation**.

This duration should only become public website copy once it is formally approved as the actual offer.

The intended journey is:

### Day 1

Understand TRON.

### Day 2

Understand the H1 → M15 → M5 framework.

### Day 3

Observe TRON across instruments.

### Day 4

Study structure, momentum and trail interaction.

### Day 5

Study execution-context reading.

### Day 6

Review observations and questions.

### Day 7

Evaluate whether the framework fits the operator.

The goal is not:

> “Take signals for seven days.”

The goal is:

> **Experience the framework and understand how TRON reads the market.**

---

# 27. POST-EVALUATION COMMERCIAL PATH

After the evaluation period, the intended commercial path is:

**V1.1 full access**

with a potential grandfather/founding offer.

Current working concept:

> **$24.50 / 50% off the $49 lifetime anchor**

for qualifying operators during the V1.1 → V2 transition.

This must not be hard-coded as a permanent public offer until the exact commercial terms are approved.

---

# 28. FOUNDING 50

There is a distinction between:

### Public V1.1 pricing

and

### Founding 50 / grandfather pricing

The Founding 50 should be treated as a special cohort.

Current planned anchor:

**$49 lifetime**

The precise grandfather mechanism and timing must be explicitly confirmed before implementation.

---

# 29. AFFILIATE / BROKER ECOSYSTEM

The broader ecosystem may eventually point operators toward relevant infrastructure for the instruments they choose to study.

Potential ecosystem references include:

* Deriv
* TradingView
* HFM
* Pepperstone
* Bybit
* other appropriate platforms

However:

**The website should not become a broker-deposit funnel.**

Broker references must be presented carefully and transparently.

Affiliate relationships should be disclosed.

No copy should imply:

* guaranteed profitability,
* guaranteed execution quality,
* guaranteed funding,
* or that depositing money is required to become successful.

---

# 30. ASSET-AGNOSTIC POSITIONING

TRON is intended to be **asset agnostic**.

The underlying market-reading framework can be applied across different instruments and environments, subject to the capabilities and data available on the relevant platform.

Potential examples include:

* Gold
* Forex / CFDs
* Synthetic Indices
* Crypto
* other supported TradingView instruments

The framework should therefore be positioned around **market structure and intelligence**, rather than around a single asset.

---

# 31. EXAMPLE MULTI-TIMEFRAME APPLICATIONS

These are framework examples, not trading instructions.

## Intraday / CFD / Gold

Potential conceptual workflow:

**H1 → macro view**

**M15 → tactical structure**

**M5 → execution context**

The purpose is to maintain context before examining lower-timeframe conditions.

---

## Synthetic Indices

For lower-timeframe analysis, the operator may use:

**M5**

with:

* Smart Signals,
* BUY / SELL labels,
* Liquidity Trail,
* momentum.

On:

**M1**

the operator may use:

* Alpha Gate,
* Smart Signals,
* Liquidity Trail,
* momentum.

This is an operator workflow observation, not a guarantee.

---

## Crypto

A broader structure can be:

**H4 → macro context**

**M15 → tactical / execution context**

**M5 → entry context**

Again, this is a conceptual framework for reading multiple timeframes rather than an instruction to trade.

---

# 32. THE WEBSITE

## Current Website

Project:

**absolute-dollar-intelligence**

Lovable project ID:

`0bfdc3ca-85e2-41e7-a3dc-9220eec805cc`

Production:

https://absolute-dollar-intelligence.lovable.app

TradingView:

https://www.tradingview.com/script/V1lm98sj-Absolute-Dollar-Agent-ICT-Kill-zones-EAT/

---

# 33. WEBSITE DESIGN PHILOSOPHY

The existing visual identity is important.

It is:

* premium,
* dark,
* modern,
* fintech-inspired,
* clean,
* technically sophisticated,
* subtly cyber/TRON,
* but not scammy.

Influence can feel similar to:

* Apple
* Linear
* Stripe
* Vercel
* Raycast

without becoming a copy of them.

### IMPORTANT

Do not redesign the established visual language simply because a new AI agent thinks it can make the page “better.”

The goal is:

> **Improve clarity and conversion without destroying authenticity.**

---

# 34. AUTHENTICITY PRINCIPLE

A major concern identified during the website iteration:

> **The page can become too conversational / too polished / too explanatory and lose the authenticity of the original builder voice.**

The website must still sound like:

**Emmanuel built TRON because he actually went through the process of developing, testing, refining and learning from it.**

Not like:

> “Here is an AI-generated fintech SaaS product description.”

The distinction matters.

TRON should feel:

* engineered,
* tested,
* observed,
* opinionated,
* transparent,
* and human.

The copy should not become sterile corporate marketing.

---

# 35. CURRENT WEBSITE STRUCTURE

Existing components include:

* Header / Nav
* Hero
* BetaBanner
* Pillars
* Tron
* TronInAction
* The Tape / Broadcast Archive
* JoinChannels
* TrustBar
* HowItWorks
* Pricing
* FAQ
* FinalCTA
* Footer
* StickyJoin

---

# 36. HERO

The Hero should establish immediately:

### What is TRON?

A market-intelligence framework.

### What is current?

TRON Alpha V1.1.

### What does the operator do?

Learn → understand → observe → make their own decision.

### Primary CTA

WhatsApp onboarding.

### Secondary CTA

TradingView V1.1.

The Hero must not claim:

* Free Forever,
* FREE BETA,
* guaranteed results,
* Prop Firm Ready,
* or unsupported performance.

---

# 37. “TRON IN ACTION”

This section is valuable because it demonstrates the product rather than merely describing it.

Current example contexts include:

### XAUUSD

Pepperstone / Asia session context.

### Volatility 75 (1s)

Deriv / NY Overlap context.

The images should demonstrate:

* structure,
* momentum,
* PSAR,
* trail,
* position framing,
* session context,
* dashboard information.

They should not be presented as proof of profitability.

---

# 38. “WHAT'S NEW IN V1.1”

This section belongs:

**AFTER TRON IN ACTION**

and:

**BEFORE THE TAPE**

It should communicate that V1.1 is a meaningful evolution rather than merely a renamed beta.

Required ideas:

### Explicit BUY / SELL labels

Deterministic outputs gated by relevant conditions including PSAR direction and RSI momentum.

### H1 → M15 → M5

The recommended multi-timeframe operating framework.

### M1 + Alpha Gate

Operator recommendation based on live use.

### Beyond beta

Refined from real operator feedback.

The tone should feel like:

> “Here is what changed because we actually used the thing.”

not:

> “Version 1.1 contains four exciting new features!”

---

# 39. THE TAPE

The Tape / Broadcast Archive should demonstrate TRON intelligence in action.

The canonical intelligence architecture is:

### H1 Macro Regime

* price/time/session
* EMA Cross
* Liquidity Trail
* RSI Momentum
* MS/SMC Bias
* Momentum Trend
* H4/H1 location
* TRON narrative
* state

### M15 Structural

* price/session
* MS Bias
* HH/HL/LH/LL
* BOS/CHoCH
* EMA
* Trail
* Momentum
* PSAR
* PSAR Momentum
* MTF
* narrative

### M5 Execution Context

* price/time
* RSI
* Smart Signal
* Momentum Trend
* MS Bias
* BOS/CHoCH
* Trail
* EMA
* PSAR
* PSAR Momentum
* MTF
* Position Tool
* Entry
* SL
* TP1/TP2/TP3
* narrative

The narrative must derive from actual state relationships.

Never invent:

* probabilities,
* win rates,
* certainty,
* targets,
* or market outcomes.

---

# 40. COMMUNITY ARCHITECTURE

## Telegram

Used for:

* broadcast,
* market intelligence,
* structured drops,
* H1/M15/M5 analysis.

## WhatsApp Group

Used for:

* conversation,
* onboarding,
* support,
* questions,
* community interaction.

## WhatsApp Channel

Used for:

* lower-noise broadcast,
* announcements,
* market intelligence.

The Execution War Room should remain private and access-controlled.

It should not be casually presented as a public free channel.

---

# 41. CTA HIERARCHY

The website should not have competing primary actions everywhere.

Current preferred hierarchy:

### Primary

**Start V1.1 Onboarding → WhatsApp**

### Secondary

**View TRON Alpha V1.1 → TradingView**

### Supporting

Telegram / WhatsApp Channel where appropriate.

The CTA hierarchy should make sense particularly on mobile because campaign traffic is expected to come heavily from:

* Instagram,
* Facebook,
* WhatsApp Status.

---

# 42. STICKY MOBILE CTA

The mobile sticky CTA should prioritize:

**WhatsApp onboarding**

with:

**TradingView V1.1**

as the secondary action.

The sticky bar should not overwhelm the actual content.

---

# 43. PRICING

Current standard commercial anchor:

# $49 lifetime

The website may communicate:

> TRON Alpha V1.1 — Lifetime Access

without inventing additional terms.

The $24.50 / 50%-off concept belongs to a controlled promotional/founding transition offer.

Do not permanently hard-code:

* discount countdowns,
* fake scarcity,
* unsupported trial lengths,
* or “only X remaining” unless those are real.

---

# 44. FAQ PRINCIPLES

FAQ should answer:

### Is TRON a signal service?

No.

TRON is a market-intelligence / decision-support framework.

### What is V1.1?

The current live TRON Alpha release.

### What is V2?

The future premium evolution.

### Is V2 live?

No.

### Does V2 come with V1.1?

Not automatically.

### How do I start?

Begin with the onboarding/evaluation path.

### Why WhatsApp?

Because onboarding and operator support happen there.

### What is the relationship with TradingView?

TradingView is where TRON Alpha V1.1 is experienced.

### What is Whop?

Whop is the commercial/access layer.

Avoid unsupported claims involving:

* prop-firm approval,
* guaranteed funding,
* guaranteed performance,
* or broker outcomes.

---

# 45. CLAIMS DISCIPLINE

All public claims should be classified as:

## Source-derived

Directly supported by the Pine implementation.

## Explicit product decision

A decision made by the product owner.

## Operator observation

Something learned from actual use.

## Planned

Future direction.

## Provisional

A target that may change.

The site must never blur these categories.

For example:

> “Alpha Gate is enabled by default.”

would be false.

Correct:

> “Alpha Gate is optional; operator experience has led to a recommendation for M1 use.”

---

# 46. WHAT MUST NEVER BE INVENTED

Do not invent:

* win rates,
* accuracy percentages,
* profitability statistics,
* guaranteed outcomes,
* backtest results,
* broker partnerships,
* funding partnerships,
* Whop URLs,
* trial duration,
* founder terms,
* V2 features in V1.1,
* V2 release certainty,
* user counts,
* performance claims,
* or testimonials.

If something is unknown:

**mark it as unresolved.**

---

# 47. SOURCE-OF-TRUTH HIERARCHY

When resolving contradictions, use this hierarchy:

1. Uploaded Pine source
2. Explicit current product decisions
3. Version-specific source-derived parameter inventory
4. Externalized TRON dictionary
5. Canonical Telegram / WhatsApp analysis templates
6. Current Lovable implementation
7. Generic AI assumptions

Generic AI assumptions are last.

---

# 48. TECHNICAL SOURCE TRUTH

V1.1:

* Pine Script v6
* max days: 2
* timeframe limit: 15m
* timezone: GMT+3
* await bar confirmation: true

The source code is authoritative over comments.

Where comments and executable logic disagree:

> **Executable logic wins.**

---

# 49. DOLLAR / RISK MATH

TRON has historically used:

`syminfo.pointvalue`

for dollar-risk / lot-sizing calculations.

There is a known concern:

> TradingView feeds can expose inconsistent point-value behavior across instruments/brokers.

Therefore dollar calculations should not be presented as universally equivalent to every broker's MT5 contract specification.

Any future risk-sizing implementation must account for instrument-specific contract specifications.

---

# 50. CURRENT RESEARCH PHILOSOPHY

TRON is not being redesigned simply to become a conventional trading strategy.

The research objective is:

> **Optimize parameters and configuration without destroying core logic.**

TRON's purpose is:

> **READ PRICE.**

The research framework should therefore investigate:

* parameter robustness,
* multi-timeframe behavior,
* session behavior,
* market structure,
* momentum,
* liquidity,
* PSAR,
* trail behavior,
* interactions,
* sensitivity,
* regime dependence,
* and forward robustness.

---

# 51. PARAMETER RESEARCH

Research should examine robust regions rather than obsess over a single magical number.

Primary contexts:

### H1

Macro regime.

### M15

Structural context.

### M5

Execution context.

### M1

Precision.

Potential configuration families:

* Conservative
* Balanced
* Responsive
* High Momentum

These are research configurations, not promises of superiority.

---

# 52. ROBUSTNESS

Future research should include:

* backtesting,
* forward testing,
* Monte Carlo,
* sensitivity analysis,
* parameter perturbation,
* regime analysis,
* walk-forward testing,
* and interaction analysis.

A parameter is not considered “better” merely because it produced the highest historical result.

The question is:

> **Does the behavior remain coherent when conditions change?**

---

# 53. TRON NARRATIVE ENGINE

The TRON narrative must always be derived from observable state.

Example structure:

**Macro regime → structural context → momentum → liquidity/trail → PSAR → execution context**

The narrative should explain relationships.

It should not fabricate certainty.

Bad:

> “TRON is 87% likely to win.”

Good:

> “H1 structure remains bearish while M15 momentum is recovering; M5 has not yet produced aligned execution context.”

---

# 54. OPERATOR PHILOSOPHY

The operator should learn to answer:

* What is the market doing?
* Where is price relative to structure?
* What is momentum doing?
* What is the broader regime?
* What session are we in?
* Is the lower timeframe aligned?
* What information is missing?
* Is there a contradiction?
* Is there enough context to make a decision?

TRON should help make those questions visible.

---

# 55. MARKETING CAMPAIGN

Initial campaign objective:

**Instagram / Facebook / WhatsApp Status → Lovable → WhatsApp → V1.1 evaluation → conversion**

The campaign should not lead with:

> “BUY THIS INDICATOR.”

It should lead with:

> **“See how TRON reads the market.”**

The website then converts curiosity into onboarding.

---

# 56. CAMPAIGN BUDGET

The current experimental idea is approximately:

* $10 advertising budget
* Lovable Pro approximately $25
* total initial spend approximately $35–$40

The objective is not to pretend this is a statistically meaningful acquisition campaign.

It is a small validation experiment.

The question is:

> Can a small amount of qualified traffic move through the funnel and produce at least one meaningful conversion?

---

# 57. CURRENT WEBSITE ANALYTICS

Observed period:

**2026-08-05 → 2026-09-04**

Approximate totals:

* Visitors: 36
* Pageviews: 60
* Pageviews / visit: 1.67
* Bounce: approximately 77
* Desktop: 23
* Mobile: 13

Traffic sources:

* Direct: 30
* Lovable: 4
* Facebook: 2

Countries:

* Kenya: 28
* China: 4
* Unknown: 2
* United States: 2

Conclusion:

The dataset is too small to make strong conversion conclusions.

Therefore:

> **Fix positioning and funnel clarity before drawing statistical conclusions from conversion data.**

---

# 58. THE IMPORTANT LESSON FROM THE WEBSITE ITERATION

The website can technically become “better” while commercially becoming worse.

A page can become:

* cleaner,
* more polished,
* more conversational,
* more explanatory,

and simultaneously lose the founder's authenticity.

Therefore:

> **Conversion optimization must not erase identity.**

The correct objective is:

# Authenticity + clarity + conversion

Not:

# Maximum marketing polish

---

# 59. LOVABLE PROJECT KNOWLEDGE

The Lovable project previously had effectively empty project knowledge.

That created a major risk:

> The AI could edit the website without understanding the product's actual source-of-truth hierarchy.

Persistent project knowledge has therefore been established around:

* V1.1 current/live
* V2 future
* no invented TRON features
* source hierarchy
* commercial architecture
* $49 lifetime anchor
* claims discipline
* design preservation
* WhatsApp onboarding
* Whop commercial access.

This knowledge should be maintained as the product evolves.

---

# 60. LOVABLE OPERATING RULE

From this point forward:

## NO BLIND EDITING.

The workflow should be:

1. Review the proposed change.
2. Discuss it.
3. Check it against the Master MD.
4. Decide whether it improves the product.
5. Only then send an implementation prompt to Lovable.

The product owner retains final control.

Lovable is an implementation tool, not the product strategist.

---

# 61. WEBSITE CHANGE CONTROL

Before changing the website, ask:

### Does this change improve:

* clarity?
* authenticity?
* trust?
* conversion?
* product accuracy?

If not, do not make it.

### Does it contradict:

* V1.1 source truth?
* V2 boundaries?
* commercial architecture?
* claims discipline?

If yes, do not make it.

### Does it require a new product decision?

If yes:

**pause and resolve the decision before implementation.**

---

# 62. WHOP STORE SPECIFICATION

Whop should eventually contain:

## 1. Hero

TRON Alpha V1.1 as the current live market-intelligence product.

## 2. What You Get

The actual entitlement/access included.

## 3. Who It Is For

Operators interested in structured market reading and decision support.

## 4. What V1.1 Includes

Only source-accurate features.

## 5. How Access Works

Purchase / entitlement → onboarding → TradingView V1.1 access/resources.

## 6. Price

Current anchor:

**$49 lifetime**

unless explicitly changed.

## 7. Founding 50

Separate grandfather/founding treatment.

## 8. V2

Future evolution.

Not included unless explicitly stated.

## 9. Expectations

No guaranteed results.

No fabricated performance.

TRON is decision support.

## 10. CTA

Obtain access through Whop.

---

# 63. WHOP URL

The actual Whop URL is currently an unresolved external decision.

### DO NOT INVENT IT.

Once the real Whop page exists, update:

* Hero secondary CTA if appropriate
* Pricing CTA
* Final CTA
* Footer
* relevant product/access links

---

# 64. CURRENT OPEN DECISIONS

The following must be explicitly resolved before hard-coding:

### 1. Exact seven-day evaluation mechanics

Confirmed conceptually, but public implementation should wait for final offer confirmation.

### 2. V1.1 post-evaluation price

Current working concept:

**$24.50**

but must be explicitly approved as the actual commercial offer.

### 3. Founding 50 mechanics

The $49 lifetime anchor is established conceptually, but exact grandfather rules require confirmation.

### 4. Whop URL

Pending actual Whop store.

### 5. V2 release

September 28, 2026 is:

**PROVISIONAL**

not guaranteed.

---

# 65. STALE LANGUAGE TO REMOVE

Unless deliberately reintroduced:

* “FREE BETA”
* “Free Forever”
* “No Trial”
* “No Countdown”
* “Prop Firm Ready”
* “execution calls”

These belong to previous positioning and should not survive accidentally.

---

# 66. LANGUAGE THAT SHOULD REMAIN

The product should retain strong authentic statements such as:

> **TRON is not a signal provider.**

and:

> **No signal is better than a bad signal.**

and:

> **TRON does not need to predict price. TRON needs to read price exceptionally well.**

These communicate the product philosophy better than generic SaaS language.

---

# 67. TRON'S DIFFERENTIATOR

The strongest differentiation is not:

> “We have BUY and SELL signals.”

The stronger proposition is:

> **The system exposes the market information behind its decision context.**

That includes:

* structure,
* momentum,
* liquidity,
* trend,
* sessions,
* PSAR,
* trail,
* MTF context,
* and position framing.

The BUY / SELL labels are useful because they make the output explicit.

But they should not become the entire identity of TRON.

---

# 68. PRODUCT POSITIONING

TRON should sit between:

### Raw chart reading

and:

### Black-box signals.

The proposition is:

> **Structured market intelligence.**

The operator gets more structure than manually scanning dozens of variables, while retaining visibility into what the engine is reading.

---

# 69. COMPETITOR / ECOSYSTEM RESEARCH

Relevant ecosystem references for future research include:

* LuxAlgo
* AlgoBot
* TradesAI

Research should examine:

* positioning,
* UI,
* feature hierarchy,
* onboarding,
* pricing,
* trust mechanisms,
* user expectations,
* and differentiation.

The purpose is not to copy competitors.

The purpose is to understand the category.

---

# 70. PRODUCT ROADMAP

## Phase 1 — V1.1 Freeze

Current.

Establish:

* source truth,
* parameters,
* UI,
* messaging,
* onboarding,
* evaluation.

## Phase 2 — V1 Commercial Access

Build:

* Whop,
* entitlement,
* access process,
* grandfathering.

## Phase 3 — Website

Lovable becomes the clean ADI front door.

## Phase 4 — V2

Controlled premium evolution.

## Phase 5 — Webhooks

Formalize TradingView alert contracts.

## Phase 6 — External TRON Intelligence

Structured market-intelligence delivery.

## Phase 7 — TRON Live

Operator interface/dashboard.

## Phase 8 — Auto-Trader

Deriv API / execution infrastructure where appropriate.

---

# 71. FUTURE TRON LIVE

Long-term concept:

A TRON operator dashboard containing:

* live signal/event feed,
* confidence/context information where appropriately defined,
* win/loss tracking where objectively measured,
* historical reads,
* session state,
* market context,
* operator journal,
* and eventually automation.

The dashboard should not become a black-box “copy my trades” product.

---

# 72. AUTO-TRADER

Long-term:

**TRON Auto-Trader**

Potentially through:

**Deriv API**

This is future infrastructure.

It must remain clearly separated from the current V1.1 product.

---

# 73. SAFETY / RESPONSIBLE POSITIONING

Trading is financially risky.

ADI/TRON marketing should not encourage reckless behavior.

Avoid:

* “easy money”
* “guaranteed income”
* “never lose”
* “high win rate”
* “quit your job”
* “guaranteed funding”
* “guaranteed prop success”
* or similar claims.

TRON is an educational and decision-support framework.

The operator remains responsible for:

* decisions,
* risk,
* execution,
* and capital.

---

# 74. EMANUEL / FOUNDER CONCERNS

The following concerns are important because they describe the product owner's actual intent and should inform future decisions.

### Concern 1 — Authenticity

> “The page feels conversational like... It lost it's authenticity I had done but no worries. I'll work it out”

Interpretation:

The website must not become so AI-polished that the founder's original voice disappears.

---

### Concern 2 — Ownership

> “A reply is better than editing..I realize giving you access was not very wise but we learn.”

This establishes the new workflow:

**Review first. Edit second.**

The assistant should provide critique and recommendations before making external changes.

---

### Concern 3 — Lovable should not own the product direction

Lovable can implement.

It should not independently redefine:

* product positioning,
* TRON capabilities,
* commercial structure,
* founder voice,
* or roadmap.

---

### Concern 4 — Commercial funnel

The intended idea is:

> “Instagram boost / Facebook / WhatsApp Status → Lovable → WhatsApp → activation/evaluation”

The website therefore has to function as the **front door**, not as the entire business.

---

### Concern 5 — Whop

The product architecture is:

> **“Lovable = ADI front door; Whop = commercial/access door.”**

This distinction should remain foundational.

---

### Concern 6 — V1.1 versus V2

V1.1 is the current product.

V2 is the future premium evolution.

The site must create anticipation without pretending V2 already exists.

---

### Concern 7 — Seven-day evaluation

The planned commercial journey is:

> seven-day free V1.1 evaluation

followed by an upsell toward full V1.1 access.

The exact mechanics must be finalized before hard-coding.

---

### Concern 8 — Grandfather pricing

The current commercial thinking is:

> after the 7 days free trial we upsell full access untill release of V2 for grandfather pricing 50% off right at 24.5

This is a working commercial concept, not yet a permanent pricing rule.

---

### Concern 9 — Broker / affiliate path

The founder has considered an affiliate path involving Deriv, particularly around:

* Gold,
* Synthetic Indices,
* and execution infrastructure.

This should be treated as an ecosystem/affiliate decision, not allowed to distort the core TRON product.

---

### Concern 10 — Asset agnosticism

The founder's intended positioning is that TRON is not tied to one market.

The framework can potentially span:

* Gold,
* Forex,
* Synthetic Indices,
* Crypto,
* Bybit,
* and other compatible environments.

The website should therefore emphasize the **framework**, not one broker.

---

# 75. IMPORTANT FOUNDER WORKFLOW OBSERVATION

The founder's actual product-development philosophy has been iterative:

* build,
* test,
* observe,
* receive operator feedback,
* refine,
* compare,
* and repeat.

The website should communicate this.

That is much stronger than pretending TRON emerged fully formed.

---

# 76. “BEYOND BETA”

The current V1.1 positioning should communicate:

> **Beyond beta.**

But this does not mean:

> “Perfect.”

It means:

* refined,
* tested,
* iterated,
* informed by operator feedback,
* and now entering a more mature product phase.

---

# 77. DESIGN RULE

When editing the website:

### Preserve first.

Then:

### Clarify.

Then:

### Improve conversion.

Only then:

### Add.

Do not:

### Redesign because redesign is possible.

---

# 78. COPY RULE

The best copy should be:

* direct,
* confident,
* technically grounded,
* human,
* occasionally opinionated,
* concise,
* and authentic.

Avoid:

* excessive SaaS jargon,
* fake urgency,
* excessive emojis,
* generic “revolutionary AI” language,
* over-explanation,
* and corporate filler.

---

# 79. THE PRODUCT SHOULD FEEL LIKE A BUILDER'S WORK

The visitor should feel:

> “Someone actually built this because they wanted to solve a real problem in how they read the market.”

Not:

> “Someone assembled another trading indicator landing page.”

This is a critical brand distinction.

---

# 80. FUTURE CONTENT

Potential educational content:

* Multipliers explained
* TRON workflow
* H1/M15/M5 framework
* Reading market structure
* Understanding liquidity
* Understanding PSAR
* Understanding the Liquidity Trail
* Why explicit BUY/SELL labels exist
* Alpha Gate
* Killzones
* Synthetic indices
* Gold
* Crypto
* TradingView workflow

Educational content should teach the framework rather than simply push the product.

---

# 81. COMMUNITY CONTENT STANDARD

Canonical public intelligence:

**H1 → M15 → M5 → TRON Synthesis → Operator Watch**

Every market read should distinguish:

* observation,
* interpretation,
* and operator decision.

Never fabricate certainty.

---

# 82. TRON DICTIONARY

Future development should maintain a centralized dictionary defining:

* every TRON component,
* every state,
* every signal,
* every dashboard label,
* every parameter,
* every alert,
* and every narrative rule.

This reduces semantic drift between:

* Pine,
* website,
* community,
* Whop,
* documentation,
* and future software.

---

# 83. VERSION CONTROL

Every product version must have:

* version number,
* release state,
* source truth,
* feature inventory,
* parameter inventory,
* UI terminology,
* alert inventory,
* commercial status.

### V1.1

**CURRENT / LIVE**

### V2

**FUTURE / PROVISIONAL**

---

# 84. UPDATE LOG

## 2026-09-04 — Master MD established

The existing August 24 Lovable plan was promoted into the evolving Master MD rather than creating another competing document.

Established:

* V1.1 as current live product
* V2 as future product
* source hierarchy
* commercial architecture
* Lovable front door
* WhatsApp onboarding/community
* TradingView V1.1 delivery
* Whop commercial/access
* $49 lifetime anchor
* claims discipline
* V2 provisional September 28 target
* Founding 50 concept
* website change-control principles.

---

## 2026-09-04 — V1.1 Website Positioning

The website is being moved away from stale:

* Free Forever
* FREE BETA
* No Trial
* Prop Firm Ready

positioning.

Current emphasis:

* V1.1
* explicit BUY/SELL labels
* H1 → M15 → M5 workflow
* operator-informed Alpha Gate recommendation
* Beyond beta
* WhatsApp onboarding
* TradingView product experience
* future Whop access.

---

## 2026-09-04 — “What's New in V1.1”

Dedicated V1.1 update section established after TRON in action and before The Tape.

Core messages:

* explicit BUY / SELL labels,
* H1 → M15 → M5,
* M1 Alpha Gate operator recommendation,
* real operator feedback,
* beyond beta.

---

## 2026-09-04 — V2 Countdown

V2 provisional target established:

**September 28, 2026**

Founding 50 pricing concept:

**$49 lifetime**

V2 remains:

**not live / not included in V1.1.**

---

## 2026-08-24 — Historical Website Conversion Plan

Original objective:

> Convert the page into a channel-join machine.

The original plan emphasized:

* clear joining,
* Telegram,
* WhatsApp,
* sticky mobile CTA,
* channel selection,
* simplified conversion.

This remains useful historical context but has been superseded by the newer architecture:

**Lovable → WhatsApp → TradingView V1.1 → Whop**

The historical plan should not be deleted because it documents how the funnel evolved.

---

# 85. CURRENT MASTER FUNNEL

The current intended model is:

```text
SOCIAL TRAFFIC
Instagram
Facebook
WhatsApp Status
        ↓
ADI / LOVABLE
Education
Trust
TRON demonstration
Product explanation
        ↓
WHATSAPP
Onboarding
Questions
Community
Evaluation
        ↓
TRADINGVIEW
TRON Alpha V1.1
        ↓
WHOP
Commercial access
Entitlement
Lifetime purchase
        ↓
V2
Future premium evolution
        ↓
TRON LIVE
Future operator platform
```

---

# 86. FINAL PRODUCT PRINCIPLE

The entire ecosystem should ultimately reinforce one idea:

> **TRON is not here to replace the operator.**

It exists to make the market easier to read.

The product should therefore continually move the user through:

# Learn.

# Understand.

# Observe.

# Execute.

And the deeper principle remains:

# TRON DOES NOT NEED TO PREDICT PRICE.

# TRON NEEDS TO READ PRICE EXCEPTIONALLY WELL.

---

# 87. MASTER DECISION RULE

Whenever a future idea is proposed, ask:

### Does it make TRON better at reading price?

### Does it make the operator understand TRON better?

### Does it preserve transparency?

### Does it preserve the founder's authenticity?

### Is it supported by source truth?

### Is it actually current, or is it V2?

### Does it improve the user journey without turning the product into generic marketing?

If the answer is unclear:

**do not implement yet.**

Discuss first.

---

# 88. CURRENT STATE

As of **September 4, 2026**:

**TRON Alpha V1.1 is the current product.**

**V2 is future.**

**Lovable is the ADI front door.**

**WhatsApp is the onboarding/community door.**

**TradingView is the V1.1 product environment.**

**Whop is the commercial/access door.**

**$49 lifetime is the current standard pricing anchor.**

**September 28, 2026 is a provisional V2 release target.**

**The seven-day evaluation is a planned onboarding/commercial mechanism requiring final offer confirmation before being hard-coded everywhere.**

**The founder's voice and authenticity are non-negotiable.**

And from this point forward:

> **Reply first. Edit second.**

No external implementation should happen merely because an AI thinks an edit is “better.”

The product owner decides.

The MD remembers.

The tools implement.
