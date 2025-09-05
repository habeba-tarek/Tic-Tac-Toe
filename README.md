# Tic-Tac-Toe
This project implements a classic Tic-Tac-Toe game with an AI opponent that uses the Minimax algorithm to make optimal moves.The game allows a human player to play against an unbeatable AI that will either win or force a draw in every game.

Key Features
Game Board: A 3x3 grid representation using a 2D list structure
Turn Management: Automatically tracks which player's turn it is (X or O)
Win Detection: Checks for winning conditions across rows, columns, and diagonals
Optimal AI Moves: Implements the Minimax algorithm to ensure the AI makes the best possible move
Terminal State Detection: Identifies when the game has ended (win or draw)

Implementation Details
Board Representation
Uses a 3x3 grid with X, O, and None (EMPTY) values
Provides an initial_state() function to create a blank board

Game Logic
player(board): Determines whose turn it is based on the number of moves made
actions(board): Returns all possible valid moves (empty cells)
result(board, action): Applies a move to the board and returns a new board state
winner(board): Checks if there's a winner and returns the winning player
terminal(board): Determines if the game has ended
utility(board): Returns 1 for X win, -1 for O win, 0 for draw

AI Implementation
minimax(board): The main function that returns the optimal move
max_value(board): Calculates the maximum value achievable by the maximizing player (X)
min_value(board): Calculates the minimum value achievable by the minimizing player (O)

Algorithm
The AI uses the Minimax algorithm with depth-limited search (though Tic-Tac-Toe has a limited search space) to evaluate all possible moves and choose the one with the best outcome, assuming the opponent also plays optimally.

Usage
This implementation can be used as:
A standalone Tic-Tac-Toe game against an AI opponent
A learning tool to understand the Minimax algorithm

A foundation for more complex game AI implementations
