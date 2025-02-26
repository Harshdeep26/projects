Maze Solver Using BFS/DFS

Project Overview:-
A maze solver finds a path from the start position to the end position in a 2D grid-based maze.

The maze is represented as a grid, where 0 represents an open path, and 1 represents walls.
The goal is to find the shortest path from the start to the end using BFS (or DFS).


Concepts Used:-
Graph Representation: The maze is treated as a graph where each cell is a node, and edges exist between adjacent cells.
Breadth-First Search (BFS): BFS is used to find the shortest path in an unweighted grid. It explores neighbors level by level.
Depth-First Search (DFS) (Alternative): DFS can also be used, but it doesn’t guarantee the shortest path because it explores deeper paths first.


Key Components:-
Grid Representation: The maze is a 2D vector (matrix).
Movement Handling: We use four possible movement directions (up, down, left, right).
Queue (BFS): The BFS algorithm uses a queue to explore cells systematically.
Visited Cells: A 2D boolean array tracks visited cells to avoid infinite loops.
Shortest Path Calculation: BFS ensures that the first time we reach the destination, we have found the shortest path.


How It Works:-
The starting point is enqueued with an initial distance of 0.
BFS explores all possible paths, ensuring the shortest path is found first.
When we reach the destination, we return the shortest distance.
If we cannot reach the destination, we return -1 (indicating no path exists).
