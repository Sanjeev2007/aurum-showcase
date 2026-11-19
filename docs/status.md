# Project status

Last reviewed: **19 November 2026**, against private source revision `f2f3467`.

**Aurum is pre-1.0.** The implementation is substantial, but its investment hypothesis and end-to-end live readiness remain unproven. The public screenshots are synthetic UI examples, not evidence of investment performance.

## Implemented

| Area | What exists | What this does not establish |
|---|---|---|
| Quantitative pipeline | Universe construction, 13 accounting gates, sector-relative factor scoring, entry bar and bounded shortlist | That the score predicts returns or that the provisional bar is appropriate |
| Documents | Content-addressed storage, section location, deterministic auditor parsing, cited-fact verification, enrichment and gate re-evaluation, extraction and reasoning | Reliable coverage across all real filing formats |
| Disclosure monitoring | Mandatory state checks, best-effort event coverage, explicit gaps and separation of alerts from verified evidence | Complete news or official-event coverage |
| Decision path | Portfolio constraints, buy/add/constrained split/no-buy branches, thesis and invalidation conditions, memo generation | Approval to allocate real money |
| Journal | Seal-on-completion lifecycle, input manifest and hashes, provenance, rollback handling and replay-oriented consumers | An established forward investment track record |
| Operations | Preflight checks, dry-run isolation, monthly command, ticket generation, trade recording and holdings-only review | A fully accepted live monthly routine or automatic backup |
| Dashboard | Seven journal screens plus a separate holdings view | A public hosted product, broker integration or automatic trading |
| Evaluation | Historical panel and evaluation harness, pre-registration guards, holdout-look budget and data-quality audit tooling | A completed strategy evaluation, demonstrated alpha or a passing go-live gate |

## Validation still open

1. **Live data and shakedown.** Resume the attended cache acquisition and complete a successful full-universe live dry-run. Providers have refused bulk requests before; resumability, spacing and a shared request budget mitigate this but do not guarantee availability.
2. **Document probe.** The early five-company probe did not meet its acceptance criteria: clean controls were demoted for missing evidence, and evidence-handling defects obscured adverse findings. Follow-up cited-facts, parser and runtime work has landed. The completed-pipeline probe is pre-registered and scripted, with replacement controls recorded, but its acquisition, model runs, citation judging and acceptance remain pending. This is a regression check with known controls, not a blind proof of generalisation.
3. **Historical input quality.** Remaining as-filed financial transcriptions, missing-session work and acquisition/audit completion block the initial strategy evaluation. Today's restated fundamentals and incomplete delisted-company coverage can bias any retrospective result.
4. **Strategy evidence.** The pre-registered evaluation must be run and assessed before selecting the recipe. The research protocol limits holdout access and permits only bounded redesign; it does not guarantee a passing strategy. Historical success would be provisional and requires forward evidence.
5. **Policy locks.** Remaining decisions include absolute eligibility floors versus the interpretation of the score bar, early-account concentration limits and contribution handling. Recipe and threshold locks must precede viewing candidate names.
6. **Monthly acceptance.** Complete two consecutive rehearsals, confirm repeatable memo rendering, test the ticket-to-execution round trip, measure owner effort and verify retained-input backups. The CLI does not automatically perform the required external backup.
7. **Go-live review.** Research, policy, decision quality and operational gates must all pass. Until then, Aurum is not approved to direct real-money stock purchases.

## Known limits

- **PDF and citation handling:** text layers, columns, section boundaries and transposed tables can lose or misattribute evidence. Two agreeing extractions can still share the same mistake; agreement is not ground truth.
- **Partial coverage:** mandatory data gaps can block entry. Best-effort disclosure gaps are surfaced; absence of an event is not proof that nothing happened. No live general-news adapter is enabled.
- **Financial companies:** banks, NBFCs and insurers are excluded from current candidate selection. Some older demo fixtures contain a financial scoring path; they are historical display examples, not the production policy.
- **Historical fixtures:** the complete demo months were authored to exercise rendering. They retain older source labels and policy examples, and their displayed performance, calendar labels, cap values and coverage are illustrative. The generated partial fixture also predates the current live wiring.
- **Local desktop UI:** the application is deliberately designed for desktop use and runs on loopback. A phone dashboard is outside the intended scope.
- **Human participation:** some source acquisition is attended, certain official pages require manual import, and actual trades remain manual.

## Deferred

Public application hosting, a stock-count slider and broader strategy changes are outside the current delivery scope. A dedicated financial-company strategy, local-model expansion, and additional regulator adapters are not promised features of this showcase.

This page is a dated snapshot. No benchmark-beating returns, autonomous trading or production approval are implied.
