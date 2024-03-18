# Tic-Tac-Toe Game Description

1. Constants `X` and `O` are defined to represent player symbols.

2. `cells`, `statusText`, and `restartBtn` are selected from the DOM. `cells` represent the individual cells of the game board, `statusText` displays game status, and `restartBtn` allows players to restart the game.

3. An array `winConditions` is defined to hold all possible winning combinations on the game board.

4. An array `options` is initialized to represent the current state of the game board. Each element in `options` corresponds to a cell on the game board, initially empty.

5. `currentPlayer` is initialized to `X`, indicating that the first move will be made by player `X`. `running` is initially set to `false`, indicating that the game is not yet in progress.

6. `initializeGame()` sets up event listeners for each cell and the restart button, and updates the status text to indicate whose turn it is.

7. When a cell is clicked (`cellClicked()`), it checks if the cell is already occupied or if the game is not running. If either condition is true, the function returns without taking any action. Otherwise, it updates the cell with the current player's symbol and checks for a winner.

8. `updateCell()` updates the game board array (`options`) and updates the clicked cell with the current player's symbol.

9. `changePlayer()` switches the current player between `X` and `O` and updates the status text accordingly.

10. `checkWinner()` iterates through the `winConditions` array to check if any player has won. If a winning condition is found, it updates the status text with the winning player's symbol and stops the game. If no winner is found and the game board is full (no empty cells), it declares a draw. Otherwise, it switches to the next player.

11. `restartGame()` resets the game state to its initial state, including clearing the game board and resetting variables.

Overall, this code provides the basic functionality for a two-player Tic-Tac-Toe game, allowing players to take turns, detecting wins and draws, and enabling game restarts.

