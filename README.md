# Silly Pomodoro

A gamified focus timer with strict pause mechanics and collectible rewards.

## Features

- **Customizable Timer**: Set your own focus (default 31 min) and rest (default 5 min) durations
- **Strict Pause Rules**: One pause allowed per session. Second pause = session failed, no reward
- **Compounding Rest**: Skip rest periods to bank them for a longer break later
- **Three Collectibles**:
  - Sticks: Earned by completing focus sessions
  - Carrots: Earned by completing rest sessions
  - Golden Tomatoes: Earned by completing a full cycle (4 focus + 4 rest)
- **Activity Calendar**: GitHub-style grid showing your last 30 days of activity
- **Dual Themes**: Toggle between 8-bit pixel art and ASCII terminal styles
- **Offline Support**: All data stored in localStorage

## Quick Start

1. Download or clone this repository
2. Open `index.html` in your web browser
3. Click START to begin a focus session

That's it! No build tools, no dependencies, no server required.

## How It Works

### Focus Session
1. Click START to begin your focus timer
2. You get ONE pause per session - use it wisely!
3. If you pause twice, the session fails and you don't earn a reward
4. Complete the session to earn a Stick

### Rest Choice
After completing a focus session, you can:
- **Take Rest**: Start your rest timer (includes any banked time)
- **Skip Rest**: Bank your rest time for later and start another focus session

### Compounding Rest
Each skipped rest adds to your "banked rest" time. When you finally take a rest, you get all your banked time added to the base rest duration.

Example: Skip 2 rests with 5 min rest duration = your next rest is 15 minutes (5 + 5 + 5)

### Full Cycle
Complete 4 focus sessions AND 4 rest sessions to earn a Golden Tomato!

## Deploying to GitHub Pages

1. Create a new repository on GitHub
2. Push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/silly-pomodoro.git
   git push -u origin main
   ```
3. Go to repository Settings > Pages
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click Save
7. Your app will be live at `https://YOUR_USERNAME.github.io/silly-pomodoro/`

## Local Development

No build step required! Just edit `index.html` and refresh your browser.

For live reload during development, you can use any simple HTTP server:

```bash
# Python 3
python -m http.server 8000

# Node.js (npx)
npx serve

# PHP
php -S localhost:8000
```

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge).

## License

This work is licensed under [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to share and adapt this work for non-commercial purposes with attribution.

Copyright (c) 2026 SillyApps Pty
