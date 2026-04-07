---
name: novel-writing-mvp
description: Coordinate a six-agent workflow for structured fiction writing. Use when planning, drafting, continuity-checking, and polishing chapter-based novels with consistent canon.
---

# Novel Writing MVP

Use this skill to run a deterministic 6-agent fiction pipeline that keeps story direction, character consistency, and chapter continuity aligned.

## Workflow

1. Run `Story Architect` to produce `story_bible` and `macro_arc`.
2. Run `Character Designer` using `story_bible` to produce `character_bible` and `voice_rules`.
3. Run `Plot Planner` to produce `chapter_plan` and `scene_cards`.
4. Run `Scene Writer` one scene at a time from `scene_card`.
5. Run `Continuity Checker` before any stylistic edits.
6. Run `Editor Stylist` only when continuity status is `pass`.

## Non-Negotiable Rules

- Treat `story_bible`, `character_bible`, and timeline facts as canon.
- Do not let writing agents modify canon directly; emit `change_proposal` instead.
- Block release when continuity returns any blocking issue.
- Keep outputs machine-readable JSON first; prose can be nested in fields.

## Execution Notes

- Process scenes sequentially to avoid timeline drift.
- Persist `used_facts` and `open_threads` after each scene.
- If continuity fails, revise the scene draft before editing style.

## References

- Output contracts: `references/output-schemas.md`
- Agent prompts: `../../agents/*.md`