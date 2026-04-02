# ❌⭕ Event-Driven Tic Tac Toe (SDL2 in C)

A fully interactive **Tic Tac Toe game** built from scratch using **SDL2** and **SDL_ttf** in C.
This project demonstrates event-driven programming, custom UI rendering, and game logic implementation without using any high-level frameworks.

---

## 📌 Features

* 🖱️ Mouse-based interaction (hover + click)
* 🎮 Real-time game state updates
* ❌⭕ Turn-based gameplay (X vs O)
* 🏆 Winner detection (rows, columns, diagonals)
* 🤝 Draw detection
* 🔄 "Play Again" functionality
* 🎨 Custom UI rendering using SDL2
* 🖋️ Text rendering using SDL_ttf

---

## 🧱 Tech Stack

* Language: **C**
* Graphics/UI: **SDL2**
* Text Rendering: **SDL_ttf**

---

## 🏗️ Architecture

### 🔹 Core Components

* **Board System**

  * 3×3 grid using `cell` structure
  * Tracks value, hover state, click state

* **Game Logic**

  * Win detection using predefined patterns
  * Draw detection
  * Turn switching (X ↔ O)

* **UI System**

  * Custom rendering of grid and buttons
  * Hover effects
  * Dynamic text updates

* **Event Loop**

  * Handles mouse movement and clicks
  * Updates game state accordingly

---

## ⚙️ How It Works

1. Board is initialized as a 3×3 grid
2. Player clicks a cell:

   * Cell is filled with current player's symbol
   * Turn switches
3. After each move:

   * Win conditions are checked
   * Draw condition is evaluated
4. If game ends:

   * Winner or draw is displayed
   * "Play Again" button appears
5. Clicking "Play Again" resets the board

---

## ▶️ How to Run

### 🔧 Requirements

* SDL2
* SDL2_ttf
* C Compiler (GCC / MinGW / MSVC)

---

### 🛠️ Compile

```bash id="cmp1"
gcc main.c -lSDL2 -lSDL2_ttf -o tictactoe
```

---

### ▶️ Run

```bash id="run1"
./tictactoe
```

---

## 📁 Required Files

* `Arial.ttf` → Font file (must be in project directory)

---

## 🎮 Controls

* 🖱️ Click on grid to place X or O
* 🔄 Click "Play Again" after game ends

---

## ⚠️ Limitations

* No keyboard input support
* Fixed window size (not responsive)
* No AI (only two-player mode)
* Basic UI styling
* No animations or sound effects

---

## 🚀 Future Improvements

* Add single-player mode (AI using Minimax)
* Improve UI with animations
* Add sound effects
* Make window resizable
* Add score tracking system
* Enhance visual design

---

## 🧠 What I Learned

* Event-driven programming using SDL
* Game loop design and state management
* Handling user input via mouse
* Implementing game logic (win/draw detection)
* Rendering UI without frameworks
* Struct-based system design in C

---

## 🎯 Conclusion

This project demonstrates how to build an interactive game from scratch using low-level libraries.
It highlights core concepts of event handling, rendering, and game logic implementation.

---

## 📜 License

MIT License
