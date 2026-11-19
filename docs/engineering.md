# Engineering walkthrough

## Keep the expensive work small

Universe filters, accounting gates and sector-relative scoring run before model work. Only roughly 6–8 shortlisted companies enter document interrogation. This keeps cost bounded by the shortlist rather than the listed universe. The checked-in synthetic universe has 1,104 companies; that is a fixture size, not a measured current live coverage claim.

## Separate ranking from narrative authority

The quantitative layer sets rank. A document verdict can be `PASS`, `DEMOTE`, `DISQUALIFY` or `INSUFFICIENT_DATA`; there is no promotion action. Demotions are stored beside the raw score instead of overwriting it. News opens an investigation; verified primary evidence is required for an investment consequence.

The motivation is practical: an annual report or favourable story is authored by a party with an incentive to persuade. Giving its narrative positive ranking authority would reward persuasive presentation.

## Make evidence a data contract

Qualitative findings need a document reference, page and quote. Facts have separate verification and enrichment paths, with units and missingness preserved; enriched data is sent through the accounting gates again. Unverifiable evidence is not silently treated as a clean company.

This is a safeguard, not a guarantee. PDF layout and section-location errors remain known limits, and the repeat live-document probe is still pending.

## Freeze the inputs and the record

The pipeline records retained input references and SHA-256 hashes, then seals a journal month. Once sealed, the entry cannot be extended or rewritten. The dashboard reads that record; it does not recompute past decisions from today's providers. An entry that stopped early stays explicitly partial, and a dry-run uses a separate journal root.

The mutable holdings view is separate from the sealed monthly record. No broker-order placement is implemented.

## Isolate data acquisition

Provider implementations live behind the data layer and protocol seams. Tests inject fixture sources, fake model clients and controlled document bytes. Production networking stays in the data layer, and source failures remain errors rather than becoming zero-valued financial fields.

For bulk acquisition, attended resumable runs share a request budget and cache. Provider availability remains an operational dependency.

## Evaluate the hypothesis separately

The research harness uses pre-registered rules and a limited holdout-look budget. It tests production scoring rather than a second scoring implementation, and it records evaluation runs. It acknowledges survivorship and restatement bias instead of presenting historical performance as point-in-time proof.

The initial strategy evaluation is still blocked on input-quality work. The harness is implemented; its existence is not a successful investment result.

## Verification

Verification below refers to the **private application**, not tests shipped in this public showcase. Source revision: `f2f3467`; local run date: **19 November 2026**.

| Check | Result |
|---|---|
| `uv run pytest -q` | Passed; **3,429 tests**, 2 deprecation warnings (151.49 seconds) |
| `uv run ruff check` | Passed |
| `uv run mypy src` | Passed; 110 source files checked |
| `git diff --check` | Passed |

The private repository has a GitHub Actions workflow configured to install development, PDF and web dependencies and run lint, type checking and tests on Python 3.12. This page reports the local checks above; it does not claim a fresh hosted CI run.

The suite covers pipeline behavior, data adapters, evidence validation, journal integrity, research guards and dashboard rendering. Test counts measure regression coverage, not financial performance or completion of live acceptance.

## Development process

The project uses a written architecture, explicit decisions and task cards, branch review and required checks. The owner led product decisions and directed AI coding agents, which generated the application code. This showcase describes that work without representing it as entirely hand-written implementation.
