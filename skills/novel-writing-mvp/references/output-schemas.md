# Output Schemas

## story_bible
```json
{
  "title_seed": "string",
  "logline": "string",
  "theme": "string",
  "tone": "string",
  "premise": "string",
  "ending_note": "string"
}
```

## character_profile
```json
{
  "name": "string",
  "role": "protagonist|antagonist|support",
  "goal": "string",
  "fear": "string",
  "wound": "string",
  "arc": "string",
  "voice_signature": ["string"]
}
```

## scene_card
```json
{
  "chapter": 1,
  "scene": 1,
  "pov": "string",
  "objective": "string",
  "conflict": "string",
  "outcome": "string",
  "reveal": "string",
  "hook": "string",
  "continuity_flags": ["string"]
}
```

## continuity_report
```json
{
  "status": "pass|revise",
  "blocking_issues": ["string"],
  "non_blocking_issues": ["string"],
  "suggested_fixes": ["string"]
}
```
