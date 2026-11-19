# Screenshot provenance

Captured on **19 November 2026** from the existing FastAPI/Jinja dashboard at private source revision `f2f3467`. No dashboard source or fixture journal entries were modified for these captures.

The application was served locally with:

```sh
uv run aurum serve --journal fixtures/journal --port 8427
```

Playwright captured a 1440 × 1040 desktop viewport after fonts loaded. The image files are direct browser captures; no mock screen images were generated.

| File | Route and fixture | Purpose |
|---|---|---|
| `screenshots/month.png` | `/month?period=2026-09` | Fictional buy decision, rationale and shortlist |
| `screenshots/portfolio.png` | `/portfolio?period=2026-09` | Fictional sector allocation and thesis status |
| `screenshots/company.png` | `/company?period=2026-09&ticker=MERIDCHEM` | Fictional demotion and page-cited findings |
| `screenshots/universe.png` | `/universe?period=2026-09` | Fictional ranks, factors and accounting-gate results |
| `screenshots/no-buy.png` | `/month?period=2026-10` | Fictional rejection of all candidates |
| `screenshots/incomplete-run.png` | `/run?period=2027-01` | Earlier machine-generated partial fixture, with later stages not run |

September and October are hand-authored contract examples. January is an earlier machine-generated fixture. Their calendar labels, figures and outcomes are synthetic test data; the screenshots do not document actual investing activity or future decisions. Older coverage and policy labels remain visible and should not be read as current capabilities.

Only `fixtures/journal` was used as dashboard input. No private holdings screen, production journal, live provider cache or blind research output is included. The diagram in `docs/architecture.svg` is an explanatory illustration, not an application screenshot.

The private application and fixtures are not distributed in this repository, so these commands document provenance rather than providing a runnable public demo.
