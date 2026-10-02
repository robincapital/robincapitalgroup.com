# RCG Controlled Claim Registry — Operating Extension

Status: INTERNAL CONTROL — NOT PUBLICATION-READY  
Date: 2026-10-02  
Purpose: extend the controlled-claim registry to operational and website-authority statements identified during the October 2026 authority audit.

## New controlled claims

| ID | Claim / claim family | Class | Status | Evidence required | Drafting boundary |
|---|---|---|---|---|---|
| CR-016 | RCG monitors markets, portfolios, risks, or signals "continuously" | Operating capability | YELLOW | System/log evidence; monitored universe; coverage hours; exceptions; evidence as-of date | Prefer specific documented cadence. Do not use "continuously" as an absolute without coverage evidence. |
| CR-017 | RCG data, monitoring, analytics, signals, or decisions operate in "real time" | Operating capability | YELLOW | Feed/source; latency measurement; timestamp convention; outage/fallback treatment; observed period | State measured latency/cadence and scope instead of "real time" unless substantiated. |
| CR-018 | Positions can be liquidated "within hours" | Liquidity / risk | RED | Position-level liquidity methodology; market/size assumptions; stressed conditions; instrument exceptions; measurement date | Do not state a universal liquidation horizon. Any supported wording must carry assumptions and scope. |
| CR-019 | Clients/investors receive "full position-level transparency at all times" | Client service / operating capability | RED | Contract/service policy; delivery mechanism; access cadence; universe; outage/delay exceptions | Avoid "full" and "at all times" absent evidence proving both completeness and uninterrupted availability. |
| CR-020 | Current "$30M+" or other AUM/assets figure | Firm metric | YELLOW | Current ADV/custodian/internal books; metric definition; entity/universe; as-of date | Falls under CR-009. Never publish without an explicit as-of date and defined metric. |
| CR-021 | A public performance URL/document is current authoritative material | Collateral / performance authority | YELLOW | URL inventory; document date; performance vintage; owner; supersession record; canonical/current designation | Every performance artifact must be classified CURRENT/HISTORICAL/SUPERSEDED/UNKNOWN before reuse. |
| CR-022 | Legacy or duplicate website routes represent current RCG copy | Website authority | RED by default | Route provenance; canonical target; sitemap/internal-link status; content/version comparison | Do not quote or reuse a legacy/duplicate route until authority is established. |
| CR-023 | Website statements accurately describe production research/trading infrastructure | Operating capability | YELLOW | Production architecture evidence; service/data-feed status; logs; owner; as-of date | Research, prototypes, plans, and branch code do not establish production capability. |
| CR-024 | RCG's process is systematic/automated/data-backed in a specified way | Investment process | YELLOW | Approved methodology; operating evidence; scope; human-discretion boundary; date | Describe only evidenced components; do not imply autonomous or universal operation from research tooling. |

## Cross-reference rules

- CR-020 inherits CR-009's mandatory as-of-date and metric-definition requirements.
- CR-021 inherits CR-002, CR-003 and CR-012 whenever the artifact contains performance.
- CR-016 through CR-019 and CR-023/024 must be revalidated after material architecture, vendor, feed, staffing, policy, or service changes.
- Evidence of a system's design is not evidence that it operated as designed during a claimed period.
- A screenshot or marketing page is discovery evidence only; it cannot self-substantiate the operating claim it makes.

## Evidence packet for operating-capability claims

Minimum fields:
1. exact proposed wording and Claim Registry ID;
2. system/process owner;
3. production vs research/prototype status;
4. covered strategies/accounts/instruments;
5. measurement period and as-of date;
6. source logs, policy, contract, architecture record, or reproducible test;
7. cadence/latency/service-level definition;
8. known outages, exceptions, fallbacks and exclusions;
9. FACT / CALCULATION / INFERENCE / OPINION classification;
10. approved wording boundary;
11. revalidation trigger and reviewer.

## Immediate evidence queue

1. CR-021/022 — classify every indexed performance and legacy website route by authority.
2. CR-016/017 — replace absolute monitoring/latency language with measured, scoped facts.
3. CR-018 — document liquidity methodology before any liquidation-horizon claim.
4. CR-019 — reconcile transparency wording to actual client service terms and delivery mechanics.
5. CR-020 — tie any current asset figure to a dated authoritative record.
6. CR-023/024 — separate production capabilities from research roadmap and prototypes.

No external publication is authorized by this extension.
