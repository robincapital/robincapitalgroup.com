# ED-003 — Drawdown Control Is Portfolio Design, Not a Post-Trade Repair

Status: INTERNAL OUTLINE — NOT APPROVED FOR EXTERNAL MARKETING  
Editorial ID: ED-003  
Pillar: Capital preservation  
Controls: `BRAND_BRAIN_EVIDENCE_CONTROL.md`, `STORY_VAULT_EDITORIAL_CONTROL.md`, `CLAIM_REGISTRY.md`

## Editorial thesis

Drawdown control is strongest when it is designed into portfolio construction before a position is entered. Risk limits applied only after losses appear are necessary controls, but they are not a substitute for ex-ante decisions about exposure, concentration, liquidity, correlation, sizing, scenario sensitivity, and the conditions under which a thesis should be reduced or invalidated.

This is an educational framework. It does not claim that drawdowns can be prevented, that any RCG strategy follows every practice below, or that any framework guarantees a particular loss profile.

## Reader promise

Give an allocator or sophisticated investor a practical way to distinguish a portfolio that merely has stop-loss rules from one whose risk architecture begins at construction.

## Core structure

### 1. Drawdown begins before the drawdown

A portfolio's eventual path is partly shaped when exposures are first combined. The relevant question is not only "where do we exit?" but "what portfolio did we create before an exit became necessary?"

Topics:
- position size as a first-order risk decision;
- concentration by economic driver rather than ticker count;
- gross and net exposure as incomplete summaries;
- liquidity as a sizing constraint;
- correlation instability;
- path dependency and compounding.

### 2. Separate thesis risk from portfolio risk

A sound individual thesis can still be an unsuitable portfolio position. The framework should distinguish:
- thesis validity;
- implementation risk;
- sizing risk;
- factor/correlation overlap;
- liquidity risk;
- portfolio-level downside contribution.

Editorial control: do not imply that these dimensions are currently measured by RCG unless operating evidence is mapped.

### 3. Budget risk before allocating capital

Potential educational model:

`idea → downside cases → exposure map → liquidity test → sizing range → portfolio interaction → entry decision`

The useful discipline is to define the acceptable risk contribution before enthusiasm for an idea determines size.

Questions for the evidence-backed version:
- What loss or adverse move is plausible without invalidating the thesis?
- What changes under stressed correlation?
- How quickly could exposure realistically be reduced under ordinary and stressed liquidity?
- Which existing positions express the same underlying bet?
- What event would change the sizing decision even if the thesis remained intact?

### 4. Diversification should be economic, not cosmetic

Ten positions do not necessarily represent ten independent risks. Portfolio review should look through instrument labels toward shared drivers such as rates, dollar sensitivity, equity beta, volatility, liquidity, geography, commodity exposure, or a common macro scenario.

Avoid categorical claims that a particular number of positions or asset classes creates diversification.

### 5. Liquidity is part of portfolio construction

Liquidity affects the feasible size of a position and the credibility of an exit plan. A useful framework records the liquidity assumption when a position is initiated rather than introducing it only after conditions deteriorate.

Controlled-claim warning: do not reuse public assertions about positions being reducible "within hours," exclusively exchange-traded instruments, or continuous monitoring unless the operational evidence gate is satisfied.

### 6. Predefine responses without pretending the future is predefined

Ex-ante rules can define decision triggers without assuming markets will behave as modeled.

Possible trigger classes:
- thesis invalidation;
- volatility/regime change;
- correlation break;
- liquidity deterioration;
- portfolio concentration breach;
- new information that changes expected payoff.

The response can be review, reduce, hedge, exit, or deliberately hold. The framework should avoid presenting mechanical exits as universally optimal.

### 7. Treat drawdown as diagnostic information

A loss is not automatically evidence that the original decision was poor; a gain is not automatically evidence that it was good. Postmortems should ask whether the loss came from:
- an understood scenario inside the original risk budget;
- thesis failure;
- sizing error;
- hidden factor overlap;
- liquidity assumptions;
- execution;
- a regime shift not represented in the original model.

This section should cross-reference ED-002's separation of thesis quality, sizing/implementation quality, and outcome.

### 8. Portfolio repair is the last layer, not the first

Stops, hedges, reductions, and exits remain important. The distinction is sequencing: reactive controls operate on a portfolio whose initial architecture has already determined much of its vulnerability.

## Proposed visual

A simple two-column diagnostic:

| Reactive-only question | Design-first question |
|---|---|
| Where is the stop? | What risk did we allocate before entry? |
| How much has it lost? | What changed in thesis, exposure, liquidity or correlation? |
| Which position should we cut? | Which economic driver is creating portfolio-level risk? |
| Can we hedge now? | Was the hedge or response path considered ex ante? |

## Evidence packet required before promotion

Before this outline can become an RCG-specific public draft, attach evidence for any firm-practice statement:
1. approved portfolio-construction/risk methodology and version date;
2. documented sizing or exposure rules;
3. liquidity methodology, if referenced;
4. correlation/factor methodology, if referenced;
5. contemporaneous examples selected by a neutral rule;
6. evidence of actual implementation/coverage, not merely policy text;
7. controlled-claim review against the Claim Registry.

If evidence supports only the general framework, publishable language must remain educational ("a manager can," "a framework should") rather than institutional ("RCG does").

## Claims deliberately excluded

- guarantees or implications of drawdown prevention;
- maximum-loss promises;
- unsupported risk-adjusted-performance comparisons;
- specific RCG performance figures;
- AUM/client counts;
- composite availability;
- regulatory-status claims;
- "audited," "verified," or "proven" performance language;
- current or historical positions without approved evidence;
- superiority claims.

## Drafting test

A future draft passes only if a skeptical reader can tell, sentence by sentence, whether a statement is:
- a general investment principle;
- an RCG philosophy;
- a verified RCG operating practice;
- a historical fact;
- an inference or opinion.

Do not collapse those categories.

## Safe next step

Assemble the methodology evidence packet and map each proposed RCG-specific sentence before converting this outline to prose. Until then, this artifact is an internal educational outline only.
