# Tic-Tac-Toe AI with Adjustable Difficulty 🎮

This project implements a **Tic-Tac-Toe game with an AI opponent**. The game allows users to play against an AI that can operate in **Easy** (random moves) or **Hard** (optimal moves using the Minimax algorithm with alpha-beta pruning) difficulty levels. It features a **graphical user interface (GUI)** built using Python's `tkinter` library, making it easy and intuitive for users to enjoy the classic game.

## Features ✨

- Two Difficulty Levels:
  -Easy: AI makes random moves for a casual gaming experience.
  -Hard: AI calculates the optimal move using the Minimax algorithm with alpha-beta pruning for a challenging match.
  
- Dynamic GUI:
  -Board Background: A green, visually appealing interface.
  -Player Symbols (X and O): Styled in red for easy visibility.

- Game Flow:
  - Alternates between human and AI turns.
  - Detects win conditions, draws, and resets the game automatically.

- Customizable Settings:
  - Change difficulty easily through a menu option.

## How It Works 🧠

- Minimax Algorithm: 
  - The AI in Hard mode uses the Minimax algorithm with alpha-beta pruning to evaluate possible moves and make the optimal decision.
  
- Random Moves: 
  - In Easy mode, the AI selects moves randomly, making it suitable for beginners.

- Interactive Gameplay:
  - Users can play by simply clicking on the board cells. The game handles all turns and evaluates win conditions dynamically.

## Requirements ⚙️

- Python 3.x
- `tkinter` (comes pre-installed with Python)


