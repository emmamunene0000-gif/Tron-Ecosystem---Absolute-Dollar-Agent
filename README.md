# Tron-Ecosystem---Absolute-Dollar-Agent
Absolute Dollar Intelligence (ADI) / TRON — GitHub Internal AI Handover

Document status: Working handover / source-of-truth context
Date: 2026-09-03
Purpose: Give GitHub Internal AI the complete project context needed to continue ADI/TRON work without redesigning, reinterpreting, or drifting from the existing system.

0. NON-NEGOTIABLE OPERATING RULE

This project must be treated as an existing system being externalized and evolved, not as a blank-slate product.

Do not:

redesign TRON from scratch;

rewrite TRON logic merely to make it easier to implement elsewhere;

invent signals, states, probabilities, market narratives, or capabilities;

replace the source-of-truth Pine implementation with generic AI reasoning;

turn TRON into a conventional prediction engine;

make the existing V1/V1.1 product look obsolete;

introduce generic trading-indicator language where the actual TRON vocabulary is available.

When the actual TRON V1 Pine source is uploaded, treat that source as authoritative for technical behavior. Where this handover and the source disagree, inspect the source and preserve the actual implementation.

The user's previously supplied TRON dictionary, Telegram templates, product architecture, and customer-journey decisions are also canonical context.

1. WHAT TRON IS

TRON is a deterministic market-reading and decision-support engine.

It is not fundamentally a signal-selling service and it is not intended to predict price.

The governing philosophy is:

TRON DOES NOT NEED TO PREDICT PRICE. TRON NEEDS TO READ PRICE EXCEPTIONALLY WELL.

ADI motto:

LEARN. UNDERSTAND. OBSERVE. EXECUTE.

Core philosophy:

Analysis → Capital → Execution

TRON is built around a live Pine Script indicator on TradingView. The Pine Script itself executes the defined TRON logic.

The future "TRON AI" is therefore not a replacement for TRON.

It is an Augmented Intelligence layer around the live deterministic TRON engine.

2. TRON AI — CORRECT CONCEPT

The intended future system is:

LIVE MARKET
    ↓
TRADINGVIEW
    ↓
LIVE TRON PINE SCRIPT
    ↓
TRON DETERMINISTIC LOGIC
    ↓
TRON EVENTS / STATES
    ↓
TRON AI — AUGMENTED INTELLIGENCE
    ↓
ANALYSIS / OPPORTUNITY MONITORING / STATE UPDATES
    ↓
LOVABLE TRON INTERFACE
    ↓
TELEGRAM / OTHER OUTPUT SURFACES

The AI must operate from actual TRON observations.

It can:

observe TRON state;

compare current state with previous state;

maintain evolving context;

prepare analysis;

monitor developing opportunities;

identify state transitions;

prepare concise explanations;

update analysis as price develops;

produce externalized TRON communications.

It must not:

invent market conditions;

fabricate confirmations;

override the deterministic TRON state;

convert uncertainty into certainty;

manufacture a signal simply because an AI model thinks a market move is likely.

TRON observations are the ground truth.

3. TRON SOURCE ARCHITECTURE

The current TRON implementation is understood as four merged systems:

ICT Killzones / Pivots

Absolute Dollar Agent

Smart PSAR

Unified Dashboard

Core components exposed by the live system include:

Market Structure

RSI Momentum

EMA Regime

Liquidity Trail

Smart PSAR

Killzones

Position Tool

Dashboard

The actual dashboard vocabulary is important and should be preserved.

4. CANONICAL TRON VOCABULARY

RSI Momentum

Dashboard states:

Bullish 🟢

Bearish 🔴

Neutral ⚪

Underlying configuration previously identified:

RSI length: 10

Bullish threshold: 55

Bearish threshold: 48

Overbought exhaustion: 85

Oversold exhaustion: 20

Important implementation detail:

The bullish/bearish state is not simply "RSI above/below one line."

The bullish condition involves the configured threshold, non-exhaustion condition, RSI EMA direction, and related logic.

The bearish condition similarly includes its own conditions.

External language should preserve the state rather than simplify it into generic RSI advice.

Smart Signal

Dashboard states:

Smart Bull 🟢

Smart Bear 🔴

No Signal ⚪

Smart Signal is an event, not simply the current bias.

The source logic uses new-event detection:

newSmartBull = smartBull AND NOT smartBull[1]

newSmartBear = smartBear AND NOT smartBear[1]

When enabled, M5 confirmation is also involved.

Therefore:

Smart Signal ≠ overall TRON directional state.

A current bearish state can exist while Smart Signal says No Signal.

Market Structure / MS Bias

Dashboard:

Bullish

Bearish

Neutral

Structural vocabulary:

HH = Higher High

HL = Higher Low

LH = Lower High

LL = Lower Low

BOS = Break of Structure

CHoCH = structural break against the previous breakout direction

MS Bias is based on the stored breakout direction in the implementation.

Momentum Trend

Dashboard label:

Momentum Trend

Internally this was identified as the former "Trend Truth" concept.

Three components contribute:

M5 smoothed RSI

5-bar price momentum

EMA 21/55 direction

Each contributes +1, 0, or -1.

Thresholds:

score >= +2 → Bullish 📈

score <= -2 → Bearish 📉

otherwise → Neutral ⚖️

Do not replace this with vague language such as "overall market health."

EMA Cross

TRON uses:

EMA 21

EMA 55

Dashboard:

Bullish when EMA21 > EMA55

Bearish otherwise

External wording:

🟢 EMA Cross Bullish
🔴 EMA Cross Bearish

Liquidity Trail

The Liquidity Trail is not merely a generic trailing stop.

Previously identified defaults:

MA length: 13

ATR length: 14

ATR multiplier: 2.0

Conceptually:

Trail MA = EMA(close, MA length)

Bull trail = MA - ATR × multiplier

Bear trail = MA + ATR × multiplier

The system maintains directional state and can generate Trail Buy / Trail Sell events.

Dashboard:

Bullish 🔺 + level

Bearish 🔻 + level

Canonical external language:

🟢 Liquidity Trail Bullish @ [LEVEL]
🔴 Liquidity Trail Bearish @ [LEVEL]

Primary meaning:

current structural/directional Liquidity Trail state + reference level.

Do not reduce it merely to "support/resistance."

Smart PSAR

Dashboard can show:

▲ BULLISH

▼ BEARISH

▲ BULL (Opposing)

▼ BEAR (Opposing)

Direction is based on price relative to PSAR.

The "Opposing" state is important TRON vocabulary and must remain.

Canonical external language:

🟢 Smart PSAR = Bullish
🔴 Smart PSAR = Bearish
⚠️ Bull (Opposing)
⚠️ Bear (Opposing)

PSAR MTF Context

The source compares current PSAR direction with the PSAR direction from the configured higher timeframe.

Default previously identified:

psar_htf = 5

Dashboard:

● ALIGNED (5)

○ DIVERGED (5)

Important correction to earlier generic documentation:

Do NOT say:

"Higher timeframe agrees with this bias."

The technically accurate language is:

PSAR MTF ALIGNED = current PSAR direction agrees with the configured PSAR MTF timeframe.

PSAR MTF DIVERGED = current PSAR direction differs from the configured PSAR MTF timeframe.

PSAR Momentum

The dashboard displays a visual bar such as:

████████░░

The value is derived from PSAR distance relative to ATR.

Do not invent textual strength classifications unless the source explicitly provides them.

Position Tool

Dashboard states:

LONG

SHORT

No active position

The Position Tool is downstream of configured execution gates.

Previously identified gating concept:

Signal Change OR Trail Retest

PSAR direction clears

RSI momentum clears

Therefore:

Position Tool state ≠ Smart Signal.

This distinction is essential.

Entry / SL / TP

Previously identified source behavior:

Entry = close

SL = Liquidity Trail

Risk = absolute distance between Entry and SL

Default targets:

TP1 = 1R

TP2 = 1.5R

TP3 = 2R

Externalized display:

POSITION MODEL

Entry: [PRICE]
SL:    [PRICE]

TP1: [PRICE] — 1R
TP2: [PRICE] — 1.5R
TP3: [PRICE] — 2R

These values must be verified against the uploaded V1 source before treating them as immutable.

5. TEMPORAL / SESSION CONTEXT

TRON uses EAT / GMT+3 session mapping.

Previously identified sessions:

Asia: 03:00–07:00

London Open: 07:00–11:00

London Mid: 11:00–15:00

London–New York Overlap: 15:00–19:00

New York PM: 19:00–23:00

Source vocabulary includes:

Asia (H4-1)

LDN Open (H4-2)

LDN Mid (H4-3)

LDN-NY Overlap (H4-4)

NY PM (H4-5)

H4-6 (Dead Zone)

TRON also exposes:

H4 Previous Close

H4 Current Open

H4 Current High

H4 Current Low

H1 Previous Close

Active H4 Session

Active KZ Range

6. IMPORTANT MULTI-TIMEFRAME FACT

The TRON dashboard does not internally contain four independent H1/M15/M5 dashboards.

The dashboard is populated from the current chart timeframe while the source separately pulls M5 RSI/EMA and H4/H1 session context.

Therefore, when the externalized operating model uses:

H1 = macro

M15 = structural

M5 = execution

M1 = precision

that is an external operating methodology built around running/reading TRON across those chart timeframes, not a claim that the dashboard itself contains four independent timeframe engines.

Do not misrepresent this.

7. RECOMMENDED OPERATING TIMEFRAME MODEL

The current user experience points toward:

H1 — Intraday / Macro Analysis

Use H1 to establish the broader intraday environment.

M15 — Tactical / Structural Analysis

Use M15 to understand structural development and tactical context.

M5 — Recommended Execution Timeframe

M5 is the recommended tactical execution timeframe.

M1 — Precision / Optional Execution

M1 may be used for precision, but the user specifically wants to recommend the Alpha Gate when executing on M1, based on accumulated user experience.

This should be presented as an operator recommendation, not as a newly invented technical rule.

The landing page / documentation should communicate:

Recommended workflow: H1 for intraday context → M15 for tactical structure → M5 for execution.

And:

If executing on M1, use the Alpha Gate.

The Alpha Gate wording and actual behavior must be verified against the uploaded V1 source before changing technical documentation.

8. CANONICAL TELEGRAM / MARKET-INTELLIGENCE STRUCTURE

The user's Telegram templates are not generic marketing templates.

They represent how the user personally analyzes the market using TRON.

The externalized SOP should preserve this structure.

H1 MACRO REGIME

📊 TRON ALPHA — H1 MACRO REGIME

💰 XAUUSD: [PRICE]
🕐 [TIME] EAT
⏰ [ACTIVE H4 SESSION]

━━━━━━━━━━━━━━
🌍 MACRO STATE
━━━━━━━━━━━━━━

📈 EMA Cross: [STATE]

🌊 Liquidity Trail:
[STATE] @ [LEVEL]

📊 RSI Momentum:
[STATE] ([VALUE])

🏛 MS Bias:
[STATE]

🧠 Momentum Trend:
[STATE]

━━━━━━━━━━━━━━
📍 H4 / H1 LOCATION
━━━━━━━━━━━━━━

H4 Prev Close: [VALUE]
H4 Open: [VALUE]
H4 High: [VALUE]
H4 Low: [VALUE]
H1 Prev Close: [VALUE]

KZ Range: [VALUE]

━━━━━━━━━━━━━━
🧠 TRON NARRATIVE
━━━━━━━━━━━━━━

[Compressed narrative derived ONLY from actual states.]

🎯 TRON STATE:
[BEARISH TREND / BEARISH PULLBACK / TRANSITION / NEUTRAL]

M15 STRUCTURAL TREND

📈 TRON ALPHA — M15 STRUCTURAL

💰 Price: [PRICE]
⏰ Session: [SESSION]

━━━━━━━━━━━━━━
🏛 STRUCTURE
━━━━━━━━━━━━━━

MS Bias:
[STATE]

Structure:
[HH / HL / LH / LL]

Break:
[BOS / CHoCH / NONE]

━━━━━━━━━━━━━━
🌊 TREND
━━━━━━━━━━━━━━

EMA:
[STATE]

Liquidity Trail:
[STATE] @ [LEVEL]

Momentum Trend:
[STATE]

━━━━━━━━━━━━━━
🛰 PSAR
━━━━━━━━━━━━━━

Smart PSAR:
[STATE]

PSAR Momentum:
[BAR]

PSAR MTF:
[ALIGNED / DIVERGED] ([TF])

━━━━━━━━━━━━━━
🧠 TRON NARRATIVE
━━━━━━━━━━━━━━

[Derived from actual H1/M15 relationship.]

M5 EXECUTION ENGINE

⚡ TRON ALPHA — M5 EXECUTION

💰 XAUUSD: [PRICE]
🕐 [TIME] EAT

━━━━━━━━━━━━━━
📊 MOMENTUM
━━━━━━━━━━━━━━

RSI Momentum:
[STATE] ([VALUE])

Smart Signal:
[STATE]

Momentum Trend:
[STATE]

━━━━━━━━━━━━━━
🏛 STRUCTURE
━━━━━━━━━━━━━━

MS Bias:
[STATE]

BOS / CHoCH:
[VALUE]

━━━━━━━━━━━━━━
🌊 TRAIL + EMA
━━━━━━━━━━━━━━

EMA Cross:
[STATE]

Liquidity Trail:
[STATE] @ [LEVEL]

━━━━━━━━━━━━━━
🛰 SMART PSAR
━━━━━━━━━━━━━━

PSAR:
[STATE]

PSAR Momentum:
[BAR]

MTF Context:
[STATE] ([TF])

━━━━━━━━━━━━━━
🎯 POSITION TOOL
━━━━━━━━━━━━━━

Position:
[LONG / SHORT / NONE]

Entry:
[VALUE]

SL:
[VALUE]

TP1:
[VALUE] — 1R

TP2:
[VALUE] — 1.5R

TP3:
[VALUE] — 2R

━━━━━━━━━━━━━━
🧠 TRON EXECUTION NARRATIVE
━━━━━━━━━━━━━━

[Actual TRON state.]

⚠️ Smart Signal and Position Tool are separate states.

9. FULL PUBLIC CHANNEL TEMPLATE

🚀 TRON ALPHA — XAUUSD MARKET INTELLIGENCE

📅 [DATE]
🕐 [TIME] EAT
💰 Price: [PRICE]
⏰ Active H4 Session: [SESSION]

━━━━━━━━━━━━━━━━
🌍 H1 — MACRO REGIME
━━━━━━━━━━━━━━━━

📈 EMA: [STATE]
🌊 Trail: [STATE] @ [LEVEL]
📊 RSI: [STATE] [VALUE]
🏛 MS Bias: [STATE]
🧠 Momentum: [STATE]

📍 H4 Prev Close: [VALUE]
📍 H4 Open: [VALUE]
📍 H4 High: [VALUE]
📍 H4 Low: [VALUE]
📍 H1 Prev Close: [VALUE]
📏 KZ Range: [VALUE]

🧠 H1 INTELLIGENCE:
[1–2 sentence TRON narrative]

━━━━━━━━━━━━━━━━
📐 M15 — STRUCTURAL TREND
━━━━━━━━━━━━━━━━

🏛 MS Bias: [VALUE]
📐 Structure: [HH/HL/LH/LL]
⚡ Break: [BOS/CHoCH/NONE]

📈 EMA: [VALUE]
🌊 Trail: [VALUE]
🧠 Momentum: [VALUE]

🛰 PSAR: [VALUE]
🔗 MTF: [STATE]

🧠 M15 INTELLIGENCE:
[1–2 sentence narrative]

━━━━━━━━━━━━━━━━
⚡ M5 — EXECUTION ENGINE
━━━━━━━━━━━━━━━━

📊 RSI: [VALUE] [STATE]
🎯 Smart Signal: [STATE]

🏛 MS Bias: [STATE]
📈 EMA: [STATE]
🌊 Trail: [STATE] @ [LEVEL]

🛰 PSAR: [STATE]
📶 PSAR Momentum: [BAR]
🔗 MTF: [STATE]

🎯 Position: [LONG/SHORT/NONE]
Entry: [VALUE]
SL: [VALUE]
TP1: [VALUE]
TP2: [VALUE]
TP3: [VALUE]

🧠 M5 INTELLIGENCE:
[1–2 sentence execution narrative]

━━━━━━━━━━━━━━━━
🧩 TRON SYNTHESIS
━━━━━━━━━━━━━━━━

🌍 MACRO:
[STATE]

📐 STRUCTURE:
[STATE]

⚡ EXECUTION:
[STATE]

🔗 INTERNAL ALIGNMENT:
[ALIGNED / MIXED / TRANSITION]

🧠 TRON READ:
[ONE compressed statement derived ONLY from displayed states]

━━━━━━━━━━━━━━━━
🎯 OPERATOR WATCH
━━━━━━━━━━━━━━━━

👁 [KEY TRON STATE]
👁 [KEY TRON LEVEL]
👁 [KEY TRANSITION]

TRON provides market intelligence.
The operator remains responsible for the final decision and execution.

10. NARRATIVE ENGINE — DO NOT MAKE THIS ARBITRARY

Narrative generation must be deterministic and traceable to displayed states.

Example: full bearish internal agreement

Inputs:

EMA = Bearish

Trail = Bearish

MS Bias = Bearish

Momentum Trend = Bearish

PSAR = Bearish

PSAR MTF = Aligned

Output concept:

🔴 BEARISH INTERNAL ALIGNMENT — EMA regime, Liquidity Trail, Market Structure and Momentum Trend are bearish. Smart PSAR is bearish and MTF-aligned. The current TRON state is internally synchronized to the downside.

Example: bearish H1 / bullish M15

Inputs:

H1 = Bearish

M15 = Bullish

Output concept:

⚠️ COUNTERTREND STATE — the M15 directional state is opposing the higher-timeframe bearish environment. TRON is showing lower-timeframe strength inside a conflicting macro state.

Example: bearish state but no Smart Signal

Inputs:

Trail = Bearish

MS = Bearish

Momentum = Bearish

Smart Signal = No Signal

Output concept:

🔴 ESTABLISHED BEARISH STATE — NO NEW SMART EVENT. Current bearish conditions remain active, but TRON is not generating a new Smart Bear event on this bar.

The important rule:

The narrative describes observed state relationships. It does not invent reasons beyond the available TRON data.

11. PRODUCT STATUS — V1 / V1.1

The product is no longer to be presented as an August beta.

August 2026 was the beta period.

As of September 2026, the public positioning should reflect that TRON has moved beyond beta.

The current live product is:

TRON Alpha V1.1

The V1.1 update should be presented as a real product update based on user feedback and observed operator experience.

Do not keep stale language such as:

"entering beta"

"coming soon"

"beta testing"

"wait for V2"

"not ready"

unless referring historically to the August beta period.

12. V1.1 UPDATE LOG FOR THE LOVABLE LANDING PAGE

The next Lovable update should add an explicit TRON ALPHA V1.1 UPDATE LOG section or equivalent without redesigning the site.

The purpose is to communicate:

TRON has been upgraded based on user feedback.

The key focus:

Explicit BUY / SELL signal labels

V1.1 introduces explicit BUY / SELL entry labels.

These labels are gated by the same underlying TRON logic rather than being arbitrary arrows.

The landing page should explain this accurately from the uploaded source.

M1 Alpha Gate recommendation

Based on user experience:

If executing on M1, use the Alpha Gate.

This is an operator recommendation and should be clearly distinguished from the underlying technical implementation.

Recommended timeframe workflow

H1 → Intraday analysis / macro context
M15 → Tactical / structural analysis
M5 → Recommended execution timeframe
M1 → Precision execution; Alpha Gate recommended

The page should make M5 the recommended execution timeframe while explaining M1 as an optional precision layer.

13. FUTURE PREMIUM PRODUCT

The next major product is:

Absolute Dollar Agent — TRON V2

This is the premium evolution of the TRON ecosystem.

Important:

V2 should not make V1.1 look useless.

V1.1 is the current live foundation and real-world operating laboratory.

V2 is the next product layer.

The user wants a launch countdown on the Lovable landing page.

Current planning date:

2026-09-03

A 25-day countdown from this date points to approximately:

2026-09-28

This launch date should be treated as a planned/provisional date until explicitly locked.

14. V2 POSITIONING

The intended message is:

TRON Alpha V1.1 is the current live foundation.

TRON V2 is the upcoming premium evolution.

The user wants operators who have demonstrated:

consistency;

discipline;

understanding of TRON;

meaningful engagement with the framework;

to be eligible for future updates / grandfathered access under the launch offer.

Do not frame this as a subscription-first model.

15. GRANDFATHER PRICING CONCEPT

After the relevant free access period, the intended grandfather offer is:

$49 lifetime access

Not monthly subscription.

The intended concept is:

After the trial/evaluation period, eligible operators can lock in grandfather pricing for the quarter at $49 lifetime access to TRON V2.

The exact entitlement wording should be finalized before publishing, but the important commercial decision is:

$49 = lifetime, not monthly.

The offer is intended to reward early operators who actually use and understand TRON.

16. CURRENT CUSTOMER JOURNEY

The customer journey is evolving toward:

DISCOVERY
   ↓
LOVABLE / ADI LANDING PAGE
   ↓
COMMUNITY
   ↓
TRON ALPHA V1.1
   ↓
FREE ACCESS / EVALUATION PERIOD
   ↓
LEARN
   ↓
UNDERSTAND
   ↓
OBSERVE
   ↓
PRACTICE / REVIEW
   ↓
DEMONSTRATE CONSISTENCY + DISCIPLINE
   ↓
GRANDFATHER OFFER
   ↓
$49 LIFETIME TRON V2
   ↓
TRON V2 PREMIUM
   ↓
FUTURE TRON INTELLIGENCE ECOSYSTEM

The previous public site had temporarily been changed to "Alpha free forever."

That is now superseded by the user's latest product decision for this next phase:

V1.1 is no longer positioned as an August beta; the access/evaluation period and V2 grandfathering are now the intended commercial transition.

Before changing the live page, reconcile all old "free forever" copy with the latest offer decision.

Do not leave contradictory offers on the page.

17. LOVABLE'S ROLE

The existing Lovable project is:

Absolute Dollar Intelligence Landing

Project ID:

0bfdc3ca-85e2-41e7-a3dc-9220eec805cc

Current project characteristics:

premium dark fintech visual system;

Apple / Linear / Stripe / Vercel / Raycast-inspired;

subtle cyber/TRON feel;

existing reusable components;

public landing page;

no need for a complete redesign.

The explicit instruction is:

Preserve the current visual system and components. Upgrade the interface and customer journey rather than rebuilding the site.

The landing page should eventually become the front door to the wider TRON ecosystem.

18. CURRENT LOVABLE PAGE STRUCTURE

The current page has included:

ADI header/navigation

Hero

TRON explanation

Three Pillars

TRON in Action

Tape / Broadcast Archive

Channel selection

Operator's Journey

Access Model / Pricing

Difference / philosophy

FAQ

Final CTA

Footer

Mobile sticky join

Previous project work removed stale public Execution War Room links and created a public-channel journey.

Previous work also changed old trial/beta language toward "Alpha free forever."

That work now needs to be reconciled with the latest September V1.1 → V2 commercial plan.

19. LOVABLE PROJECT MUST BE INSPECTED BEFORE MODIFICATION

Before making another significant edit:

Inspect current files.

Inspect current project knowledge.

Inspect recent Lovable messages/edits.

Read the actual components being changed.

Compare current page copy against this handover.

Only then implement.

Do not assume the live page equals the latest intended architecture.

The project has undergone several iterations.

20. EXISTING LOVABLE HISTORY THAT MATTERS

Important previous work:

August

The landing page was being optimized for:

Telegram

WhatsApp group

WhatsApp channel

community conversion

removing the public Execution War Room link

The Execution War Room is intended to remain private.

It should be presented as a private TRON-access destination, not a public cold-traffic link.

September 2

The Lovable project was updated toward:

TRON Alpha — FREE BETA

Free Forever

no trial

Premium as the upgrade

five-step operator journey

This update was based on an earlier product decision.

This is now superseded where it conflicts with the latest September 3 V1.1 → V2 transition plan.

Do not blindly preserve contradictory copy.

21. COMMERCIAL ARCHITECTURE

The intended ecosystem roles are:

TRON / TradingView

Actual deterministic market-reading engine.

Lovable

Front door + education + TRON interface + future operator dashboard.

Telegram

Broadcast intelligence / market-information channel.

WhatsApp

Community, onboarding, support, direct engagement.

Whop

Commercial/access layer for the premium product.

Whop is being considered as the preferred checkout/access layer rather than building a full commerce system into Lovable.

Do not turn Lovable into a checkout platform unnecessarily.

22. FUTURE TRON WEB / LIVE ARCHITECTURE

The long-term technical direction is:

TRADINGVIEW
     ↓
TRON PINE SCRIPT
     ↓
TRADINGVIEW ALERT / WEBHOOK
     ↓
TRON EVENT INGESTION
     ↓
TRON STATE / EVENT NORMALIZATION
     ↓
TRON AUGMENTED INTELLIGENCE
     ↓
┌───────────────┬────────────────┬────────────────┐
│               │                │                │
TRON LIVE      TELEGRAM         ARCHIVE          OTHER UI
│
LOVABLE

The critical architecture principle:

Do not duplicate the TRON brain unless there is a demonstrated technical reason to do so.

Initially, TradingView/Pine remains the source of deterministic TRON state.

The external layer receives those observations and externalizes them.

23. WEBHOOK CONCEPT

A live TradingView alert should eventually be able to feed the external TRON layer.

Conceptually:

TRON Pine Script
      ↓
TradingView Alert
      ↓
Webhook endpoint
      ↓
TRON event parser
      ↓
State/event object
      ↓
Narrative/state engine
      ↓
Lovable TRON Live
      ↓
Telegram / archive

The first proof-of-concept should be deliberately small:

Can a live TRON alert leave TradingView, arrive at the backend, preserve the exact TRON state, and produce a faithful externalized TRON update?

Do not start by building a complete autonomous trading platform.

24. TRON AI'S EVENT MODEL

A useful conceptual event object is:

timestamp
symbol
timeframe
session
event_type
rsi_state
rsi_value
smart_signal
ms_bias
structure_state
break_state
ema_state
liquidity_trail_state
liquidity_trail_level
psar_state
psar_mtf_state
psar_momentum
position_state
entry
sl
tp1
tp2
tp3

The exact payload must ultimately be based on what the Pine alert can actually provide.

Do not invent fields that the source cannot supply.

25. OPPORTUNITY MONITORING

The future intelligence layer should understand that a market opportunity is not necessarily a single alert.

Price develops through states.

Therefore TRON AI should eventually maintain a timeline such as:

STATE A
↓
STATE CHANGE
↓
NEW TRON EVENT
↓
CONTEXT UPDATE
↓
STRUCTURAL DEVELOPMENT
↓
EXECUTION-STATE DEVELOPMENT
↓
CONFIRMATION / FAILURE / TRANSITION

This lets the system communicate:

what TRON saw;

what changed;

what remains unchanged;

what is developing;

what transition matters next.

It should not invent a trade because a model "feels" one is coming.

26. EXAMPLE OF AUGMENTED INTELLIGENCE

Suppose:

H1 = Bearish
M15 = Bearish
M5 = Bullish

TRON AI can identify:

Countertrend lower-timeframe development inside a bearish higher-timeframe environment.

If later:

M15 = CHoCH
M5 = Bullish
PSAR = Bullish
PSAR MTF = Aligned

the intelligence layer can update the existing analysis:

The lower-timeframe transition has developed into a structural change on M15 while PSAR remains aligned.

The system is tracking market development, not generating a prediction.

27. THE "TRON TAPE"

The existing landing page contains a broadcast archive / tape concept.

This should eventually become more powerful.

Every externalized TRON event can become part of a chronological record:

TIME
SESSION
SYMBOL
TIMEFRAME
TRON EVENT
STATE
CONTEXT
NARRATIVE

This creates an auditable history of what TRON actually reported.

The principle:

No rewriting the tape after the fact.

The archive should reflect the actual event chronology.

28. DATA SOURCES

TradingView is the first and most important source because it already executes the actual TRON Pine logic.

Other market-data sources may eventually be integrated where necessary.

Deriv data was discussed as a possible additional source, particularly where instrument-specific live data may matter.

However:

Do not build a second market engine just because an additional data source exists.

First determine:

what TradingView already provides;

what TRON already calculates;

what the webhook can transmit;

what genuinely missing data needs another source.

29. V1.1 UPDATE PAGE — PROPOSED INFORMATION HIERARCHY

The Lovable landing page should eventually communicate:

CURRENT

TRON Alpha V1.1

WHAT CHANGED

explicit BUY / SELL labels;

user-feedback-driven refinement;

execution workflow clarification;

M1 Alpha Gate recommendation;

M5 recommended execution timeframe;

H1/M15/M5 operating framework.

WHAT TRON IS

Deterministic market intelligence, not a prediction service.

WHAT COMES NEXT

TRON V2 — Absolute Dollar Agent

COUNTDOWN

25-day launch countdown, targeting approximately September 28, 2026, subject to final confirmation.

EARLY OPERATOR OFFER

After the applicable evaluation period:

$49 lifetime grandfather access

No monthly subscription as the grandfather offer.

30. IMPORTANT BRAND LANGUAGE

Preferred:

TRON

TRON Alpha

TRON Alpha V1.1

Absolute Dollar Agent

TRON V2

Absolute Dollar Intelligence

market intelligence

market reading

decision support

deterministic

augmented intelligence

operator

analysis

observe

execution

state

transition

alignment

internal alignment

developing opportunity

market state

Avoid:

magic AI

guaranteed signals

guaranteed profits

prediction machine

win-rate promises

"AI knows where price will go"

arbitrary confidence percentages

invented signals

language that implies TRON can guarantee outcomes

31. SAFETY / CLAIMS DISCIPLINE

The product should be described accurately.

Do not make unsupported performance claims.

Do not claim that TRON guarantees profitable outcomes.

Do not fabricate backtests.

Do not turn historical observations into guaranteed future results.

The system should clearly distinguish:

Observed TRON state

from

operator interpretation

from

future uncertainty

32. WHAT THE USER WANTS TO DO NEXT

Immediate sequence:

STEP 1 — Upload TRON V1 source

The complete V1 Pine source will be supplied.

STEP 2 — Verify this handover against source

Audit the dictionary and update any technical details that differ from the actual source.

STEP 3 — Update Lovable

Do not redesign.

Update the current landing page to:

remove August beta positioning;

establish V1.1 as the current live product;

add V1.1 update log;

explain BUY/SELL labels;

recommend M5 as execution timeframe;

recommend Alpha Gate for M1 execution;

clearly communicate H1 → M15 → M5 workflow;

introduce V2;

add the 25-day countdown;

introduce the grandfather/lifetime offer;

keep the current visual system.

STEP 4 — Build Whop

Use Whop as the commercial/access layer for the premium product.

STEP 5 — Future webhook proof

Prove:

TradingView → webhook → TRON event → externalized TRON state.

STEP 6 — Future TRON AI

Build the deterministic augmented-intelligence layer around those actual events.

33. CURRENT STRATEGIC VISION

The project is moving from:

"A TradingView indicator with a community around it"

toward:

"A deterministic market-intelligence engine with multiple interfaces."

The interfaces can eventually include:

TradingView

TRON Live

Lovable

Telegram

WhatsApp

archive / tape

future APIs

future data sources

But the underlying identity remains:

TRON is the deterministic market-reading engine.

And the future AI layer is:

Augmented Intelligence that continuously externalizes and organizes what TRON is actually observing as price develops.

34. FINAL SOURCE-OF-TRUTH HIERARCHY

When making future decisions, use this order:

Actual TRON V1/V1.1 Pine source

User's explicit product decisions in the current conversation

The externalized TRON dictionary

The user's Telegram market-intelligence templates

Existing Lovable project architecture/components

General implementation assumptions

If an assumption conflicts with the actual source, the source wins.

If an old Lovable message conflicts with the latest explicit product decision, the latest decision wins.

If generic AI reasoning conflicts with the user's established TRON methodology, do not substitute generic reasoning.

35. ONE-SENTENCE DEFINITION FOR INTERNAL AI

TRON is a deterministic market-reading engine implemented as a live Pine Script indicator; TRON AI is the future augmented-intelligence layer that receives TRON's actual live states/events, maintains their evolving context, prepares faithful analysis and opportunity monitoring as price develops, and communicates those observations across Lovable and external channels without inventing or overriding the underlying TRON logic.

PENDING SOURCE FILE

TRON V1 Pine Script: awaiting upload.

Once uploaded, perform a source-level reconciliation of this handover before modifying the technical documentation or Lovable implementation.
