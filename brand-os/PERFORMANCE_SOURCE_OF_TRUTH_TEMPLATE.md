# RCG Performance Source-of-Truth Reconciliation v0.1

Status: INTERNAL CONTROL — NOT PUBLICATION-READY
Primary claim links: CR-001, CR-002, CR-003, CR-011, CR-012, CR-013

## Purpose
Create one auditable reconciliation layer between authoritative performance evidence and every public performance representation. This file contains no approved return figures and authorizes no publication.

## Reconciliation rule
Never resolve a discrepancy by selecting the higher, newer-looking, or more favorable figure. A figure becomes canonical only after its source, methodology, universe and period reconcile to authoritative evidence.

## Canonical performance record
Create one row for every strategy/period/return basis that may be represented externally.

| Record ID | Strategy canonical name | Historical label | Period start | Period end | Gross / net | Return | Benchmark / comparator | Account / model / proxy / composite | Fee treatment | Source dataset / record | Calculation method | Evidence tier | Verified by | Verification date | Status |
|---|---|---|---|---|---|---:|---|---|---|---|---|---|---|---|---|
| PERF-TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | UNRECONCILED |

Allowed status: UNRECONCILED / RECONCILED-INTERNAL / COMPLIANCE-REVIEW / APPROVED / SUPERSEDED.

## Source evidence packet
For each PERF record retain:
1. original authoritative source identifier and retrieval date;
2. immutable/raw source copy or stable reference;
3. account/strategy universe represented;
4. inclusion/exclusion rules;
5. period boundaries and valuation convention;
6. cash-flow treatment;
7. fee/expense treatment;
8. benchmark source and calculation convention, if used;
9. calculation workbook/notebook/version;
10. preparer and independent reviewer;
11. discrepancies against prior collateral;
12. disclosure version required for any eventual presentation.

## Public representation map
Every website, deck, tear sheet, white paper or other externally reachable representation gets mapped back to a canonical PERF record.

| Artifact ID | Version/date | URL/path | Exact represented figure/claim | PERF record | Disclosure version | Current status | Discrepancy | Action |
|---|---|---|---|---|---|---|---|---|
| ART-TBD | TBD | TBD | TBD | TBD | TBD | INVENTORY | TBD | REVIEW |

Current status: DRAFT / APPROVED / SUPERSEDED / ARCHIVED / UNKNOWN.

## Discrepancy log
| Exception ID | Claim ID | Strategy / period | Source A | Source B | Nature of conflict | Materiality | Resolution evidence | Owner | Status |
|---|---|---|---|---|---|---|---|---|---|
| PX-001 | CR-002 | TBD | Public collateral version A | Public collateral version B | Different return figures for same apparent strategy/period | HIGH | Pending authoritative performance record | TBD | OPEN |
| PX-002 | CR-001 | Firm/performance description | Website/white-paper language | Performance collateral disclosure | "audited" representation conflicts with outside-audit disclaimer | HIGH | Pending exact audit/verification documentation and scope | TBD | OPEN |
| PX-003 | CR-003 | Composite availability | Website disclosure | Maintained composite evidence | Availability not yet substantiated | HIGH | Pending composite definition, account rules, calculation and deliverable | TBD | OPEN |

## Proxy-account control — CR-012
Before proxy-account performance can support external material, record:
- internal account identifier;
- why the account is representative;
- strategy mapping and effective dates;
- whether all intended strategy trades were reflected;
- deviations from other managed accounts;
- cash flows and restrictions;
- fee treatment;
- whether the result is actual account performance versus hypothetical/model output;
- limitations necessary to prevent inference that the proxy is an all-account composite.

A proxy must never be relabeled as a composite merely for presentation consistency.

## Composite control — CR-003
A statement that composite returns are available requires an actual maintained deliverable with:
- composite name and definition;
- account inclusion/exclusion policy;
- effective dates;
- treatment of terminated/new accounts;
- calculation methodology;
- fee treatment;
- underlying account reconciliation;
- reproducible output;
- review/approval record.

Until all fields exist, status remains UNSUBSTANTIATED — DO NOT PROMISE AVAILABILITY.

## Audit / verification control — CR-001
Do not use "audited", "verified", "independently verified" or "proven" based on inference. Record the exact:
- report/provider;
- engagement type;
- entity, accounts, composite or calculations covered;
- period covered;
- standard/procedure;
- report date;
- limitations;
- wording the evidence actually supports.

Financial-statement audit evidence does not automatically substantiate an audited-performance claim.

## Strategy lineage — CR-013
| Lineage ID | Canonical strategy | Historical name | Effective from | Effective to | Investment treatment unchanged? | Evidence | Performance continuity treatment | Status |
|---|---|---|---|---|---|---|---|---|
| LIN-TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | UNRECONCILED |

Names that appear related are not presumed equivalent. Conversely, a rename alone does not create a new track record if authoritative records establish continuity.

## Reconciliation gate
A performance representation cannot advance to APPROVED unless:
1. the canonical performance row is complete;
2. source evidence is attached;
3. calculations are reproducible;
4. strategy lineage is resolved;
5. proxy/model/composite status is explicit;
6. contradictory collateral is logged and resolved;
7. required disclosures are mapped;
8. compliance review is complete.

## Current safe next actions
1. Populate the artifact map for all publicly reachable performance materials.
2. Retrieve authoritative underlying records for each conflicting strategy/period.
3. Build the strategy lineage table before normalizing historical labels.
4. Locate any audit/verification engagement documentation and bound its scope.
5. Determine whether an actual maintained composite exists before retaining availability language.

This is an internal reconciliation template. It changes no public claim, approves no performance figure, and authorizes no external distribution.
