# Knight Path Visualization

A collaborative Data Structures coursework project built with Python and Pygame. Choose starting and target squares, then watch a chess knight follow paths produced by different search algorithms.

## Features

- An 8×8 chessboard with an animated knight
- Breadth-first search (BFS)
- Depth-first search (DFS)
- An experimental A*-style search using a heuristic
- Coloured paths and directional arrows
- Execution-time measurements for each search
- A depth-limited tree of possible knight moves, printed in the terminal

The animation shows each algorithm’s returned path, rather than every square explored during its search.

## Running the Project

Install Python 3 and Pygame:

```bash
python -m pip install pygame
```

Download or clone this repository. Keep these files together:

- `Knight_Game.py`
- `Knight free icons designed by Victoruler.png`

From the project folder, run:

```bash
python Knight_Game.py
```

Enter the starting and target coordinates in the terminal. Each coordinate must be an integer from **0 to 7**.

The Pygame window automatically displays the BFS, DFS and experimental A*-style paths in sequence. Close the window to exit.

## Algorithm Notes

- **BFS:** Finds a shortest path by number of knight moves on this unweighted board.
- **DFS:** Finds a valid path, but does not guarantee the shortest path.
- **Experimental A*-style search:** Prioritizes paths using their length and a distance estimate. This implementation is a coursework experiment and does not guarantee an optimal path.

Displayed times measure individual search calls, excluding animation. They are illustrative measurements, not a rigorous performance benchmark.

## Contributions

- **Dlon Rash:** Pygame board setup and visualization, including path presentation and directional arrows.
- **Kara:** Move-generation and search code, as identified in the source comments.
- **Chris:** Knight node and depth-limited tree implementation.

## Asset Credit

Knight icon credited to **Victoruler** in the supplied image filename.

## Current Limitations

- Coordinates are entered through the terminal.
- Non-numeric input is not handled.
- Changing the start and target requires restarting the program.
- The start-square highlight currently uses the target coordinates and needs correction.
