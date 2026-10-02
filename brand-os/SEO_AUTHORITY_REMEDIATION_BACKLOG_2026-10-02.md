# SEO & Authority Remediation Backlog — 2026-10-02

Status: INTERNAL DRAFT — NOT FOR EXTERNAL PUBLICATION  
Scope: reversible remediation planning only. No production changes are authorized by this document.

## Purpose

Translate the website/index authority audit into discrete engineering and content-control work that can be reviewed, tested, and rolled back independently.

## P0 — Claim and authority controls

### 1. Quarantine “audited”
- Do not introduce or repeat “audited,” “independently audited,” or equivalent assurance language in new RCG marketing drafts unless the exact object, period, auditor/assurance provider, standard, and supporting evidence are recorded in the Claim Registry.
- Conflicting historical uses must remain visible in the authority register until resolved; do not silently harmonize source history.
- A source containing “audited” cannot substantiate itself.

Acceptance: no new draft can inherit the term merely because it appears in an older public artifact.

### 2. Performance URL authority classification
Classify every indexable performance-bearing URL or PDF:
- CURRENT — approved current source.
- HISTORICAL — valid dated snapshot retained for historical reference.
- SUPERSEDED — replaced by a newer authoritative artifact.
- UNKNOWN — authority not yet established.

For each item record: URL, artifact date/as-of date, strategy, authority class, successor URL if any, indexability, and reviewer.

Acceptance: any performance number used in a new draft resolves to one CURRENT source plus an as-of date.

### 3. Time-sensitive and absolute claims
Require proposition-level evidence before reuse of:
- AUM/current asset figures;
- “real time,” “continuously,” or similar monitoring claims;
- “within hours” liquidity/execution statements;
- “at all times” transparency statements;
- other absolute or universal operating claims.

Prefer bounded wording where the evidence supports only a narrower proposition.

## P1 — Legacy URL investigation

Investigate the indexed legacy route `/?p=6869` without changing production:
1. Compare response status/body with the canonical homepage.
2. Inspect `rel=canonical`.
3. Inspect robots meta and X-Robots-Tag.
4. Check sitemap inclusion.
5. Search repository/templates/content for internal links to the route or underlying post ID.
6. Determine whether it is a true duplicate, an obsolete artifact, or intentionally distinct content.

Remedy hierarchy:
1. **301 redirect** only if the URL is genuinely superseded and there is a clear successor.
2. **Canonical correction** when duplicate URLs must remain technically reachable but one authoritative URL should consolidate indexing.
3. **Noindex** only when a separate accessible URL must remain but should not compete in search.
4. Do not use robots.txt as a substitute for canonicalization/removal.

No remedy is authorized until the classification above is complete.

## P1 — Performance-document freshness

For indexable tearsheets and performance PDFs:
- display an unambiguous as-of date;
- identify CURRENT versus HISTORICAL/SUPERSEDED status in the authority register;
- provide a current-successor reference where technically and compliance-appropriate;
- prevent undated search snippets/titles from implying that an old snapshot is current;
- establish a revalidation trigger whenever a new approved performance period is released.

Do not rewrite historical numbers merely to match current numbers. Preserve dated history and fix authority/navigation instead.

## P2 — Proposed engineering workstreams

Keep technical SEO and investment-marketing copy changes in separate commits.

### A. Canonical / robots / sitemap mechanics
Draft-only branch change covering canonical tags, robots directives, sitemap generation, and automated tests. No performance copy edits.

### B. Legacy-route handling
Separate branch commit for the classified `/?p=6869` remedy. Include before/after status, canonical, indexability, and redirect tests.

### C. Metadata / internal-link cleanup
Correct titles, descriptions, internal links, and stale navigation references only after URL authority is established. Do not alter investment claims in the same commit.

### D. Structured data
Validate Organization/WebSite/Article or other schema only where the visible page supports the same proposition. Structured data must not amplify a claim that is quarantined in visible copy.

## Required tests before any future merge request

- Production build succeeds in a non-production environment.
- Canonical URL is self-consistent on authoritative pages.
- Superseded URLs behave exactly as classified.
- Sitemap contains only intended canonical/indexable URLs.
- No accidental `noindex` on authoritative pages.
- No redirect chains or loops introduced.
- Internal links resolve to intended authoritative URLs.
- Structured data matches visible content.
- Claim Registry review completed for any changed investment-marketing proposition.
- Diff contains no unrelated performance-copy or design changes.

## Commit discipline

Recommended independent commits:
1. `seo: canonical robots sitemap mechanics`
2. `seo: handle classified legacy p-6869 route`
3. `seo: normalize metadata and internal authority links`
4. `seo: align structured data with approved visible claims`

Each commit must be independently revertible. Do not merge these changes to production without Nick's explicit approval of the specific merge/deploy.

## Definition of done

This backlog is complete only when:
- every public performance artifact has an authority class;
- the legacy route has a documented classification and tested proposed remedy;
- conflicting assurance terminology has an evidence-backed disposition;
- time-sensitive/absolute claims map to Claim Registry records;
- proposed technical changes exist only on a review branch with test evidence;
- production remains unchanged until explicit approval.
