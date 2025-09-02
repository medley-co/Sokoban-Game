# Extra Fancy Sokoban

Sokoban is a Python puzzle game where players push crates (C) to goals (G) while managing moves and strength. Collect potions (S, M, F) to gain power-ups. Navigate mazes (W = walls, = floor) and solve puzzles to win!

---

## Features
- Classic Sokoban puzzle mechanics (push crates onto goals).
- Player stats tracking: strength, moves remaining, and money.
- Collect coins and purchase items in the in-game shop:
  - Strength Potion (+2 strength)
  - Move Potion (+5 moves)
  - Fancy Potion (+2 strength, +2 moves)
- Undo functionality to revert your last move.
- Win & lose conditions with replay option.
- Polished Tkinter GUI with images for tiles, entities, and a game banner.

---

## Project Structure
```
.
├── sokoban.py        # Main game controller and entry point
├── model.py          # Core Sokoban game logic
├── support.py        # General helpers & constants
├── gui_support.py    # GUI/Tkinter support classes
├── images/           # Sprite images for tiles, entities, and banner
├── maze_files/       # Maze layouts (text files)
```

---

## How to Play
1. Run the game:
   ```bash
   python sokoban.py
   ```

2. Use the keyboard to move:
   - **W** → Up
   - **S** → Down
   - **A** → Left
   - **D** → Right
   - **U** → Undo last move

3. Push crates (`C`) onto goal tiles (`G`).
4. Collect coins (`$`) to buy potions in the Shop.
5. Win by filling all goals, or lose when you run out of moves.

---

## Requirements
- Python 3.10+  
- Tkinter (bundled with Python)  
- Pillow (`pip install pillow`)

---

## Maze File Format
Each maze file in `maze_files/` has:
- First line → Player’s starting **strength** and **moves**.
- Following lines → Maze grid (characters represent tiles & entities).

Example (`maze1.txt`):
```
2 10
WWWWWW
WP  C W
W   G W
WWWWWW
```

---

## License
This project is licensed under the **MIT License**. ([github.com](https://github.com/medley-co/Sokoban-Game.git))

---

## Acknowledgements
- Inspired by the classic Sokoban puzzle game.
- Built as an enhanced assignment version with added gameplay features.
