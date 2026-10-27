# 2048 Game

A classic, fully functional 2048 puzzle game implemented in vanilla JavaScript using an object-oriented programming approach. This project features robust game logic encapsulated in a core class, smooth keyboard event handling, dynamic DOM rendering and score tracking.

## Live Preview

[2048 Game Demo](https://VladyslavL02.github.io/2048_game/)

## Game Reference

[Original 2048 Game](https://play2048.co/)

## Technologies Used

**Core**

- JavaScript (ES6+) – Object-oriented game logic, array manipulation, and event handling
- HTML5 – Semantic structure and responsive game board layout
- SCSS – Modular styling, BEM architecture, and dynamic cell state classes
- Parcel – Asset bundling, SCSS compilation, and local development server

**Code Quality & Testing**

- ESLint & Prettier – Code linting and automated formatting
- Stylelint – SCSS syntax validation

**Deployment & Hosting**

- GitHub Pages – Public hosting and live preview deployment

## Getting Started

To set up the project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/VladyslavL02/2048_game.git
   cd 2048_game
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the project locally:

   ```bash
   npm start
   ```

## Features

- **Core Game Logic (`Game` class):** Encapsulated state management handling initialization, resets, score calculation, win/loss status tracking, and directional tile sliding and merging (up, down, left, right).
- **Random Tile Spawning:** Automatically spawns a `2` (90% probability) or `4` (10% probability) in a random empty cell after every valid move.
- **Interactive Keyboard Controls:** Seamlessly responds to arrow key inputs (`ArrowUp`, `ArrowDown`, `ArrowLeft`, `ArrowRight`) to slide and merge matching numbers.
- **Score Tracking:** Dynamically updates and increments the score based on the sum of all merged tiles during a move.
- **Game State Modals:** Displays distinct messages and UI triggers for winning (reaching the 2048 tile) and game over scenarios (no available moves left).
- **Dynamic UI Adaptation:** Toggles button states between "Start" and "Restart", hides start overlays, and maps numerical values to corresponding CSS modifier classes (`field-cell--%cell_value%`).
