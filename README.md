# 🎮 Classical Games in C++: Tic Tac Toe & Chess

Welcome to the **Classical Game Suite**, a C++ project featuring two timeless board games: **Tic Tac Toe** and **Chess**. This project is a demonstration of **Object-Oriented Programming (OOP)** in C++, combined with a **simple graphical user interface (GUI)** using **SFML**. Users can choose which game to play through a game launcher menu on startup.

---

## 🧠 Project Overview

This project was created to:
- Practice and demonstrate object-oriented programming in C++
- Learn GUI programming using SFML
- Build fully functional board games with clear game rules
- Create a game launcher interface to choose between games

Both games are interactive and include visual feedback using mouse input.

---

## 🎯 Features

### 🕹 Game Launcher
- Clean and user-friendly **startup menu**
- Lets the player choose between:
  - `Play Tic Tac Toe`
  - `Play Chess`

### ✅ Tic Tac Toe
- 3x3 graphical grid
- Two-player gameplay (no AI)
- Detects win, draw, and invalid moves
- Mouse click-based interaction

### ♟ Chess
- Standard 8x8 board layout
- Implements complete chess rules:
  - Castling
  - En passant
  - Pawn promotion
  - Check, checkmate, and stalemate
- Turn-based gameplay with GUI interaction
- Move validation and rule enforcement

---

## 🛠 Technologies Used

- **C++17**
- **SFML (Simple and Fast Multimedia Library)**:
  - Graphics
  - Window & Event handling
- **Object-Oriented Design**:
  - Encapsulation
  - Inheritance
  - Polymorphism
  - Class hierarchies for game objects

---

## 📁 Project Structure
Cpp-Classical-Games/
├── assets/ # Fonts and images for GUI
├── src/
│ ├── tictactoe/ # Tic Tac Toe logic and UI
│ │ ├── Game.cpp
│ │ └── Game.hpp
│ ├── chess/ # Chess logic and UI
│ │ ├── Game.cpp
│ │ └── Game.hpp
│ └── main.cpp # Entry point with game launcher
├── CMakeLists.txt # Optional build configuration
└── README.md # You're here!


---

## 🚀 Getting Started

### 🔧 Prerequisites

- C++ compiler (g++ or MSVC)
- SFML (version 2.5 or later)

Download SFML from:  
🔗 https://www.sfml-dev.org/download.php

Or follow setup instructions:  
🔗 https://www.sfml-dev.org/tutorials/

---

### 💻 Build Instructions

#### ✅ Method 1: Using g++
```bash
g++ -std=c++17 src/main.cpp src/chess/*.cpp src/tictactoe/*.cpp \
-I<path_to_sfml>/include -L<path_to_sfml>/lib \
-lsfml-graphics -lsfml-window -lsfml-system -o classical_games

./classical_games
