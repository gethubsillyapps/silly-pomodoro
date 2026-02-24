# Silly Pomodoro

## What It Is

Silly Pomodoro is a Pomodoro-style focus timer with a simple belief: the best reward for focusing is watching something grow. Complete focus sessions, earn collectibles, and tend to a pixel-art garden that resets fresh each day.

The timer mechanics are intentionally strict. One pause per session. Pause twice and the session fails. This keeps the reward meaningful.

## Features

### Timer
- **Customisable durations**: Set your own focus and rest times (default 31 min focus / 5 min rest)
- **Strict pause rules**: One pause allowed per session — second pause fails the session
- **Compounding rest**: Skip rest periods to bank them; take them all at once later as a longer break
- **Quick Timer widget**: A side stopwatch/countdown for tracking anything outside the main session

### Collectibles
Earned by completing sessions. Each has a use in the garden crafting system.

| Collectible | Earned by | Garden use |
|---|---|---|
| Sticks | Completing a focus session | Craft a raised garden bed |
| Carrots | Completing a rest session | Plant a carrot in your garden |
| Golden Tomatoes | Completing a full cycle (4 focus + 4 rest) | Plant a tomato; clear failed sessions |

### Garden
A pixel-art plant grows in the left panel as you focus. It passes through 8 stages — from an empty pot to a harvest-ready plant — driven by your focus sessions. The garden resets each morning, fresh for the day.

- **Gifted starter pot**: No barrier on day one — the pot is yours from the start
- **Plant choice**: Spend a Carrot to grow a carrot, or a Golden Tomato to grow a tomato
- **Today's harvest**: Completed cycles drop into a visible basket
- **Total plants grown**: An all-time counter across every day

### Themes
- **Zen**: Warm gradient background, glassmorphism cards, serif headings, pixel-art collectible icons
- **ASCII**: Green-on-black terminal style, monospace font, solid backgrounds

### Activity Calendar
GitHub-style grid showing your last 30 days of sessions at a glance.

## How It Works

### Focus Session
1. Click START — the timer counts down and your garden begins to grow
2. You get **one pause** per session — use it if you need it
3. Pause a second time and the session fails (no reward, a grey mark in your garden)
4. Complete the session to earn a **Stick** and advance your plant

### After a Focus Session
You can:
- **Take Rest** — start your rest timer and earn a Carrot on completion
- **Skip →** — bank your rest time and go straight into another focus session

### Full Cycle
Complete 4 focus sessions and 4 rest sessions to earn a **Golden Tomato** and see it drop into your garden basket.

### Compounding Rest
Each skipped rest adds to your banked time. When you finally take a rest, all banked time is added together.

Example: Skip 2 rests with a 5-minute rest duration → your next rest is 15 minutes (5 + 5 + 5).

## Roadmap

The garden crafting system is being built in phases:

- **Phase 1** ✓: Planting choice (carrot or tomato), gifted pot onboarding, today's harvest basket, total plants counter
- **Phase 2** ✓: Raised garden bed upgrade (craft with Sticks), carrot vs tomato plant pixel art
- **Phase 3** ✓: Grey tomato removal — spend a Golden Tomato to clear failed sessions
- **Phase 4**: Greenhouse upgrade — plants survive the daily reset
- **Future**: Inventory persistence with accounts, multiplayer garden visits

## Quick Start

1. Open [gethubsillyapps.github.io/silly-pomodoro](https://gethubsillyapps.github.io/silly-pomodoro/) in any browser
2. Click START
3. That's it

Or run locally:

```bash
git clone https://github.com/gethubsillyapps/silly-pomodoro.git
cd silly-pomodoro
open index.html
```

No build tools, no dependencies, no server required.

## Deploying Your Own Copy

1. Fork this repository
2. Go to Settings > Pages
3. Under Source, select "Deploy from a branch"
4. Select `main` branch and `/ (root)` folder
5. Your copy will be live at `https://YOUR_USERNAME.github.io/silly-pomodoro/`

## Browser Support

Works in all modern browsers. Optimised for mobile Safari and Chrome on iOS.

## License

[Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/)

You are free to share and adapt this work for non-commercial purposes with attribution.

Copyright (c) 2026 SillyApps Pty
