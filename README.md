https://Sagi4A.github.io/react-tic-tac-toe-game
# react-tic-tac-toe-game


This project is a classic Tic Tac Toe game built by following the official React tutorial. (https://react.dev/learn/tutorial-tic-tac-toe#)
It demonstrates the fundamental concepts of React development, including components, props, state management, event handling, and lifting state up.

What is Implemented
Interactive game board with nine squares.
Player turns alternating between “X” and “O”.
Winner detection using a helper function to evaluate board state.
Game status display showing the next player or the winner.
Move history (“time travel”) allowing players to navigate back to previous game states.
Re-rendering logic so that the UI updates automatically when state changes.

React Concepts and Methods Used
Functional Components: The game is structured into reusable components (Square, Board, Game).
Props: Data is passed from parent to child components (e.g., value and onSquareClick props in Square).
State (useState): Used to store and update the board’s squares and track the current player.
Event Handling (onClick): Squares respond to user clicks and trigger state updates.
Lifting State Up: Game state is managed in the Board component rather than individual squares, ensuring synchronization across the board.
Immutable Updates (slice): The board state is updated by creating copies of the array rather than mutating it directly.
Conditional Rendering: The UI displays either the next player or the winner depending on the game state.
Lists and Keys: The move history is rendered as a list, with unique keys for each move.
Time Travel Feature: Implemented by storing past states in an array and allowing navigation through them.

Project Structure
src/
├── App.jsx        # Root component
├── index.jsx      # Entry point
├── components/
│   ├── Square.jsx # Individual square
│   ├── Board.jsx  # Game board
│   └── Game.jsx   # Game logic and history
├── styles.css     # Styling
public/
└── index.html
