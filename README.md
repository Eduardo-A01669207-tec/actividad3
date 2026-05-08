# Pacman modified
How to run the game: python3 pacman.py

List of changes for this file:

The ghosts move faster across the board.

The ghosts are smarter and now actively chase Pacman instead of moving randomly.

Change 1
The speed of the ghosts was increased to make the game more challenging. Inside the options array where the movement vectors are defined, the values were changed from 5 and -5 to 7 and -7, allowing the ghosts to cover more distance per frame.

Author: Alejandro Rodriguez Brito

Change 2
The pathfinding logic for the ghosts was rewritten to make them smart. Previously, they would blindly choose a random valid direction when hitting a wall using choice(options). Now, the code evaluates all valid moves, calculates the distance between the ghost and Pacman for each option, and uses a min() function with a lambda expression to always select the path that brings the ghost closer to Pacman.

Author: Eduardo Arteaga Camacho
