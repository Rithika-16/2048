# 2048 Game Implementation  

This project is a **Python-based implementation of the 2048 puzzle game** using the **Pygame library**. The game features smooth tile animations, responsive controls, and an intuitive graphical interface. Below is an overview of the code functionality:  

## Code Breakdown  

### 1. Game Setup  
- **Constants and Configuration**: Defines screen dimensions, colors, font styles, and grid properties.  
- **Window Initialization**: Sets up the game window using Pygame with an 800x800 resolution.  

### 2. Tile Class  
Represents the numbered tiles on the grid.  
- **Key Functions**:  
  - `get_color()`: Dynamically assigns tile colors based on their value.  
  - `draw()`: Renders the tile and its value on the grid.  
  - `move()`: Updates tile position during animations.  
  - `set_pos()`: Adjusts tile position to align with grid cells.  

### 3. Grid and Drawing Functions  
- `draw_grid(window)`: Draws the 4x4 grid with outlined cells.  
- `draw(window, tiles)`: Updates the game window with the current tile positions and grid layout.  

### 4. Tile Management  
- **Random Tile Placement**:  
  - `get_random_pos(tiles)`: Finds an empty cell to place a new tile.  
  - `generate_tiles()`: Initializes the grid with two starting tiles.  
- **Updating and Sorting**:  
  - Tiles are sorted and updated based on movement direction to handle merging and repositioning efficiently.  

### 5. Movement Logic  
- `move_tiles(window, tiles, clock, direction)`: Implements tile movement and merging logic based on input direction.  
- **Directional Logic**:  
  - Handles conditions for moving, merging, and stopping tiles using boundary checks and delta movements.  
  - Manages collision detection and value merging for tiles of the same value.  

### 6. Game State Management  
- `end_move(tiles)`: Adds a new tile after each move and checks for game-over conditions.  
- `update_tiles(window, tiles, sorted_tiles)`: Updates tile positions in the grid after every move.  

### 7. Main Game Loop  
- **Input Handling**: Captures user input for directional movements (arrow keys).  
- **Game Loop**: Updates the game state, handles drawing, and checks for termination.  

---

## Key Features  
- **Dynamic Animations**: Smooth tile movement with collision handling.  
- **Responsive Controls**: Arrow key inputs for seamless user interaction.  
- **Win/Loss Conditions**: Automatically adds new tiles until no valid moves are left.  
- **Modular Codebase**: Classes and functions are designed for scalability and easy modification.  



