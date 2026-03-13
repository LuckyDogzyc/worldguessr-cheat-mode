---
name: worldguessr-cheat-mode
description: WorldGuessr/GeoGuessr-style cheat mode with browser automation: extract exact coordinates when available ("Google Maps data" approach), auto-click precise point on guess map, and submit. Support Singleplayer and Multiplayer (join via room code). Use to debug UI changes (Guess disabled, minimap/map interactions, selector ref changes).
---

# WorldGuessr cheat mode

## Operating constraints
- Prefer speed + correctness: per round ≤90s unless user requests slower analysis.
- Avoid reckless clicks (e.g., clicking ocean) unless explicitly requested.
- If UI changed / controls missing: capture screenshot + report exact blocker.

## Workflow

### Mode A — Precise auto-guess (preferred)
Use this when we can extract the **exact coordinates** (the previous “directly obtained Google Maps data” approach).

1) Open/reuse tab: https://www.worldguessr.com
2) Choose mode:
   - **Singleplayer**: start a game
   - **Multiplayer**: join via **room code**
3) Each round:
   - Extract exact lat/lng (if available)
   - Open/activate the guess map
   - Click the exact point and submit Guess

### Mode B — Clue-based fallback
Use only if exact coordinates are not available.

1) Read clues quickly (language/script → road markings → driving side → signs → landscape)
2) Pick best location, click on land, submit Guess

## Common UI issues
- **Guess disabled**: try expanding minimap / clicking mini map area to activate; avoid random clicks.
- **Stall / selector timeout**: take screenshot, note current URL, and fall back to manual navigation.

## Notes
- Skill authoring reference (for future skill iteration): https://github.com/mgechev/skills-best-practices
