# 8 Queens Puzzle - Constraint Satisfaction Problem

This project implements the 8 Queens Puzzle using the Constraint Satisfaction Problem (CSP) approach. The game is built with **Pygame** for visualization and **python-constraint** to enforce constraints while placing the queens.

## Overview
The 8 Queens Puzzle is a classic combinatorial problem where the goal is to place 8 queens on an 8×8 chessboard such that no two queens threaten each other. This means:
- No two queens share the same row.
- No two queens share the same column.
- No two queens share the same diagonal.

## Features
- **Graphical Interface:** The board is displayed using Pygame, allowing players to click on squares to place queens.
- **Constraint Checking:** The CSP approach ensures that each queen placement follows the problem's constraints.
- **Win/Lose Detection:** The game detects when the player has either successfully placed all 8 queens correctly or has exhausted their attempts.

## Requirements
Ensure you have the following dependencies installed:
```bash
pip install pygame python-constraint
```

## How to Play
1. Run the Python script:
   ```bash
   python queens.py
   ```
2. Click on the board to place queens.
3. If a queen placement is invalid, you receive a warning. You have 3 chances.
4. Successfully place all 8 queens following the constraints to win.
5. If you place too many invalid queens, you lose the game.

## Code Structure
- **Board Initialization:**
  - The chessboard is created using Pygame.
  - Colors and grid sizes are defined.
- **CSP Implementation:**
  - Uses `python-constraint` to define and enforce constraints.
  - Ensures no two queens share a row, column, or diagonal.
- **User Interaction:**
  - Players click to place queens.
  - The program validates each move and updates the game state.
- **Win/Lose Conditions:**
  - Displays a congratulatory message if the player wins.
  - Ends the game if the player loses after 3 incorrect attempts.

## Future Improvements
- Implement an AI solver that automatically places queens.
- Add difficulty settings for different board sizes.
- Improve UI with animations and better visuals.

## License
This project is open-source and free to use. Feel free to contribute!

---
