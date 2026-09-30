# ED-005 — Research Infrastructure as Investment Discipline

Status: INTERNAL LONG-FORM OUTLINE — NOT APPROVED FOR EXTERNAL MARKETING  
Editorial ID: ED-005  
Pillar: Firm craft  
Controls: `EDITORIAL_INVENTORY.md`, `STORY_VAULT_EDITORIAL_CONTROL.md`, `CLAIM_REGISTRY.md`  
Last reviewed: 2026-09-30

## Audience / useful question

Prospective clients, allocators, and practitioners asking: how can a focused investment firm make discretionary judgment more repeatable, reviewable, and less dependent on one person's memory?

## Core proposition

A small investment firm does not become institutional by accumulating software. It becomes more disciplined when research, decisions, evidence, risk checks, and postmortems leave a durable trail. The objective is not to automate judgment away; it is to reserve judgment for decisions where it adds value and make the surrounding process reproducible.

## Draft thesis

The operating advantage of a focused firm can be speed and clarity, but those advantages disappear when the investment process lives primarily in the portfolio manager's head. Research infrastructure should therefore be designed as a decision system rather than a collection of tools.

A useful system has five properties:

1. **Traceability** — every material conclusion can be traced to dated evidence and assumptions.
2. **Reproducibility** — calculations and research outputs can be recreated from identified inputs.
3. **Separation of observation and interpretation** — facts, calculations, inferences, and opinions are labeled differently.
4. **Decision memory** — the original thesis, sizing logic, invalidation conditions, and uncertainty survive the outcome.
5. **Reviewability** — later evaluation can distinguish thesis quality, sizing quality, execution quality, and luck.

## Proposed article architecture

### 1. The real scaling problem is decision memory

Opening idea: a growing research stack creates more information but not necessarily more knowledge. The bottleneck becomes whether the firm can reconstruct why a decision was made, what evidence was available at the time, and what would have changed the decision.

Safe angle: discuss the general operating problem without AUM, client-count, performance, or comparative claims.

### 2. Build an evidence chain before building more dashboards

Describe a controlled research object:

`SOURCE → OBSERVATION → CALCULATION → INFERENCE → DECISION → REVIEW`

For every material research item, retain:
- source and retrieval/as-of date;
- exact proposition supported;
- transformation/calculation method;
- assumptions and uncertainty;
- decision relevance;
- owner/status;
- revalidation trigger.

Editorial point: a chart without provenance is a picture; a conclusion without an evidence chain is difficult to audit.

### 3. Keep facts, calculations, inferences, and opinions separate

Use the Brand OS classification:

- **FACT:** directly supported by identified evidence.
- **CALCULATION:** reproducible transformation of identified inputs.
- **INFERENCE:** interpretation that could reasonably be disputed.
- **OPINION / FORECAST:** judgment about meaning or future state.

Explain why this matters: outcome knowledge creates hindsight pressure. Explicit labels make it harder to rewrite yesterday's uncertainty as today's certainty.

### 4. The decision journal is the bridge from research to portfolio action

Minimum decision record:
- timestamp;
- thesis;
- evidence set;
- competing explanation;
- sizing rationale;
- key risks;
- invalidation conditions;
- expected horizon;
- action/no-action;
- subsequent amendments with timestamps.

Do not use a winning trade as the illustrative example unless the evidence packet also contains the contemporaneous uncertainty and counterfactual. A synthetic example is safer for an initial public candidate.

### 5. Separate decision quality from outcome quality

Postmortem grid:

| Thesis | Sizing / risk | Outcome | Review question |
|---|---|---|---|
| Sound | Sound | Good | Was success consistent with the original mechanism? |
| Sound | Sound | Bad | Was this acceptable uncertainty or was a risk omitted? |
| Weak | Sound | Good | Did luck rescue a poor thesis? |
| Sound | Weak | Mixed/bad | Did implementation overwhelm otherwise useful research? |
| Weak | Weak | Good | Do not let P&L validate the process. |

This section deliberately avoids performance figures.

### 6. Automate collection and checking; preserve accountable judgment

Candidate automation domains:
- ingestion and normalization of repeatable datasets;
- stale-data and missing-data checks;
- calculation pipelines;
- risk and exposure monitoring;
- evidence/version capture;
- exception queues;
- scheduled review prompts.

Human-accountability domains:
- deciding whether evidence is decision-relevant;
- resolving conflicting signals;
- choosing sizing under uncertainty;
- overriding a model;
- changing a mandate or methodology;
- approving external representations.

Core line for later drafting: automation should reduce clerical discretion, not obscure investment discretion.

### 7. Treat exceptions as information

A robust operating system should surface unresolved items rather than silently coerce them into a clean answer. Examples:
- conflicting source values;
- stale evidence;
- methodology changes;
- strategy-name changes;
- missing account coverage;
- unsupported marketing claims.

Connect this to the internal claim/evidence architecture without exposing sensitive implementation details.

### 8. What good infrastructure should buy

Frame benefits without superiority or performance claims:
- faster reconstruction of past decisions;
- less dependence on memory;
- clearer handoffs and reviews;
- easier detection of stale assumptions;
- more consistent research hygiene;
- better separation of research, portfolio action, and external communication.

Avoid promising better returns, lower losses, real-time monitoring, or institutional equivalence.

## Evidence packet

### EP-005-A — Internal controls already created

Primary internal evidence:
- `BRAND_BRAIN_EVIDENCE_CONTROL.md`
- `CLAIM_REGISTRY.md`
- `PERFORMANCE_SOURCE_OF_TRUTH_TEMPLATE.md`
- `STORY_VAULT_EDITORIAL_CONTROL.md`
- `EDITORIAL_INVENTORY.md`
- `COLLATERAL_AUTHORITY_REGISTER.md`
- `WEBSITE_SEO_AUTHORITY_AUDIT_2026-09-30.md`

Supported proposition: RCG is building a documented evidence, claim, editorial, and performance-control architecture.

Boundary: existence of internal controls does not prove that every historical investment decision followed these controls.

### EP-005-B — Public-site language to avoid inheriting without separate substantiation

The current public site contains operational assertions such as continuous automated monitoring, real-time tracking, exclusively liquid exchange-traded instruments, and positions reducible within hours. These are not evidence for this article. If later used, map them to dedicated operational claim records and supporting system/portfolio evidence first.

## Controlled-claim posture

- CR-001 audited/verified/proven performance: EXCLUDED.
- CR-002 historical returns: EXCLUDED.
- CR-003 composite availability: EXCLUDED.
- CR-008 registration status: NOT NEEDED.
- CR-009 AUM/client scale: EXCLUDED.
- CR-010 superiority/institutional-grade language: EXCLUDED.
- CR-012 proxy-account performance: EXCLUDED.
- CR-015 client/holding/trade facts: EXCLUDED.

## Compliance / hindsight checks

Before promotion beyond internal draft:
1. Verify that every statement about current RCG operating practice is actually implemented, not merely aspirational.
2. Convert aspirational architecture to “we are building” or general-principle language where implementation evidence is incomplete.
3. Use no specific trade example without a contemporaneous evidence packet.
4. Use no client/account identifiers or non-public positions.
5. Do not imply that process discipline guarantees investment outcomes.
6. Re-run controlled-claim review after substantive edits.

## Reusable derivative drafts after evidence check

- Long-form research note: “Research Infrastructure Is Part of the Investment Process.”
- Short note: “A Decision System, Not a Dashboard Collection.”
- Diagram: source → observation → calculation → inference → decision → review.
- Checklist: minimum viable decision journal.
- Founder note: what should remain human judgment as research automation expands.

## Next safe step

Validate the statements describing *current* RCG operating practice against actual workflow artifacts. Until that validation is complete, keep the piece framed as operating doctrine and architecture rather than a claim that every component is already live.

This outline is an internal drafting artifact. It authorizes no external publication.
