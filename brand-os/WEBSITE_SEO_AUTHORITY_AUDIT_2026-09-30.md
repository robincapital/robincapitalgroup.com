# Website SEO & Authority Audit — 2026-09-30

Status: INTERNAL DRAFT / CONTROL DOCUMENT  
Scope: website, public collateral, SEO/authority consistency, and evidence gating.  
Publication status: NOT APPROVED FOR EXTERNAL USE.

## Purpose

Create a page-level control layer between the public website/collateral and the Brand Brain, Claim Registry, Collateral Authority Register, and Performance Source-of-Truth. This document does not approve any investment, performance, regulatory, AUM, superiority, testimonial, or assurance claim.

## Authority tests

Every externally reachable page or artifact should pass all ten tests before it is treated as canonical:

1. Identity — firm and individual naming are consistent and supported.
2. Regulatory wording — registration/jurisdiction statements are dated and evidence-backed.
3. Strategy taxonomy — current and historical strategy names map to documented lineage.
4. Performance mapping — every return or benchmark representation maps to a canonical PERF record.
5. Assurance language — audited, auditable, verified, proven, or similar terms map to documentary evidence.
6. Structured data — schema reflects only supported public facts.
7. Metadata — title, description, social metadata, and headings describe the actual canonical page.
8. Canonicalization — canonical URL, sitemap, redirects, and internal links do not create competing authority.
9. Collateral versioning — PDFs and downloadable artifacts carry an as-of/version identity and supersession state.
10. Compliance adjacency — qualifications/disclosures remain close enough to the claim they qualify.

## Page / artifact control matrix

| Surface | Primary authority risk | Evidence/control dependency | Safe action now |
|---|---|---|---|
| Homepage | identity, AUM, regulatory and operating claims | Claim Registry | inventory exact claims; do not strengthen copy |
| Strategy pages | taxonomy, process, liquidity and operational assertions | CR records + strategy lineage | map assertions and historical labels |
| Performance section | proxy/composite distinction, dates, gross/net basis | PERF records + composite evidence | require PERF ID per figure/table |
| About/history | founder history, sole-practitioner vs plural-principal language | identity/history evidence | normalize only after evidence |
| Disclosures | registration, methodology, proxy/composite qualifications | dated regulatory + PERF evidence | check adjacency and consistency |
| January 2026 decks | stale figures, version conflict, assurance wording | Collateral Register + PERF + CR-001 | preserve; identify canonical/superseded state |
| Safe Haven tear sheet | dated performance and strategy claims | PERF + strategy lineage | map all figures and as-of date |
| Portfolio-construction white paper | performance and "audited" language | PERF + CR-001 | block assurance language pending evidence |
| Legacy index (4).html | possible duplicate/deployed authority surface | deployment history | determine whether public or repository-only |

## P0 evidence gates

### Performance
No return should be normalized across website/PDFs merely because strategy names match. Each representation needs: strategy identity, exact period/as-of date, gross/net basis, account/model/proxy/composite classification, fee treatment, source dataset, methodology, and evidence tier.

### Proxy versus composite
A single proxy-account track record must remain explicitly distinct from a composite. Any statement that composite returns exist or are available requires evidence of the composite, its account population, methodology, maintenance history, and applicable disclosures.

### Assurance terminology
"AUDITED", "AUDITABLE", "VERIFIED", "PROVEN", and similar terms are separate claims. Custodian statements, PortfolioAnalyst calculations, or a financial-statement audit do not by themselves establish that investment performance was audited.

### Regulatory and AUM facts
Registration status, jurisdictions, AUM/client counts, addresses, and similar time-sensitive facts require a dated source and revalidation date before reuse in canonical metadata, schema, or marketing copy.

## Technical SEO workstream that can proceed independently

The following are separable from investment-claim approval and may be prepared as branch-only diffs after repository inspection:

- canonical-tag defects and duplicate canonical targets;
- sitemap/robots inconsistencies;
- broken or redirected internal links;
- duplicate/missing H1s and mechanical heading hierarchy defects;
- stale Open Graph/Twitter metadata where replacement text introduces no new claim;
- schema syntax defects and removal of unsupported structured-data fields;
- missing PDF version/as-of labels where the date is already established;
- internal-link improvements among existing canonical educational pages;
- accessibility defects affecting crawlability or comprehension.

Technical fixes must not silently rewrite performance, AUM, regulatory, strategy, superiority, testimonial, or assurance language.

## Proposed remediation sequence

1. Enumerate all publicly reachable HTML and downloadable collateral.
2. Capture current canonical, robots, sitemap, title, description, H1, social metadata, schema, status code, and internal-link state.
3. Extract factual/quantitative claims and map each to CR and, where applicable, PERF IDs.
4. Resolve P0 evidence conflicts before copy normalization.
5. Prepare technical-SEO diffs separately from marketing-copy diffs.
6. Preserve provenance before any artifact is superseded; never silently delete historical evidence.
7. Require explicit approval before merge/deploy or external publication.

## Acceptance criteria for a future canonical site

A page is authority-ready only when its URL state is unambiguous, metadata is internally consistent, structured data contains no unsupported claims, quantitative claims resolve to evidence records, strategy names resolve to lineage, dated facts have revalidation controls, and downloadable collateral is versioned with a clear current/superseded state.

## Current decision

This audit authorizes no production change. It is an internal control artifact for evidence gathering and branch-only remediation planning.
