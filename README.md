# 🧩 Maze Solver

A C++ implementation of the classic **Rat in a Maze** problem using a backtracking algorithm.

---

## 🚀 Overview

This project finds **all possible paths** for a rat to travel from the top-left corner `(0,0)` to the bottom-right corner `(n-1,n-1)` in a square maze. The rat can move **Down (D), Left (L), Right (R), or Up (U)**, but only through cells marked with `1` (open path).

---

## 🧠 Algorithm Details

1. **Start** at cell `(0,0)`.
2. **Check** if the current cell is within bounds, open, and not previously visited.
3. **Mark** the cell as visited.
4. **Recursively explore** all four directions:
    - Move and append the direction (`D`, `L`, `R`, `U`) to the path.
    - Recurse to the next cell.
    - **Backtrack**: Remove the direction and mark the cell as unvisited.
5. **Store** the path if the destination `(n-1,n-1)` is reached.
6. **Return** all valid paths.

---

## 🧪 Sample Input

You will be prompted for:

- The size of the maze (`n`)
- The maze matrix (where `1` = open, `0` = blocked)

**Example:**
```
Enter the size of the maze (n): 4
Enter the maze matrix:
1 0 0 0
1 1 0 1
0 1 0 0
1 1 1 1
```

---

## 📤 Sample Output

All valid paths from start to finish will be displayed:

```
Paths found:
DDRDRR
DRDDRR
```

If there is **no possible path**, you’ll see:
```
No path found
```

---

## 📚 Features

- Efficient **backtracking** algorithm.
- Supports **all possible paths** (not just one).
- **User-friendly** prompts and output.
- Handles **blocked start/end** gracefully.

---

## 💡 Real-Worl Application

This project mirrors challenges in:

- Robotics (pathfinding for autonomous agents).
- Game Development (NPC navigation).
- Network Routing (optimizing data pathways)

---
