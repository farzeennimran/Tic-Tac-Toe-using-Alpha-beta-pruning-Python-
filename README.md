# Tic-Tac-Toe using Alpha-Beta Pruning (Python)

## Introduction

Welcome to the **Tic-Tac-Toe using Alpha-Beta Pruning (Python)** repository! This project implements a Tic-Tac-Toe game where an AI opponent uses the Minimax algorithm enhanced with Alpha-Beta Pruning to play optimally. The AI ensures that the player is always challenged, making the game both enjoyable and educational.

## What is Alpha-Beta Pruning?

Alpha-Beta Pruning is an optimization technique for the Minimax algorithm, which is used in decision-making and game theory. It reduces the number of nodes evaluated by the Minimax algorithm in its search tree. By eliminating branches that cannot possibly influence the final decision, Alpha-Beta Pruning makes the algorithm more efficient, allowing it to handle more complex scenarios or to run faster in simpler ones.

## How is Alpha-Beta Pruning Used in Tic-Tac-Toe?

In Tic-Tac-Toe, the Minimax algorithm explores all possible moves to determine the optimal strategy. Alpha-Beta Pruning enhances this process by cutting off branches in the search tree that won't affect the outcome, thus speeding up the decision-making process. This allows the AI to compute the best possible move within a reasonable time frame, ensuring a challenging opponent without long waits.

## Explanation of the Code

### Initial Setup

The constants and initial state of the board are defined at the beginning:
```python
X = "X"
O = "O"
D = "D"
EMPTY = None

def initial_state():
    return [[EMPTY, EMPTY, EMPTY],
            [EMPTY, EMPTY, EMPTY],
            [EMPTY, EMPTY, EMPTY]]
```
### Drawing the Board

The `draw_board` function prints the current state of the board:
```python
def draw_board(board):
    ...
```

### Player Turn

The `player` function determines whose turn it is:
```python
def player(board):
    ...
```

### Possible Actions

The `actions` function lists all possible moves:
```python
def actions(board):
    ...
```

### Resulting Board State

The `result` function returns the board state after a move:
```python
def result(board, action):
    ...
```

### Checking for a Winner

Helper functions `get_horizontal_winner`, `get_vertical_winner`, and `get_diagonal_winner` check for winning lines. The `winner` function integrates these:
```python
def winner(board):
    ...
```

### Terminal State and Utility

The `terminal` function checks if the game is over, and the `utility` function evaluates the board:
```python
def terminal(board):
    ...
def utility(board):
    ...
```

### Minimax Algorithm with Alpha-Beta Pruning

The core logic for the AI is implemented in the `minimax`, `max_value`, and `min_value` functions:
```python
def minimax(board, alpha, beta):
    ...
def max_value(board, alpha, beta):
    ...
def min_value(board, alpha, beta):
    ...
```

### Playing the Game

The `play_game` function manages the game loop, allowing a human player to compete against the AI:
```python
def play_game():
    ...
```

## Conclusion

This repository demonstrates a practical application of the Minimax algorithm with Alpha-Beta Pruning in a classic game of Tic-Tac-Toe. The AI opponent ensures an engaging experience by playing optimally, showcasing the effectiveness of Alpha-Beta Pruning in reducing computation time while maintaining strategic depth. Feel free to explore the code, play the game, and learn more about game theory and AI decision-making processes.

Enjoy playing Tic-Tac-Toe with an intelligent opponent!
