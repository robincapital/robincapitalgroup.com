# Claim-to-Source Evidence Queue — 2026-10-02

Status: INTERNAL CONTROL / NOT APPROVED FOR EXTERNAL USE

Purpose: convert CR-016 through CR-024 into an executable evidence-retrieval queue. This file does not establish that any claim is true; it defines what must be retrieved before a claim can be promoted.

## Priority queue

| Priority | Claim family | Registry | System-of-record class | Minimum evidence | Pass condition | If incomplete |
|---|---|---|---|---|---|---|
| P0 | Public URL authority / duplicate routes | CR-022 | repository routing, sitemap, canonical metadata, search index observations | route behavior; canonical target; sitemap inclusion; internal links; historical purpose | one documented authoritative URL per content object, with legacy handling justified | classify UNKNOWN; do not infer authority from search rank |
| P0 | Performance-document authority | CR-021 | approved performance source, dated tear sheets, methodology/disclosure record | as-of date; strategy; calculation source; approval status; supersession chain | every cited performance artifact classified CURRENT/HISTORICAL/SUPERSEDED with a current source identified | no performance reuse; classify UNKNOWN |
| P0 | Current AUM | CR-020 | administrator/custodian/accounting or approved firm reporting record | dated aggregate; scope definition; calculation/reconciliation; reviewer | amount, scope, and as-of date reconcile to approved record | omit numeric/current AUM claim or use non-quantified description |
| P1 | Monitoring frequency / latency | CR-016, CR-017 | production logs, scheduler/telemetry, incident history | observation window; actual cadence/latency distribution; outages; system scope | wording bounded by measured cadence/latency and observation period | downgrade to process/design language |
| P1 | Position-level transparency | CR-019 | production portfolio/risk reporting, broker/custodian feeds, outage records | coverage universe; update cadence; exceptions; stale-data behavior | claim explicitly scoped to measured coverage and availability | remove “at all times” and other absolutes |
| P1 | Production infrastructure | CR-023 | deployment inventory, production logs, service ownership, data-feed records | deployed service; production dates; operational owner; live inputs; failure history | evidence shows actual production use, not prototype/research intent | describe as research, development, or planned capability |
| P1 | Systematic / automated / data-backed process | CR-024 | decision journals, model outputs, execution records, process documentation | repeated dated examples linking input -> analysis -> decision; exception handling | operating practice is observable across a defined sample/window | describe framework/process aspiration only |
| P2 | Liquidity / liquidation horizon | CR-018 | holdings, ADV/liquidity data, execution records, stress methodology | security-level assumptions; participation rates; market-impact method; exceptions | horizon is reproducible, portfolio/date scoped, and stress-tested | prohibit universal “within hours” claim |

## Evidence packet required for each operating claim

1. Claim Registry ID.
2. Exact proposed wording.
3. Scope: strategy, system, account population, asset class, and channel.
4. Measurement or observation window.
5. Primary source and retrieval date.
6. Calculation/methodology where applicable.
7. Exceptions, outages, contradictory evidence, and known limitations.
8. FACT / CALCULATION / INFERENCE / OPINION classification.
9. Supported wording boundary: strongest statement the evidence actually permits.
10. Reviewer and review date.
11. Revalidation trigger or expiry date.

## Controlled language ladder

When evidence does not support the strongest formulation, move downward; never move upward by inference:

1. **Absolute claim** — only where the evidence supports an exceptionless statement over the defined scope and period.
2. **Measured/scoped claim** — state the measured cadence, latency, coverage, amount, horizon, or period.
3. **Process description** — describe what the firm does without asserting unmeasured frequency, universality, or outcome.
4. **Research/design description** — describe architecture, testing, development, or intended capability without implying production operation.
5. **Omit** — when even a bounded description would be misleading.

Examples of prohibited inference:
- architecture diagram -> production capability;
- scheduled job -> continuous successful operation;
- dashboard screenshot -> complete/current portfolio coverage;
- model output -> systematic use in investment decisions;
- one fast liquidation -> universal liquidation horizon;
- old tear sheet -> current performance;
- search visibility -> canonical authority.

## Retrieval order

1. Resolve URL and performance-document authority first; these determine which public evidence is safe to cite.
2. Reconcile current AUM only from a dated approved system of record.
3. Retrieve production telemetry and exception history for monitoring/transparency claims.
4. Retrieve deployment and decision records for infrastructure/process claims.
5. Treat liquidity-horizon claims last because they require portfolio-, date-, and methodology-specific substantiation.

## Promotion rule

No CR-016–CR-024 claim advances to externally reusable language until its packet is complete, contradictory evidence is recorded, the wording boundary is explicit, and the relevant authority source is CURRENT. Approval of one claim, date, strategy, system, or channel does not cascade to another.
