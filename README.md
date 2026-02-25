# Unbeatable Tic-Tac-Toe 🎮🤖

A sleek, modern, browser-based Tic-Tac-Toe game where the AI is mathematically guaranteed to never lose. Play against it and try your best to force a draw!

![Status](https://img.shields.io/badge/Status-Playable-brightgreen)
![Tech](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-blue)

Play at https://unbeatable-tictactoe.pages.dev

## ✨ Features

- **Unbeatable AI:** Powered by the Minimax algorithm. The best you can ever do is tie.
- **Zero Dependencies:** Pure HTML, CSS, and vanilla JavaScript. No frameworks, no servers, no npm installs required.
- **Modern UI:** Clean, dark-mode inspired design with smooth hover effects and responsive gameplay.
- **Plug & Play:** Runs completely locally in your web browser.

## 🚀 How to Run

Because this project is entirely self-contained in a single file, running it is incredibly simple:

1. Download or save the code as an `.html` file (e.g., `index.html`).
2. Double-click the file to open it in your default web browser (Chrome, Firefox, Safari, Edge, etc.).
3. Click any square to make your move as **X**. 

## 🧠 How the AI Works (The Minimax Algorithm)

You might be wondering: *How does it never lose?* 

The AI uses a decision rule algorithm called **Minimax**. When it is the AI's turn to move, it doesn't just look at the current board. Instead, it plays out the rest of the game in its "head" by simulating every single possible future move from both players.

1. It evaluates the end states of the game:
   - If a path leads to an **AI Win**, it gets a score of `+10`.
   - If a path leads to a **Human Win**, it gets a score of `-10`.
   - If a path leads to a **Tie**, it gets a score of `0`.
2. The AI assumes that **you** are playing perfectly and will always choose the move that minimizes the AI's score.
3. Knowing this, the AI chooses the current move that guarantees the highest possible score across all future turns.

Because Tic-Tac-Toe is a perfectly solvable game, a perfect AI playing against a perfect Human will *always* result in a Tie. 

## 🛠️ Technologies Used

- **HTML5:** Structuring the game board and UI.
- **CSS3:** Inline styling, CSS Grid for the board, and color theming.
- **JavaScript (ES6):** Game state management, UI updates, and the recursive Minimax algorithm.

## 📝 License

This project is open-source and free to use, modify, and distribute.
