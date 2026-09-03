# Review scope
- Only report Critical and Important severity findings in Code Review on this repository. Do not report Suggestion or Quality-level findings at all.
- Report each distinct root cause once. If a response-shape change breaks its own tests, cover that in a single finding, including any note about consistency with sibling endpoints. Do not raise a second, separate finding purely comparing endpoint shapes.
- New endpoints in `app.py` must include at least one pytest test in `tests/`. Flag as Code Quality if missing. This applies only to brand-new HTTP endpoints — do not flag missing test coverage for behavior changes inside an existing endpoint (e.g. deduplication, validation tweaks).
