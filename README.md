Tic Tac Toe Game with Minimax AI Algorithm
This program is an implementation of the Tic Tac Toe game with an AI player that uses the Minimax algorithm to make decisions.

The game has a command-line interface and is written in Python.

Running the Game
To run the game, simply execute the following command in your terminal:

bash
python3 tictactoe.py

How to Play
The game is played on a 3x3 board. Players take turns placing their symbol (X or O) on the board. The first player to get three of their symbols in a row (horizontally, vertically, or diagonally) wins the game.
When it is the player's turn, they will be prompted to enter the row and column of the cell they want to play. Rows and columns are numbered 1, 2, and 3.
When it is the AI's turn, it will automatically make the best move using the Minimax algorithm.
The player can choose to be X or O at the beginning of the game. If the player chooses X, they will go first. If they choose O, the AI will go first.

Code Structure
The code is divided into several functions:

evaluate(state): Evaluates the state of the board and returns a score based on whether the computer or human has won or if it is a draw.
wins(state, player): Determines if the player has won the game by checking all possible winning configurations.
game_over(state): Determines if the game is over by checking if either player has won or if the board is full.
empty_cells(state): Returns a list of all the empty cells on the board.
valid_move(x, y): Determines if the given move is valid by checking if the cell is empty.
set_move(x, y, player): Sets the move on the board if it is valid.
minimax(state, depth, player): Uses the Minimax algorithm to determine the best move for the computer player.
render(state, c_choice, h_choice): Renders the board on the command line.
The game itself is implemented in the main() function.
