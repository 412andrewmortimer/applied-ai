# 5.1.1 Perfect Information Zero-Sum Games

## Overview
This section focuses on **perfect information zero-sum games**, a subclass of competitive environments where:
1. **Perfect Information**: All players have complete knowledge of the game state.
2. **Zero-Sum**: One player’s gain is another player’s loss.

Examples include **Chess**, **Go**, and **Tic-Tac-Toe**, where both players can see the entire game state and take turns making decisions.

---

## **Key Components of Perfect Information Games**
### **1. Game Representation**
A game is modeled using:
- **Initial State**: The starting position of the game.
- **Players**: Typically two competing agents.
- **Move**: A legal action taken by a player.
- **State Space Graph**: A directed graph where nodes represent game states, and edges represent legal moves.
- **Search Tree**: A tree representation of game states explored by an AI agent.

### **2. Game Progression**
- **Transition Model**: Defines how actions change the game state.
- **Terminal State**: A state where the game ends (win/loss/draw).
- **Terminal Test**: A function that checks whether a state is terminal.

### **3. Game Evaluation**
- **Utility Function**: Assigns a numerical value to terminal states:
  - Win (+1), Loss (-1), Draw (0) in Tic-Tac-Toe.
  - More complex utility values exist in Chess and Go.

### **4. Game Trees vs. Search Trees**
- **Game Tree**: Represents all possible sequences of moves from the initial state.
- **Search Tree**: Explored portion of the game tree based on an AI agent's search algorithm.

---

## **Vocabulary Table for 5.1.1**

| **Term**              | **Definition**                                                                 |
|----------------------|-------------------------------------------------------------------------------|
| **Perfect Information** | A game where all players have full visibility of the game state. No hidden information exists. |
| **Zero-Sum Game**     | A game where one player’s gain equals the other player’s loss. |
| **Position**         | The current configuration of the game state at a specific point in play. |
| **Move**            | A legal action that transitions the game from one state to another. |
| **Initial State**   | The starting position of a game, from which the first move is made. |
| **Transition Model** | A function that defines the result of taking an action in a given state. |
| **Terminal Test**   | A function that checks whether the current game state is a terminal state (i.e., the game has ended). |
| **Terminal State**  | A game state where no further moves can be made, and the game is over. |
| **Utility Function** | A numerical function that assigns values to terminal states (e.g., Win = 1, Loss = -1, Draw = 0). |
| **State Space Graph** | A graph where nodes represent game states and edges represent moves. |
| **Search Tree**     | A tree representation of game states explored during an AI search process. |
| **Game Tree**       | A full representation of all possible moves and game states from the initial state onward. |

---

## **Key Takeaways**
1. **Perfect information zero-sum games** allow for complete visibility of the game state.
2. **Utility functions** are used to evaluate terminal states numerically.
3. **Game trees** represent all possible moves, while **search trees** focus only on explored paths.
4. These principles lay the foundation for AI strategies like **Minimax** and **Alpha-Beta Pruning**.
