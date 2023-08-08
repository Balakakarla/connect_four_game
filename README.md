# connect_four_game
Connect Four is a popular two-player strategy game where players take turns dropping colored discs into a vertical grid. The objective is to connect four discs of the same color vertically, horizontally, or diagonally before your opponent does.

To make the game more challenging and competitive, an AI-based approach using alpha-beta pruning can be used. Alpha-beta pruning is a search algorithm used in game-playing to decrease the number of nodes evaluated by the minimax algorithm, which is used to determine the best move for the AI player.

This paper presents an implementation of the Connect Four game using an AI-based approach with alpha-beta pruning. The algorithm utilizes a game tree to represent all possible moves and outcomes, and alpha-beta pruning to efficiently eliminate unnecessary branches of the tree, resulting in a faster and more accurate decision-making process.

The implementation was tested against human players and achieved a high level of success, demonstrating the effectiveness of the AI-based approach using alpha-beta pruning in Connect Four. This approach can be applied to other strategy games, making it a valuable tool in the development of intelligent game-playing agents.

Alpha-beta Pruning:
Alpha-beta pruning is a search algorithm used in decision trees to minimize the number of nodes that need to be evaluated in the search tree. It is a heuristic search algorithm that eliminates the nodes that are guaranteed to never be selected. It is an extension of the Minimax algorithm, which is used to determine the best move for a player assuming that the opponent is also playing optimally.



                                             Implementation
In the implementation of the AI-based Connect Four game using alpha-beta pruning, we first represent the game board as a two-dimensional array. We use the following notation for the game board:

0 represents an empty cell
1 represents a disc placed by player 
2 represents a disc placed by AI

Next, we define the evaluation function for the game board. The evaluation function assigns a score to each possible game state, indicating how favorable it is for the player. A positive score indicates that the state is favorable for player 1, while a negative score indicates that the state is favorable for player 2.
We then implement the alpha-beta pruning algorithm. The algorithm recursively evaluates each possible move by considering the game board resulting from each move. It keeps track of the best score found so far and the range of scores that are still possible. The algorithm prunes branches of the search tree that are guaranteed to never be selected.
Alpha-beta pruning is used in the Connect Four game because it is an optimization technique that allows the AI player to search the game tree more efficiently and make better decisions.
Connect Four has a large game tree with many possible moves and states, and the traditional Minimax algorithm without alpha-beta pruning would need to evaluate all possible moves to determine the best one. However, by using alpha-beta pruning, the algorithm can eliminate certain branches of the game tree that are guaranteed to not lead to a better outcome, and thus avoid evaluating those moves, significantly reducing the search space and making the AI player more efficient.


Result:
![image](https://github.com/Balakakarla/connect_four_game/assets/123648737/9094e9c8-3f54-4312-8768-3a7d821960e8)  --->won by ai
![image](https://github.com/Balakakarla/connect_four_game/assets/123648737/2c1290fa-bd8d-46a4-85c5-6e5d40a41878)   ---->won by human player

