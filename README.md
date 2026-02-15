# Emoji Game

A memory game built with React where the goal is to click each emoji exactly once.

## Gameplay
- Click any emoji card to score a point.
- The emojis are shuffled after every click.
- Clicking an already selected emoji ends the game.
- If you click all unique emojis without repeating, you win.
- `Top Score` tracks your best score across rounds.

## Tech Stack
- React 19
- JavaScript (ES6+)
- CSS3
- Create React App (`react-scripts` 5)
- React Testing Library + Jest DOM

## Project Structure
```text
src/
  Components/
    EmojiCard/
    EmojiGame/
    NavBar/
    WinOrLoseCard/
  App.js
  index.js
```

## Getting Started
### Prerequisites
- Node.js (LTS recommended)
- npm

### Installation
```bash
npm install
```

### Run Locally
```bash
npm start
```
Open `http://localhost:3000` in your browser.

## Available Scripts
- `npm start` - Runs the app in development mode.
- `npm test` - Launches the test runner.
- `npm run build` - Builds the app for production.
- `npm run eject` - Ejects Create React App configuration (one-way action).

## How It Works
- `EmojiGame` manages game state (`clickedEmojisList`, `isGameInProgress`, `topScore`).
- `EmojiCard` renders each emoji button and sends click events to the game.
- `NavBar` displays current score and top score during gameplay.
- `WinOrLoseCard` displays the result screen and allows restarting.

## Future Improvements
- Add difficulty levels.
- Add score persistence using local storage.
- Add animations and sound effects.
