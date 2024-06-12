# Tic-Tac-Toe using Alpha-Beta Pruning (Python)

## Introduction

Welcome to the **Tic-Tac-Toe using Alpha-Beta Pruning (Python)** repository! This project implements a Tic-Tac-Toe game where an AI opponent uses the Minimax algorithm enhanced with Alpha-Beta Pruning to play optimally. The AI ensures that the player is always challenged, making the game both enjoyable and educational.

## What is Alpha-Beta Pruning?

Alpha-Beta Pruning is an optimization technique for the Minimax algorithm, which is used in decision-making and game theory. It reduces the number of nodes evaluated by the Minimax algorithm in its search tree. By eliminating branches that cannot possibly influence the final decision, Alpha-Beta Pruning makes the algorithm more efficient, allowing it to handle more complex scenarios or to run faster in simpler ones.

## How is Alpha-Beta Pruning Used in Tic-Tac-Toe?

In Tic-Tac-Toe, the Minimax algorithm explores all possible moves to determine the optimal strategy. Alpha-Beta Pruning enhances this process by cutting off branches in the search tree that won't affect the outcome, thus speeding up the decision-making process. This allows the AI to compute the best possible move within a reasonable time frame, ensuring a challenging opponent without long waits.

## Explanation of the Code

### 1) Initial Setup

The constants and initial state of the board are defined at the beginning

### 2) Drawing the Board

The `draw_board` function prints the current state of the board

### 3) Player Turn

The `player` function determines whose turn it is

### 4) Possible Actions

The `actions` function lists all possible moves

### 5) Resulting Board State

The `result` function returns the board state after a move

### 6) Checking for a Winner

Helper functions `get_horizontal_winner`, `get_vertical_winner`, and `get_diagonal_winner` check for winning lines. The `winner` function integrates these

### 7) Terminal State and Utility

The `terminal` function checks if the game is over, and the `utility` function evaluates the board

### 8) Minimax Algorithm with Alpha-Beta Pruning

The core logic for the AI is implemented in the `minimax`, `max_value`, and `min_value` functions

### 9) Playing the Game

The `play_game` function manages the game loop, allowing a human player to compete against the AI

## Conclusion

This repository demonstrates a practical application of the Minimax algorithm with Alpha-Beta Pruning in a classic game of Tic-Tac-Toe. The AI opponent ensures an engaging experience by playing optimally, showcasing the effectiveness of Alpha-Beta Pruning in reducing computation time while maintaining strategic depth. Feel free to explore the code, play the game, and learn more about game theory and AI decision-making processes.

Enjoy playing Tic-Tac-Toe with an intelligent opponent!
