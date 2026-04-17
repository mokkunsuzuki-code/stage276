# Stage276: CI Evidence Automation

## Overview

Stage276 automates CI evidence generation for QSP.

This stage bundles:

- run information
- artifact information
- verification results
- summary output

using GitHub Actions.

## Files

- `.github/workflows/stage276-ci-evidence.yml`
- `docs/stage276_ci_evidence.md`
- `tools/build_stage276_summary.py`
- `tools/verify_stage276_evidence.py`
- `out/ci_evidence/stage276_summary.json`
- `out/ci_evidence/verify_stage276_result.json`

## What This Stage Adds

- automatic CI evidence generation
- automatic verification output
- artifact preservation in GitHub Actions
- structured summary for later review

## Local Run

Run locally:

```bash
python3 tools/build_stage276_summary.py
python3 tools/verify_stage276_evidence.py
Generated Evidence
out/ci_evidence/stage276_summary.json
out/ci_evidence/verify_stage276_result.json
Security Meaning

Before this stage, trust depended on definitions and policy.

Stage276 adds automated execution evidence.

This means the project can now show not only how verification should work,
but also that it was executed in CI and preserved as artifacts.

Limitations

This stage does NOT yet prove external independent re-execution.

License

MIT License
