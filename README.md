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

## **Screenshots**
### ***Initially**
![WhatsApp Image 2024-11-14 at 08 24 25_8992d88d](https://github.com/user-attachments/assets/2cda762a-d070-43b8-9809-52490e76cc5f)

### ***Turns of Player X and O Respectively***
![WhatsApp Image 2024-11-14 at 08 24 25_6f7a0b67](https://github.com/user-attachments/assets/402f2498-6d3e-40c8-a403-d85077bd2cf0)
![WhatsApp Image 2024-11-14 at 08 24 25_e12659d5](https://github.com/user-attachments/assets/03c142a1-9e64-4cc4-990f-53b2e5ef723f)
![WhatsApp Image 2024-11-14 at 08 24 24_d8213a43](https://github.com/user-attachments/assets/54160a9f-4f71-40e5-8937-6c18b9330301)
![WhatsApp Image 2024-11-14 at 08 24 27_d77f67f8](https://github.com/user-attachments/assets/8195524f-0e3f-4e88-b748-02d549dc3965)
![WhatsApp Image 2024-11-14 at 08 24 26_5654aacc](https://github.com/user-attachments/assets/a787dc15-12f5-469e-8544-2ea7fa15dad9)
![WhatsApp Image 2024-11-14 at 08 24 26_a132030e](https://github.com/user-attachments/assets/651aee56-59ea-46a3-b621-cdfb2ec58aef)

### ***Game Result-X/O Wins***
![WhatsApp Image 2024-11-14 at 08 24 26_7b872d17](https://github.com/user-attachments/assets/fe60d1d1-e00f-46a2-bc29-921bf33ce98b)

### ***Reset Game***
![WhatsApp Image 2024-11-14 at 08 24 27_884ac556](https://github.com/user-attachments/assets/432ae79a-3e98-4e59-99ec-7266e3e6ea2e)


### ***Game Result- Draw***
![WhatsApp Image 2024-11-14 at 08 24 27_2ed55f3d](https://github.com/user-attachments/assets/f1e69d1a-bb28-4194-a88e-85a5541f39aa)








---


