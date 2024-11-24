# CI2024_lab3
# Lab 3: Solving the n²-1 Puzzle with A* Algorithm

This project implements the **A\*** search algorithm to solve the **n²-1 Puzzle** (e.g., 15-puzzle for a 4x4 grid). The goal is to arrange the tiles in numerical order, from left to right and top to bottom, with the blank tile in the bottom-right corner.

---

## Approach

1. **Randomization**:  
   The puzzle is randomized using 100,000 valid moves to ensure solvability.

2. **Heuristic**:  
   The **Manhattan Distance** is used to estimate the cost to reach the goal state. It calculates the sum of tile distances from their correct positions.

3. **A\***:  
   The algorithm explores the most promising states based on the cost function `f(n) = g(n) + h(n)`, where:
   - `g(n)`: Steps taken to reach the current state.
   - `h(n)`: Estimated cost to reach the goal (Manhattan Distance).

---
