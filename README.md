# PathfindingWithA-Algorithm_202401100400208
Description
This Python program implements the A (A-star)* pathfinding algorithm on a user-defined 2D grid. The algorithm calculates the shortest path from a start point to a goal point, avoiding obstacles provided by the user.

Features:
User-defined grid size and obstacle placement.
A* algorithm to find the shortest path.
Displays the path and obstacles.

Code Overview
Key Functions:

heuristic(a, b):
Calculates the Manhattan distance between two points a and b (used as a heuristic for A*).

a_star(grid, start, goal):
Implements the A* pathfinding algorithm. Finds the shortest path from the start position to the goal while avoiding obstacles.

display_grid(grid, path):
Displays the grid, marking the path with P, obstacles with X, and empty spaces with ..

get_grid_input():
Handles user input for the grid size, obstacles, and positions for the start and goal.

How It Works:

Initialization: The start node is added to the Open List with an initial f score.
Node Expansion: The node with the lowest f score is expanded. Its neighbors are evaluated, and valid ones are added to the Open List.
Pathfinding: The algorithm explores neighbors, updating scores and backtracking once the goal is reached.
Reconstructing Path: When the goal is found, the algorithm traces back through parent nodes to reconstruct the shortest path.
