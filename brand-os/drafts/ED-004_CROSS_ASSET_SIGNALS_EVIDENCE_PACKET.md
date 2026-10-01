# ED-004 — Cross-Asset Signals Evidence Packet

**Status:** Internal evidence-control draft; not approved for external publication.  
**Purpose:** Define the minimum evidence required before RCG publishes educational or marketing content about cross-asset signals.  
**Control principle:** A chart is not evidence of predictability. A relationship must be reproducible, time-valid, appropriately qualified, and tied to a precisely scoped claim.

## 1. Proposed editorial thesis

Working title: **What Cross-Asset Signals Can Tell You — and What They Cannot**

Permitted thesis at draft stage:

> Cross-asset observations can provide context for portfolio decisions when their construction, timing, limitations, and failure cases are explicit.

This packet does **not** authorize claims that an RCG signal predicts markets, generates alpha, improves returns, reduces drawdowns, or is currently used in production.

## 2. Claim ladder

Every statement must be classified before drafting.

| Level | Claim type | Example form | Default status |
|---|---|---|---|
| L1 | Descriptive | “X and Y moved in opposite directions during this interval.” | May proceed with sourced data |
| L2 | Conditional | “Historically, condition A has coincided with condition B in the defined sample.” | Requires reproducible test |
| L3 | Interpretive | “One possible interpretation is…” | Requires L1/L2 evidence + alternatives |
| L4 | Decision-use | “This information can affect sizing / risk review under defined conditions.” | Requires documented decision framework |
| L5 | Predictive | “Signal X forecasts / predicts / anticipates Y.” | Blocked absent separate predictive-evidence approval |

No lower level may be worded so strongly that a reasonable reader would infer a higher-level claim.

## 3. Per-signal evidence record

For every signal proposed for inclusion, record:

- Signal ID and plain-English name.
- Economic hypothesis and plausible transmission mechanism.
- Exact input series, vendor/source, field identifiers, units, currency, timezone, and frequency.
- Source retrieval date and dataset/version where available.
- Transformations, normalization, winsorization, smoothing, lags, thresholds, and missing-data treatment.
- Target variable and exact horizon.
- Sample start/end dates and exclusions.
- What was observable at each historical decision timestamp.
- Publication/release lag for each input.
- Revision policy and whether historical values can be revised.
- Test statistic(s), uncertainty measure(s), and number of observations.
- Subperiod and regime behavior.
- Counterexamples and known failure modes.
- Whether parameters were selected before or after observing results.
- Number of alternative specifications examined.
- Implementation delay/cost assumptions if the claim crosses into decision-use.
- Reproduction owner, code/data location, and reproduction date.
- Claim-ladder level authorized by the evidence.

## 4. Time-integrity gate

A historical relationship fails the publication gate until the analysis establishes what information was actually available at the relevant historical timestamp.

Explicitly test for:

1. **Release lag:** macro/fundamental data may be published after the period they describe.
2. **Revision:** later-vintage data may differ materially from the first release.
3. **Look-ahead:** calculations must not use information unavailable at the decision time.
4. **Threshold hindsight:** cutoffs chosen after seeing outcomes must be disclosed and treated as exploratory.
5. **Specification search:** testing many variants raises false-discovery risk.
6. **Survivorship/constituent bias:** historical universes must reflect what existed then where relevant.
7. **Calendar/timezone alignment:** closes, releases, and asynchronous markets must be aligned to observable timestamps.
8. **Implementation lag:** a decision-use claim must reflect realistic delay between observation and action.

If point-in-time data are unavailable, the limitation must be explicit and the claim normally remains descriptive or exploratory.

## 5. Reproducibility gate

A signal is reproducible only if an independent reviewer can recreate the chart/table from the recorded sources and methodology without discretionary reconstruction.

Minimum packet:

- immutable or versioned analysis code;
- source manifest;
- transformation specification;
- parameter file or explicit parameters;
- output checksum or archived output;
- environment/dependency record where material;
- reviewer/date;
- variance explanation if reproduction does not match exactly.

“Recreated approximately” is not sufficient for a quantitative claim.

## 6. Statistical and economic checks

The analysis should distinguish statistical association from economic usefulness.

Required where applicable:

- effect magnitude, not only direction;
- uncertainty/confidence intervals rather than isolated point estimates;
- sample size;
- sensitivity to start/end dates;
- rolling or subperiod stability;
- regime dependence;
- outlier dependence;
- autocorrelation/overlapping-horizon considerations;
- multiple-testing/specification-search disclosure;
- plausible mechanism;
- transaction costs, spreads, financing, market impact, and delay if implementation is implied.

Statistical significance alone does not authorize a decision-use or predictive claim.

## 7. Counterexample requirement

Every externally usable signal discussion must include at least one material failure case or environment in which the relationship weakened, reversed, or became ambiguous.

The counterexample must not be trivialized. Record:

- date/regime;
- observed signal;
- expected interpretation;
- actual outcome;
- plausible explanation;
- whether the episode changes the authorized claim level.

This prevents the Story Vault from becoming a collection of only favorable historical anecdotes.

## 8. Neutral example-selection rule

Examples must be selected by a predeclared rule rather than because the subsequent outcome makes the framework look prescient.

Acceptable methods include:

- most recent completed occurrence as of a predeclared cutoff;
- all occurrences in a defined period;
- fixed calendar sampling;
- mechanically selected strongest/weakest readings under a threshold defined before outcome review.

If an example was chosen editorially after seeing the outcome, label it illustrative and do not use it as evidence of efficacy.

## 9. Chart and table standard

Every chart intended for eventual external review should carry or map to:

- descriptive title;
- exact series labels and units;
- visible date range;
- source(s);
- data/as-of date;
- transformation note;
- recession/regime shading source if used;
- clear distinction between observed and modeled data;
- no truncated axis or visual treatment that materially exaggerates an effect;
- claim ID / signal ID in internal metadata.

Annotations must describe what happened, not silently convert correlation into causation.

## 10. Performance quarantine

Signal research and investment-performance advertising are separate evidence domains.

Do not include in ED-004 without a separate approved performance packet:

- strategy returns;
- hypothetical or backtested portfolio returns;
- hit rates framed as investor outcomes;
- Sharpe/Sortino or drawdown improvement;
- “alpha generated” by the signal;
- cherry-picked profitable trades;
- comparisons implying superiority.

If a backtest is genuinely necessary to explain methodology, quarantine it as research evidence and route it through the applicable performance/hypothetical-performance review before external use.

## 11. Practice-versus-framework control

Until implementation evidence exists, permitted language is framework-oriented:

- “A cross-asset process can…”
- “One way to test this relationship is…”
- “A portfolio manager may use the observation as context…”

Evidence-gated language includes:

- “RCG monitors…”
- “Our model identifies…”
- “We use this signal to…”
- “The system predicts…”
- “Our cross-asset engine…”

A validated individual signal does not substantiate a broad claim about an “RCG cross-asset model,” production system, or firmwide predictive capability.

## 12. Evidence packet approval checklist

Before a signal enters an external draft:

- [ ] Signal definition is exact and versioned.
- [ ] Data provenance is complete.
- [ ] Historical observability/release lag is tested.
- [ ] Revision/look-ahead risks are addressed.
- [ ] Analysis is independently reproducible.
- [ ] Specification search is documented.
- [ ] Subperiod/regime behavior is shown.
- [ ] At least one material counterexample is included.
- [ ] Example selection is neutral or explicitly illustrative.
- [ ] Chart metadata and as-of dates are complete.
- [ ] Claim level is assigned.
- [ ] Language does not exceed the authorized claim level.
- [ ] Performance claims, if any, have separate approval.
- [ ] RCG-practice language has implementation evidence.
- [ ] Compliance/evidence review is recorded before publication.

## 13. Suggested article structure after evidence approval

1. Why investors look across asset classes.
2. Observation is not prediction.
3. Three ways cross-asset information can be useful: context, contradiction, and risk review.
4. One or more fully evidenced signal examples.
5. What the examples cannot establish.
6. Failure regimes and counterexamples.
7. How to preserve time integrity in historical analysis.
8. From signal to decision: why sizing and portfolio context still matter.
9. Closing principle: use signals to discipline questions, not manufacture certainty.

## 14. Relationship to Brand OS

- **Brand Brain:** use the claim ladder to prevent unsupported escalation from research observation to firm capability.
- **Story Vault:** store signal examples only with provenance, neutral-selection status, and counterexamples.
- **Editorial Inventory:** ED-004 remains evidence-gated until at least one signal packet passes the controls above.
- **Claim Registry:** any RCG-specific capability or predictive representation requires a distinct claim record.
- **Performance Source of Truth:** strategy or hypothetical performance must never be sourced from this packet alone.

## 15. Current disposition

**Draft-ready:** educational discussion of evidence hygiene, time integrity, reproducibility, and limitations of cross-asset analysis.

**Evidence-gated:** named RCG signals, current production practices, decision-use claims, and statements about model efficacy.

**Blocked absent separate approval:** predictive claims, performance claims, superiority claims, or language implying verified alpha generation.

Passing one signal packet authorizes drafting around that signal only. It does not validate other signals or a broader RCG modeling capability.
