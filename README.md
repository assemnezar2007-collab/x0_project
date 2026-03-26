# 🎮 Tic Tac Toe Game (C++)

## 📌 Overview

This project is a simple **Tic Tac Toe game** implemented in C++.
Two players (`X` and `O`) take turns playing on a 3×3 board until one wins or the game ends in a draw.

---

## 🧠 Features

* Two-player mode (Player X vs Player O)
* Input validation (prevents invalid moves)
* Win detection (rows, columns, diagonals)
* Draw detection (when the board is full)
* Clean console-based UI

---

## 🕹️ How the Game Works

1. The game starts with Player **X**.
2. Players take turns entering:

   * Row (1–3)
   * Column (1–3)
3. The game checks:

   * If a player wins → game ends
   * If the board is full → draw
4. Otherwise, the turn switches to the next player.

---

## 🔄 Game Logic

### ✔️ Switching Players

```cpp
player = (player == 'X') ? 'O' : 'X';
```

---

### ✔️ Win Conditions

The game checks:

* All rows
* All columns
* Both diagonals

---

### ✔️ Draw Condition

```cpp
if (isfull(board)) {
    // No empty spaces → Draw
}
```

---

## 🧩 Functions Explained

### 🔹 `displayboard`

Prints the current state of the board in a formatted way.

---

### 🔹 `check_win`

Checks if the current player has:

* 3 in a row
* 3 in a column
* 3 in a diagonal

Returns:

* `true` → player wins
* `false` → no win yet

---

### 🔹 `isfull`

Checks if the board is full.

Returns:

* `true` → no empty spaces (Draw)
* `false` → still moves available

---

## 🚀 How to Run

### 1. Compile

```bash
g++ main.cpp -o game
```

### 2. Run

```bash
./game
```

---

## ⚠️ Notes

* Input must be within range (1–3)
* Cannot overwrite an occupied cell
* Game ends immediately after a win or draw

---

## 💡 Future Improvements

* Add AI player 🤖
* Add score tracking
* Improve UI design
* Add replay option

---

## 👨‍💻 Author

**Assem Albon**

---

## 🎯 Key Takeaway

> This project demonstrates basic concepts of:

* Arrays
* Loops
* Functions
* Conditionals
* Game logic design

---

🔥 Simple
