# Canvas Pong

A robust, physics-based implementation of the classic Pong arcade game, built entirely using **HTML5 Canvas** and **Vanilla JavaScript**. 

This project demonstrates a clean separation between the game engine and game logic, featuring a double-buffered rendering system and an adaptive AI that reacts to player performance.

## 🎮 Key Features

* **Game Modes:** Supports Single Player (vs AI), Local Two Player, and a self-playing Demo mode.
* **Adaptive AI:** The computer opponent adjusts its reaction time and error margin dynamically based on the score difference to maintain competitive gameplay.
* **Physics Engine:** Includes ball acceleration over time and "spin" effects based on paddle movement during impact.
* **Visual Debugging:** Optional settings to visualize the AI's prediction algorithm and the ball's tracking "footprints."
* **Performance:** Utilizes a custom game loop with double buffering to ensure smooth rendering without flickering.

## 🛠️ Technical Overview

The codebase is structured into three main components:

1.  **`game.js` ( The Engine):** A generic game runner that handles the game loop, input events, custom event binding, and canvas rendering contexts (front and back buffers).
2.  **`pong.js` (The Logic):** Contains the specific rules for Pong, including collision detection (axis-aligned bounding boxes), vector mathematics for ball trajectory, and the finite state machine for the AI.
3.  **`index.html`:** The entry point that initializes the canvas and binds UI elements to the game settings.

## 🚀 How to Run
Since this project relies on standard HTML5 and JavaScript with no external dependencies or build tools, it is incredibly easy to run:
1.  Clone or download this repository.
2.  Open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge).
3.  Enjoy the game!

## ⚙️ Configuration
You can toggle the following settings directly from the sidebar menu:
* **Sound:** Enable/Disable audio effects.
* **Stats:** Show FPS and rendering time (ms).
* **Footprints:** Visualize the ball's recent path.
* **Predictions:** Visualize where the AI calculates the ball will land.

## 📝 Credits
Based on the original JavaScript Pong implementation by [Jake Gordon](https://jakesgordon.com/writing/javascript-pong/).
