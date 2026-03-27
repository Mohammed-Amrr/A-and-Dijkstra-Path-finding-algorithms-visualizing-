# Pathfinding Algorithm Visualizer

An interactive visualizer for A* and Dijkstra's pathfinding algorithms, built with Python and Pygame. Watch in real time as each algorithm explores the grid and finds the shortest path.

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pygame](https://img.shields.io/badge/Pygame-2.x-green)

---

## Demo

[Pathfinding_visualizer](https://github.com/user-attachments/assets/6133643c-cebe-42b1-8536-d45910e04029)


---

## What it does

- Renders a 40x40 interactive grid
- Lets you place a start node, end node, and draw walls manually
- Generates a random maze with one keypress
- Visualizes A* and Dijkstra's algorithms step by step in real time
- Highlights the final shortest path once found
- Displays live status in the UI bar

---

## Algorithms


 - Dijkstra's Algorithm
   
Explores all directions equally, expanding outward (something like a circle) from the start node based purely on distance traveled. Guaranteed to find the shortest path but evaluates in all directions making it far more slower than A* alogrithm. The visual demonstration clearly shows the difference between both alogorithms and why A* is more efficient.

 - A* Algorithm
  
Depends on heuristic function (Manhattan distance) to search in the direction of the goal. By calculating an estimation of the remaining distance to the goal at each step (node). This algorithm can be 5x up to 20x faster than Dijkstra depending on the maze shape. This is because Dijkstra's explored node count grows as a circle (area = πr²), while A*'s grows as a much narrower cone pointed at the goal. ( it's easier to just see it yourself to understand , check the instructions and controls to try it OR see the GIF demonstration above )



---

## Controls

| Key | Action |
|-----|--------|
| Left click | Place start node (first click), end node (second click), then draw walls |
| Left click + drag | Draw walls |
| Right click | Erase a node |
| `SPACE` | Run A* |
| `D` | Run Dijkstra |
| `M` | Generate random maze (requires start and end placed first) |
| `C` | Clear the grid |

---

## Color Reference

| Color | Meaning |
|-------|---------|
| Green | Start node |
| Red | End node |
| Black | Wall |
| Orange | Open set — currently being evaluated |
| Blue | Closed set — already evaluated |
| Purple | Final shortest path |


---
