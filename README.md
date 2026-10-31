# Tic-Tac-Toe CLI with Smart AI

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-3776AB.svg?logo=python&logoColor=white)](https://python.org)
[![Interface: CLI](https://img.shields.io/badge/Interface-CLI%20%2F%20Terminal-black.svg)](#)
[![AI Opponent](https://img.shields.io/badge/AI-Rule--Based%20Heuristic-success.svg)](#)

English | [فارسی](README_FA.md)

A classic **Tic-Tac-Toe** (دوز) game designed for the command-line interface, written in **Python**. It features a smart, defensive computer opponent with look-ahead logic and colorized terminal output.

---

## 🌟 Overview

Tic-Tac-Toe is a timeless zero-sum strategy game played on a 3x3 grid. While trivial for humans, building a competent terminal opponent requires algorithmic decision-making.

This Python implementation equips the computer opponent with a layered heuristic strategy:
1. **Immediate Win**: The AI checks if any available move immediately wins the game.
2. **Defensive Block**: If the player is one move away from winning, the AI detects the threat and blocks that space.
3. **Strategic Positioning**: If no immediate win or block is required, the AI prioritizes high-value tactical squares (corners $\rightarrow$ center $\rightarrow$ sides).

---

## ✨ Features

- **Heuristic AI Engine**: Smart look-ahead and defensive move counteraction.
- **Rich Terminal Styling**: Color-coded markers using `termcolor` (Red for Player `[X]`, Blue for Computer `[O]`, Green for victory, Yellow for defeat).
- **Interactive Move Selection**: Clean 1–9 numeric keypad layout representing the board tiles.
- **Defensive Move Validation**: Prevents overwriting already played squares or entering out-of-bounds numbers.

---

## 🎮 How to Play

The board tiles are numbered **1** through **9**:

```text
[1] [2] [3]
[4] [5] [6]
[7] [8] [9]
```

1. You play as **X** (Red) and always make the first move.
2. The computer responds as **O** (Blue).
3. Enter the number corresponding to an unoccupied cell when prompted.
4. The first player to align 3 consecutive marks horizontally, vertically, or diagonally wins!

---

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- `termcolor` library

### Installation & Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/soheilabbasnia/tic-toc-toe.git
   cd tic-toc-toe
   ```

2. **Install dependency**:
   ```bash
   pip install termcolor
   ```

3. **Start the game**:
   ```bash
   python3 program.py
   ```

---

## 📁 Project Structure

```text
tic-toc-toe/
├── program.py              # Main game loop, board rendering, and AI logic
├── LICENSE                 # MIT License
└── README.md               # English documentation
```

---

## 🤝 Contributing

Contributions, Minimax algorithm implementations, and multiplayer mode additions are welcome!
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/minimax-ai`).
3. Commit your changes (`git commit -m 'Implement unbeatable Minimax AI'`).
4. Push to the branch (`git push origin feature/minimax-ai`).
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
Free and open-source for personal and educational use.
