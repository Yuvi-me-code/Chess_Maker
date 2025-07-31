# Chess Maker

This repository contains a fully functional chess game built with Python and Pygame. It features a clean graphical user interface, complete chess rule implementation, and a challenging AI opponent to play against.

## Features

- **Graphical User Interface**: A clean and responsive chessboard rendered with Pygame.
- **Player vs. AI**: Play a full game of chess against an AI opponent.
- **Intelligent AI**: The AI uses the Negamax algorithm with alpha-beta pruning to determine the best move. Its evaluation function considers material advantage and piece positioning using piece-square tables.
- **Complete Chess Rules**:
    - Standard moves for all pieces (Pawn, Rook, Knight, Bishop, Queen, King).
    - Castling (both kingside and queenside).
    - *En passant* captures.
    - Pawn promotion (automatically promotes to Queen).
- **Advanced Move Validation**:
    - Detects checks, pins, and illegal moves.
    - Accurately determines checkmate and stalemate conditions.
- **Interactive Gameplay**:
    - Click-to-move interface.
    - Highlights the selected piece and all its valid moves.
    - Highlights the previous move for clarity.
    - Smooth animations for piece movements.
- **Game Controls**:
    - Undo the last move.
    - Reset the board to start a new game.
- **Move Log**: Displays a running log of all moves made during the game in standard chess notation.

## Project Structure

```
.
├── ChessMain.py        # Main entry point, handles GUI, user input, and game loop.
├── ChessEngine.py      # Core game logic, game state, move generation, and validation.
├── ChessAI.py          # AI logic, including Negamax search and board evaluation.
└── images/             # Contains all the PNG images for the chess pieces.
```

## How to Run

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/yuvi-me-code/chess_maker.git
    cd chess_maker
    ```

2.  **Install dependencies:**
    The project requires Pygame. You can install it using pip.
    ```sh
    pip install pygame
    ```

3.  **Run the game:**
    Execute the `ChessMain.py` script.
    ```sh
    python ChessMain.py
    ```

## Controls

-   **Mouse Click**:
    -   First click on a piece to select it.
    -   Second click on a valid destination square to move the piece.
-   **'z' Key**: Press `Z` to undo the last move (works for both player and AI moves).
-   **'r' Key**: Press `R` to reset the game to its initial state.
