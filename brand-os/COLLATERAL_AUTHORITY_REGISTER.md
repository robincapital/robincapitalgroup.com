# RCG Collateral & Authority Artifact Register

Status: INTERNAL CONTROL — NOT APPROVED FOR EXTERNAL DISTRIBUTION

## Purpose
Maintain a single inventory of website and collateral artifacts so identity, authority, performance, regulatory, and version claims can be reconciled before publication. Retirement means preserve + supersede; never silently delete historical evidence.

## Lifecycle
- CURRENT-CANDIDATE — candidate for controlled current use after evidence/compliance checks.
- UNKNOWN — provenance or distribution state not yet established.
- SUPERSEDED-CANDIDATE — appears replaced; retain until lineage and inbound links are verified.
- ARCHIVE-CANDIDATE — preserve for records; not intended for public distribution.
- BLOCKED — contains unresolved controlled claims and must not advance.

## Required fields
Artifact ID; title; repository/path or source; version/date; SHA/hash; intended audience; distribution surface; provenance owner/source; lifecycle; linked CR claim IDs; linked PERF IDs; evidence status; inbound links; replacement/supersession target; review date; reviewer; notes.

## Seed inventory
| ID | Artifact | State | Known control issue | Safe next action |
|---|---|---|---|---|
| ART-001 | Primary website / index.html | CURRENT-CANDIDATE | Duplicate schema; address exposure; January deck links; unresolved performance-disclosure wording | Page-level authority/SEO matrix and claim mapping; propose branch-only diff |
| ART-002 | January 2026 investor deck candidate A | BLOCKED | Performance/version reconciliation unresolved | Hash, extract claims, map every performance representation to PERF records |
| ART-003 | January 2026 investor deck candidate B | BLOCKED | Conflicts with another January 2026 collateral candidate | Hash, compare exact figures/periods/methodology; do not select favorable version |
| ART-004 | Safe Haven tear sheet | UNKNOWN | Performance and distribution provenance not yet mapped | Establish exact source/version and map controlled claims |
| ART-005 | Portfolio-construction white paper | UNKNOWN | Authority/evidence provenance not yet mapped | Inventory factual claims and citations; classify reusable evergreen material |
| ART-006 | index (4).html | UNKNOWN | Duplicate/legacy website artifact; deployment history unknown | Determine commit/deployment provenance before archive decision |

Seed mappings above are control prompts, not assertions that every referenced claim appears in every artifact. Exact claim occurrence must be verified before a CR or PERF mapping is marked confirmed.

## Claim-to-artifact control
Every externally reachable controlled claim must resolve:
ARTIFACT -> exact location -> CR claim family -> evidence source -> approval state.
Every performance representation additionally resolves:
ARTIFACT -> exact figure/period/basis -> PERF record -> source dataset/calculation -> reconciliation status.

Conflicting figures are never reconciled at the collateral layer by choosing the more favorable number.

## Canonicalization rules
1. Same-title artifacts with different bytes receive distinct artifact IDs and hashes.
2. Filename similarity never establishes version lineage.
3. A superseded artifact remains retained for records and receives an explicit replacement pointer.
4. Archive retention and public distribution are separate states.
5. Public links to blocked/superseded collateral are remediation candidates, not authorization to delete source evidence.
6. Historical strategy labels remain distinct until the strategy-lineage control establishes continuity.
7. “Audited,” “verified,” “proven,” composite, AUM/client-count, regulatory-status, superiority, testimonial/award, and performance claims require their applicable Claim Registry evidence before release.

## SEO / authority consistency gate
For each indexable page or public collateral surface, verify:
- canonical organization/founder identity;
- canonical location wording and privacy policy;
- dated regulatory wording;
- strategy-name lineage;
- canonical URL, title, description, Open Graph/social metadata;
- structured-data consistency and absence of duplicate schema;
- controlled-claim mappings;
- performance mappings where applicable;
- current collateral version and supersession pointer;
- no contradictory claims across website, PDF, metadata, and schema.

## Execution queue
1. Enumerate publicly reachable PDFs and collateral.
2. Hash same-title/version candidates.
3. Extract and map every performance statement to a PERF record.
4. Locate every occurrence of audited / verified / proven and map to CR-001.
5. Trace inbound website/repository links to January 2026 deck candidates.
6. Establish whether index (4).html was deployed or is only a repository remnant.
7. Build page-level SEO/authority matrix.
8. Draft branch-only remediation diffs; no merge/deploy without explicit approval.

## Release gate
An artifact may become PUBLICATION-CANDIDATE only when provenance is known, controlled claims are evidence-mapped, performance exceptions are reconciled, supersession state is explicit, compliance review is recorded where required, and the distribution surface points to the intended current version.

This register authorizes no publication, merge, deployment, deletion, purchase, or external distribution.
