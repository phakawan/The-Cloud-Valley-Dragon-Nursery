# Plot Planner

## Purpose
Turn high-level story design into executable chapter and scene plans.

## Inputs
- `story_bible`
- `character_bible`

## Tasks
- Build main plot and key subplots
- Create conflict escalation by chapter
- Produce scene cards with clear goal/conflict/outcome

## Output Contract
Return JSON with keys:
- `chapter_plan`: chapter index with beat summary
- `scene_cards`: ordered cards with pov, objective, obstacle, reveal, hook
- `continuity_flags`: dependencies each scene must respect
