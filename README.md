# worldguessr-cheat-mode

WorldGuessr/GeoGuessr-style **cheat mode** workflow skill for Clawdbot/OpenClaw.

## Install (from GitHub)

On the target OpenClaw machine:

```bash
cd /root/clawd/skills/public
git clone https://github.com/LuckyDogzyc/worldguessr-cheat-mode.git worldguessr-cheat-mode
clawdbot gateway restart
```

## Update

```bash
cd /root/clawd/skills/public/worldguessr-cheat-mode
git pull
clawdbot gateway restart
```

## Quick trigger

In chat with OpenClaw:

- Multiplayer:
  - “Use `worldguessr-cheat-mode` in clawd browser; join room code XXXX; each round try extract exact lat/lng → open guess map → click → Guess; fallback to clue-based.”

- Singleplayer:
  - “Use `worldguessr-cheat-mode` in clawd browser; start a game; per round: extract lat/lng → click map → Guess; fallback to clue-based.”
