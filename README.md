# Snake_Game

The Snake Game is a classic arcade game that involves a snake navigating around a grid, consuming food items to grow longer while avoiding collisions with the walls or itself. This implementation of the Snake Game in C++ uses arrays to manage the game state and provide a simple, yet effective, gaming experience.

## Key Features:

1. **Grid-Based Gameplay:**
    - The game is played on a 2D grid represented by a 2D array. Each cell of the array can be empty, contain a part of the snake, or hold a food item.

2. **Snake Representation:**
    - The snake is represented using a linked-list-like structure within arrays, where each element of the snake is tracked by its coordinates. The head and the tail of the       snake are managed to facilitate movement and growth.

3. **Food Generation:**
    - Food items are randomly placed on the grid in empty cells. When the snake consumes a food item, it grows longer, and a new food item is generated.

4. **Movement and Controls:**
    - The snake can move in four directions: up, down, left, and right. These movements are controlled by user input (typically arrow keys).
    - The snake's body follows the head, mimicking real-life snake movement.

5. **Collision Detection:**
    - The game detects collisions with the walls (grid boundaries) and the snake's own body. A collision results in the game being over.

6. **Score Tracking:**
    - The player's score is tracked based on the number of food items consumed by the snake.



## Implementation Details:

1. **Grid Initialization:**
    - A 2D array is initialized to represent the game grid. Empty cells are marked with a specific character (e.g., ' '), the snake's body is marked with another character         (e.g., 'S'), and food items are marked with a different character (e.g., 'F').

2. **Snake Movement:**
    - The snake's head moves to a new cell based on user input. The previous positions of the snake's body are updated accordingly.
    - If the snake moves to a cell containing food, the snake grows by adding a new segment to its body.

3. **Game Loop:**
    - The game runs in a loop, continuously checking for user input, updating the snake's position, checking for collisions, and rendering the grid.
    - The loop runs until a collision is detected, at which point the game ends.

4. **Rendering:**
    - The game grid is rendered to the console after each move, providing a real-time view of the game state.
