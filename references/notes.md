# Notes / assumptions (WorldGuessr cheat mode)

## What LuckyDog wants
- Fully automated: **precise point** → auto-click on map → submit.
- Support both:
  - Singleplayer
  - Multiplayer (join via room code)
- No debrief/recap required.

## Precision strategy
- Prefer the prior approach: “directly obtained Google Maps data” to derive exact coordinates.
- If coordinates cannot be extracted reliably, fall back to clue-based country/region guessing.

## Open questions to resolve when implementing scripts
- Where exactly do coordinates come from?
  - network response payload?
  - embedded JSON on page?
  - hidden API call?
  - a map provider URL containing lat/lng?
- What UI elements are used to enter room code and join?
- What is the most stable selector for the minimap / guess map area?

## Multiplayer join
- Requirement clarified: join multiplayer via **room code input**.

## Output
- No recap/debrief required.
