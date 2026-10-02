# Website Index & Authority Drift Audit — 2026-10-02

Status: INTERNAL / DRAFT / NOT FOR EXTERNAL DISTRIBUTION

## Purpose
Capture current search-index authority drift and convert it into reversible remediation work. This document does not authorize publication, deployment, performance advertising, or changes to production.

## Verified search findings
1. The canonical homepage currently presents August 31, 2026 performance and describes returns as a single fully-invested proxy account, TWR, net of management fees, not a GIPS-compliant composite.
2. An indexed legacy route at `/?p=6869` exposes materially different homepage copy and lacks the canonical homepage's full performance/disclosure context in the indexed result.
3. A search-indexed January 2026 Portfolio Construction white paper states RCG has a "live, audited track record." That statement conflicts with indexed January/February/May 2026 strategy materials that say performance results "have not been audited by outside parties."
4. Search-indexed tearsheets remain discoverable with older report dates and older performance figures. This creates source-of-truth/freshness risk even where each document states its as-of date.
5. Current homepage operating claims include "Automated risk monitoring runs continuously," risk inputs are "tracked in real time," "Every position can be reduced or eliminated within hours," and "full position-level transparency at all times." These are testable operating claims and should not be inherited into new editorial/marketing copy without evidence packets.

## Authority conflicts

| ID | Proposition | Current indexed evidence | Control state | Required action |
|---|---|---|---|---|
| WEB-001 | Performance is audited | White paper says "live, audited"; strategy disclosures say not audited by outside parties | CONFLICT / QUARANTINE | Do not reuse "audited." Identify intended meaning and documentary basis. If no scoped third-party audit exists, remove from proposed future collateral. |
| WEB-002 | Which homepage is authoritative | Canonical homepage and `/?p=6869` expose different narratives | DRIFT | Inspect routing/canonical/index directives on a branch; propose redirect/noindex/canonical remediation only. |
| WEB-003 | Current performance source | Homepage is Aug. 31, 2026; indexed tearsheets include Jan/Feb/May 2026 snapshots | STALE-DOC RISK | Create freshness hierarchy and superseded-document policy; preserve historical records internally. |
| WEB-004 | Continuous / real-time risk monitoring | Current homepage | EVIDENCE REQUIRED | Map to dated system logs, monitoring coverage, cadence, exceptions, and outage behavior before reuse. |
| WEB-005 | Positions reducible/eliminable within hours | Current homepage | EVIDENCE REQUIRED | Define scope/exceptions (market hours, halts, liquidity, settlement, size) and substantiate operationally before reuse. |
| WEB-006 | Full position-level transparency at all times | Current homepage | EVIDENCE REQUIRED | Define custodian/client-access mechanism and known exceptions before reuse. |
| WEB-007 | $30M+ AUM | Current homepage/history and indexed white paper | TIME-SENSITIVE | Require dated AUM source, calculation scope, and revalidation date before reuse. |

## Proposed search/index remediation backlog — branch only
P0 — Resolve the contradictory "audited" proposition in the Claim Registry and quarantine the phrase globally for new drafts.

P0 — Inspect how `/?p=6869` is generated. Draft the smallest reversible change that establishes one authoritative homepage via canonical/noindex/redirect behavior. Do not deploy.

P1 — Inventory every indexable performance-bearing URL and assign: CURRENT, HISTORICAL-ARCHIVE, SUPERSEDED, or UNKNOWN. Search-facing pages should identify report date and current-source destination.

P1 — Add a performance-document freshness rule: a dated historical artifact may remain preserved, but must not silently compete with the current source of truth.

P1 — Add evidence packets for continuous/real-time monitoring, liquidity timing, transparency, AUM, registration/status, and employment/credential claims before those propositions are propagated.

P2 — Review sitemap and canonical outputs for attachment pages, query/permalink variants, old PDFs, and tearsheets. Draft technical diffs on a non-production branch only.

## Safe language controls
Until resolved:
- Never describe the track record as audited.
- Never convert "data sourced/calculated by a custodian platform" into "audited."
- Keep historical performance tied to an explicit as-of date and methodology/disclosure block.
- Treat "real time," "continuously," "at all times," and "within hours" as evidence-bearing absolute/near-absolute claims.
- Do not infer firmwide capability from one account, one model, one log sample, or one historical artifact.

## Definition of done for remediation proposal
A branch-only proposal is ready for Nick review when it contains:
1. URL inventory and authority classification.
2. Exact conflicting propositions and evidence.
3. Proposed canonical/noindex/redirect diff with rollback path.
4. Claim Registry updates.
5. No performance-number changes unless reconciled to the approved source of truth.
6. No production merge/deploy and no external publication.
