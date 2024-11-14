# CSE3218_Assignments

# SwiftUI Tic Tac Toe Game

Welcome to the **SwiftUI Tic Tac Toe Game**! This project is a fun, interactive Tic Tac Toe game built entirely in SwiftUI. Players take turns as "X" and "O," and the game includes winner detection, draw handling, and a smooth UI with animations.

---

##  **Project Overview**

This SwiftUI project features a **Tic Tac Toe game** where:
- Players X and O take turns marking cells.
- The game detects wins and draws automatically.
- The UI provides immediate feedback with colors and animations.

---

##  **Key Features**

### **Player Turns and Color Coding**
- The game alternates turns between **Player X** (Red) and **Player O** (Blue).
- The current player’s turn is displayed at the top in their respective color.

### **Winner Detection & Highlighting**
- The game automatically checks for wins after every move.
- Winning cells are highlighted with a scale animation to celebrate the win.
- A message displays the winning player when a win is detected.

### **Draw Detection**
- If all cells are filled without any player winning, the game ends in a draw.
- A message is displayed indicating a draw.

### **Animations**
- Winning cells have a smooth scale animation, and winning/draw messages appear with a fade-in effect.

### **Reset Button**
- A button is provided at the bottom to reset the game, clearing the board and restarting the game state.

---

##  **Code Structure**

The project consists of the following key components:

### **ContentView.swift**
- **Player Enum**: Defines the `Player` type with cases `.x` and `.o` representing "X" and "O".
- **@State Properties**:
  - `currentPlayer`: Tracks the current player.
  - `cells`: Holds the game board as a 3x3 grid of optional `Player` values.
  - `winner` and `isDraw`: Track the winner and whether the game ended in a draw.
  - `winningCells`: Holds the positions of winning cells for highlighting.
- **UI**:
  - The game board is created with a nested `ForEach` loop, with buttons for each cell.
  - Cell colors change dynamically based on the player occupying them.
  - Messages and a reset button are displayed conditionally based on game state.
- **Functions**:
  - `makeMove(row:column:)`: Handles moves by updating the cell, changing players, and checking for a winner.
  - `checkWinner()`: Checks rows, columns, and diagonals for a winning combination.
  - `resetGame()`: Resets the game state for a new round.

---

##  **UI and Game Flow**

The game consists of a 3x3 grid with interactive cells:

1. **Colorful Gameplay**: Player X uses red, and Player O uses blue.
2. **Responsive Animations**: Winning cells scale up, and messages animate smoothly.
3. **Status Messages**: Displays the current player’s turn, win messages, or draw message.

---


