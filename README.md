# 🕹️ Math Games Arcade

> A browser-based mini-game arcade — six classic games in a single HTML file.
> No frameworks, no build step, no dependencies. Just open and play.

[![Live Demo](https://img.shields.io/badge/Play%20Now-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://infrabeam1927.github.io/COOL-MATH-GAMES/)
![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript-yellow?style=for-the-badge&logo=javascript)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-blue?style=for-the-badge)
![Single File](https://img.shields.io/badge/Single-HTML%20File-orange?style=for-the-badge)

---

## 🎮 Games

| | Game | Description | Controls |
|---|------|-------------|----------|
| 🟦 | **2048** | Slide and merge tiles until you reach 2048 | Arrow keys · Swipe |
| 🐍 | **Snake** | Eat food, grow longer, don’t bite yourself | Arrow keys · WASD · Swipe |
| 🃏 | **Memory Match** | Flip emoji card pairs in the fewest moves | Click / Tap |
| ➗ | **Math Sprint** | Rapid-fire arithmetic in 60 seconds | Number input · Enter |
| ⭕ | **Tic-Tac-Toe** | Beat the CPU — Easy or unbeatable Hard (minimax) | Click / Tap |
| 🧱 | **Breakout** | Smash all bricks; clear the board to advance levels | Arrow keys · Mouse · Touch |

---

## 🏆 Scoring

| Game | What’s Tracked | Best Score Saved |
|------|---------------|------------------|
| 2048 | Merge score (sum of merged tiles) | Highest score |
| Snake | Food eaten | Highest count |
| Memory Match | Moves to complete the board | Fewest moves |
| Math Sprint | Correct answers in 60 seconds | Highest count |
| Tic-Tac-Toe | Wins / Losses / Draws (session) | Total wins |
| Breakout | 10 pts per brick destroyed | Highest score |

All bests are saved to `localStorage` and shown on the hub card for each game.

---

## 💡 Tips & Tricks

- **2048** — Keep your highest tile in a corner and build a chain toward it. Swipe into the corner repeatedly to stay in control.
- **Snake** — Hug the walls early when the snake is short; as it grows, leave space to loop back.
- **Memory Match** — Watch the cards that flip on mismatches — they stay visible long enough to memorise.
- **Math Sprint** — Wrong answers still auto-advance after showing the correct one, so keep typing — speed beats accuracy.
- **Tic-Tac-Toe (Hard)** — The AI uses minimax and cannot be beaten. Best you can do is force a draw by taking the centre on move 1.
- **Breakout** — Hit the ball with the edge of the paddle for a steep angle; centre hits go straight up. Use angles to target remaining bricks.

---

## ✨ Features

- **Single file** — everything in one `index.html`; open locally with no server
- **Zero dependencies** — vanilla HTML, CSS, and JavaScript only
- **Dark neon theme** — near-black background with a unique neon accent per game
- **Persistent bests** — scores survive page refresh via `localStorage` (wrapped in try/catch so a blocked storage API never breaks gameplay)
- **Responsive** — works on desktop and mobile, keyboard and touch
- **Clean state** — `requestAnimationFrame` loops and `keydown` listeners are torn down on every game exit so nothing leaks between games

---

## 🚀 Running Locally

```bash
# No server needed — just open the file
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Or drag `index.html` into any modern browser tab.

---

## 🛠️ Built With

| Technology | Usage |
|------------|-------|
| HTML5 Canvas | Snake, Breakout rendering |
| CSS Grid + custom properties | Hub layout, 2048 board, Memory grid |
| CSS 3D transforms | Memory card flip animation |
| Vanilla JS | All game logic, minimax AI, localStorage |
| Web Audio API | *(not used — no audio assets required)* |

---

## 📝 Roadmap / Ideas

- [ ] Sound effects via Web Audio API (blip on score, crunch on collision)
- [ ] Animated tile transitions for 2048
- [ ] High-score leaderboard with initials (localStorage)
- [ ] Color-blind friendly theme toggle
- [ ] More games: Tetris, Wordle, Minesweeper

PRs and suggestions welcome!

---

<p align="center">
  Made with ❤️ &nbsp;·&nbsp;
  <a href="https://github.com/infrabeam1927/COOL-MATH-GAMES">View on GitHub</a> &nbsp;·&nbsp;
  <a href="https://infrabeam1927.github.io/COOL-MATH-GAMES/">Play Live</a>
</p>
