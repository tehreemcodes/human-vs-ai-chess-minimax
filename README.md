# ♟️ Human vs AI Chess Game — Minimax Algorithm with GUI

## 🎯 Objective

This project implements a simplified **Human vs AI Chess Game** in Python using the **Minimax Algorithm** (with optional Alpha-Beta Pruning) as part of our Spring 2025 Artificial Intelligence course.

It includes a complete object-oriented design, supports standard chess rules and mechanics, and features a GUI for interaction.

---

## 📦 Features

- ✅ Turn-based gameplay (Human vs AI)
- ✅ Full 8x8 Chessboard with GUI (Tkinter)
- ✅ Standard piece movement and capturing
- ✅ Minimax AI (with optional Alpha-Beta Pruning)
- ✅ Special moves:
  - Castling (Kingside and Queenside)
  - Pawn Promotion
  - En Passant
- ✅ Check, Checkmate, and Stalemate detection
- ✅ Input-based move system (e.g., `e2e4`)
- ✅ AI Evaluation based on:
  - Material advantage
  - King safety
  - Positional heuristics

---

## 🧠 AI: Minimax Overview

The **AIPlayer** uses the **Minimax algorithm** to simulate moves up to a fixed depth and evaluates board states based on:
- Material value of pieces
- Safety of the king
- Central control and piece mobility

Alpha-Beta pruning is optionally enabled for optimization.

---

## 🏗️ Class Structure

| Class         | Responsibility |
|---------------|----------------|
| `ChessGame`   | Game loop, turns, endgame logic |
| `Board`       | Manages 8x8 grid and pieces |
| `Move`        | Encapsulates a chess move |
| `Piece`       | Abstract base for all pieces |
| `King`, `Queen`, `Rook`, `Bishop`, `Knight`, `Pawn` | Implement piece-specific movement logic |
| `Player`      | Abstract class for players |
| `HumanPlayer` | Takes move input via GUI |
| `AIPlayer`    | Makes decisions using Minimax |
| `Evaluation`  | Contains heuristics used by AI |

---

## 🖥️ GUI Features

- Built with **Tkinter**
- Input move in formats like `e2e4`
- Visual board with Unicode chess symbols
- Status display: AI Thinking, Checkmate, etc.
- Highlighting valid moves (optional)

---

## 📂 Folder Structure

human-vs-ai-chess-minimax/
├── chess-pieces/
│ ├── Bblack.png
│ ├── Bwhite.png
│ ├── Kblack.png
│ ├── Kwhite.png
│ ├── Nblack.png
│ ├── Nwhite.png
│ └── Pblack.png
│ ├── Pwhite.png
│ ├── Qblack.png
│ ├── Qwhite.png
│ ├── Rwhite.png
│ └── Rblack.png
├── chess.ipynb # Jupyter notebook 
├── Report.pdf # Report with explanations and test cases
├── README.md # Project overview


---

## 🖥️ GUI Overview

- Built with **Tkinter**
- Board visually displays pieces using images or Unicode characters
- Move input via textbox (e.g., `e2e4`)
- Optional: Highlight valid moves
- Game status updates (e.g., "Checkmate", "AI is thinking...")

---

## 📚 Minimax with Alpha-Beta Pruning

The **Minimax algorithm** is implemented in the `AIPlayer` class to evaluate future game states up to a fixed depth (2–3 levels).

### Evaluation Function Includes:

- 🔢 Material count (piece weights)
- 🛡️ King safety heuristics
- ♟️ Central control and piece mobility

**Alpha-Beta Pruning** reduces the number of nodes evaluated by pruning irrelevant branches.

---

## 🧩 Class Design

| Class Name       | Description |
|------------------|-------------|
| `ChessGame`      | Main game loop and state transitions |
| `Board`          | Represents the board and piece positions |
| `Move`           | Encapsulates a chess move |
| `Piece`          | Abstract base class for all pieces |
| `King`, `Queen`, etc. | Implement movement logic for each piece |
| `Player`         | Abstract class for player types |
| `HumanPlayer`    | Allows human move input via GUI |
| `AIPlayer`       | Implements Minimax (with pruning) |
| `Evaluation`     | Evaluates board position for AI decisions |

---

## 📋 How to Run

1. **Clone the repo**
```bash
git clone https://github.com/tehreemcodes/human-vs-ai-chess-minimax.git
cd human-vs-ai-chess-minimax

