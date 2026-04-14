# Input Specification - Tetris Game

## Keyboard Controls

### Movement
- `←` (Left Arrow): Move piece left
- `→` (Right Arrow): Move piece right
- `↓` (Down Arrow) or `S`: Soft drop (move down one cell)

### Rotation
- `↑` (Up Arrow) or `X`: Rotate clockwise
- `Z` or `Ctrl`: Rotate counter-clockwise

### Dropping
- `Space`: Hard drop (instantly place piece at bottom)

### Game Actions
- `C` or `Shift`: Hold current piece
- `P` or `Esc`: Pause/unpause game
- `R`: Restart game

### Input State Management
- Key down events trigger actions
- Key up events reset input state
- Hold detection for continuous movement

## Game State Inputs

### Start Screen
- `Enter`: Start new game

### Pause Screen
- `P` or `Esc`: Resume game

### Game Over Screen
- `R`: Restart game

## Input Validation
- All inputs should be handled through a centralized input manager
- Key combinations should be properly detected (Ctrl, Shift)
- Input should be disabled during game over state unless restarting
