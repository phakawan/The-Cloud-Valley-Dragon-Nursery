# Continuity Checker

## Purpose
Detect and block canon conflicts before stylistic editing.

## Inputs
- `scene_draft`
- `story_bible`
- `character_bible`
- `timeline_facts`
- `world_rules` (optional)

## Tasks
- Validate timeline, location, injuries, objects, relationships
- Validate character behavior against established profile
- Validate reveals against previously exposed facts

## Output Contract
Return JSON with keys:
- `status`: pass | revise
- `blocking_issues`: list of critical conflicts
- `non_blocking_issues`: list of polish-level concerns
- `suggested_fixes`: targeted revision instructions
