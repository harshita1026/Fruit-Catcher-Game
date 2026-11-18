# 🍎 Fruit Catcher – 2D Arcade Game

## Project Overview

**Fruit Catcher** is a customizable 2D arcade game developed using Python and Pygame. The player controls a basket to collect falling fruits, earn points, collect bonus items, and avoid bombs.

The game demonstrates multimedia programming concepts such as animation, keyboard interaction, collision detection, score management, game states, and difficulty progression.

## Technologies Used

- **Programming Language:** Python
- **Game Library:** Pygame
- **Modules:** Random, Sys, OS
- **IDE:** Visual Studio Code

## Features

- Start screen with game instructions
- Basket movement using keyboard
- Falling fruit animation
- Normal fruit collection
- Golden apple bonus
- Bomb hazard
- Score management
- Three-life system
- 60-second countdown timer
- Increasing difficulty
- Pause and resume functionality
- Game-over screen
- Restart option
- Graphics created using Pygame drawing functions
- Optional sound effects and background music

## Game Rules

1. Press Enter to start the game.
2. Move the basket using the Left and Right arrow keys.
3. Catch normal fruits to earn points.
4. Catch golden apples to earn bonus points.
5. Avoid bombs because they reduce your lives.
6. The game becomes more difficult as time progresses.
7. The game ends when all lives are lost or the timer reaches zero.
8. Restart the game to play again.

## Scoring System

| Object | Effect |
|---|---|
| Normal Fruit | +10 Points |
| Golden Apple | +30 Points |
| Bomb | −1 Life |

## Controls

| Key | Action |
|---|---|
| Enter | Start the game |
| Left Arrow | Move basket left |
| Right Arrow | Move basket right |
| P | Pause / Resume |
| R | Restart after Game Over |
| Esc | Exit from Game Over screen |

## Customization

The game includes the following functional customizations:

- **Golden Apple Bonus:** Golden apples provide 30 points instead of the normal fruit's 10 points.
- **Limited Lives:** The player starts with 3 lives. Bomb collision decreases one life.
- **Increasing Difficulty:** Object speed increases as gameplay time progresses.
- **Dynamic Objects:** Fruits, golden apples and bombs are generated randomly.

## Installation

### 1. Install Python

Download and install Python from:

https://www.python.org/downloads/

### 2. Install Pygame

Open the terminal and run:

```bash
pip install pygame
```

### 3. Download or Clone the Project

Download the project files or clone the repository.

### 4. Run the Game

Open the project folder in VS Code and execute:

```bash
python main.py
```

## Project Structure

```text
Fruit_Catcher_Game/
│
├── main.py
├── assets/
│   ├── collect.wav
│   ├── bomb.wav
│   └── background_music.mp3
│
├── screenshots/
│   ├── start_screen.png
│   ├── gameplay.png
│   └── game_over.png
│
└── README.md
```

*Sound files and screenshots are optional and should be included if available.*

## Game Logic

The game follows these basic steps:

1. Initialize Pygame and create the game window.
2. Display the start screen.
3. Start the game when the player presses Enter.
4. Generate falling objects at random positions.
5. Move the basket according to keyboard input.
6. Update object positions to create animation.
7. Detect collisions between the basket and objects.
8. Update score or lives according to the collision.
9. Increase difficulty over time.
10. Check the timer and remaining lives.
11. Display the Game Over screen when the game ends.
12. Allow the player to restart.

## Collision Detection

Collision detection is implemented using Pygame's `colliderect()` method.

```python
if player.colliderect(rect):
    # Handle collision
```

This method checks whether the player's rectangular area overlaps with the falling object's rectangular area.

When a collision occurs, the game checks the object type and updates the score or lives accordingly.

## Learning Outcomes

Through this project, I learned:

- How to create a 2D game using Python and Pygame
- How to create a graphical game interface
- How to handle keyboard events
- How to implement animation
- How to detect collisions
- How to manage score, timer and lives
- How to implement game states
- How to create game difficulty progression
- How to restart a game without closing the application

## Author

**Student Project**  
Multimedia Systems Lab – Lab Test 2

## License

This project was developed for academic and educational purposes.
