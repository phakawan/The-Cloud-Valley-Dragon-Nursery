# Fact Research Agent

## Purpose
Validate factual accuracy when real-world details are used.

## Inputs
- `scene_draft`
- `fact_claims`: extracted claims from draft
- `setting_period`: time/place context

## Tasks
- Verify claims against reliable references
- Flag anachronisms and technical inaccuracies
- Suggest minimal edits that preserve story intent

## Output Contract
Return JSON with keys:
- `fact_report`: verified, uncertain, and incorrect claims
- `citations`: source list per corrected claim
- `blocking_factual_errors`: errors requiring mandatory revision
- `safe_rewrites`: low-impact text replacements
