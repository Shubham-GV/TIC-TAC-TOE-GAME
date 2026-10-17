# Tic-Tac-Toe

A single-file Tic-Tac-Toe game for the browser. Just HTML, CSS and JavaScript: no frameworks, no build step, no dependencies.

**Live demo:** _add your GitHub Pages link here_

## Features

- **Two modes:** 2 Players, or vs Computer
- **Three difficulty levels:**
  - **Easy:** picks any free square
  - **Medium:** wins if it can, blocks you if it must, otherwise plays randomly
  - **Hard:** perfect play using the Minimax algorithm, so it can't be beaten
- Play as **X** (goes first) or **O**
- Score tracking, winning-line highlight, and a responsive layout for phones

## Run it

Download or clone the repo and open `index.html` in any browser.

```bash
git clone https://github.com/<your-username>/tic-tac-toe.git
cd tic-tac-toe
# then double-click index.html
```

## How the Hard AI works

The computer uses **Minimax**: it explores every way the rest of the game could go, assumes you will play your best, and picks the move with the best guaranteed outcome. Faster wins and slower losses score higher, so it finishes games instead of dragging them out. Positions are cached in a `Map`, so each one is only evaluated once.

## Ideas for improvement

- Bigger boards (4x4, 5x5) with a configurable win length
- Sound effects and win animations
- Undo last move
- Save the scoreboard in `localStorage`

## License

MIT
