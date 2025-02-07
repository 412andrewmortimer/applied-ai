# 5.1 Game Theory

## Overview
Game theory provides a mathematical framework for modeling multi-agent environments where the outcomes for each agent depend on the actions of others. It is widely applied in adversarial search to analyze competitive scenarios, such as games.

---
## **Vocabulary and Definitions**

| **Term**                  | **Definition**                                                                                                                              |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| **Game**                  | A scenario involving multiple players, each with a set of strategies and payoffs.                                                           |
| **Player**                | An agent that participates in the game, aiming to maximize its payoff.                                                                      |
| **Strategy**              | A plan of action or decision-making rule for a player in the game.                                                                          |
| **Pure Strategy**         | A deterministic approach where a player always selects the same move in a given situation.                                                  |
| **Mixed Strategy**        | A probabilistic approach where a player assigns probabilities to different moves.                                                           |
| **Utility Function**      | A numerical value representing the desirability of a game state for a player.                                                               |
| **Payoff Matrix**         | A table showing the payoffs for each combination of strategies by the players.                                                              |
| **Zero-Sum Game**         | A game where one player’s gain is the other player’s loss.                                                                                  |
| **Nash Equilibrium**      | A stable state where no player benefits from unilaterally changing their strategy.                                                          |
| **Minimax Principle**     | A decision rule where a player minimizes the maximum possible loss.                                                                         |
| **Adversarial Search**    | A search method where multiple agents compete, aiming to maximize their utility while minimizing the opponent's.                            |
| **Economy**               | The concept of efficiently using resources, often applied in AI to optimize computation and decision-making.                                |
| **Pruning**               | A technique in search algorithms (e.g., Alpha-Beta Pruning) that eliminates branches in the game tree that do not need to be explored.      |
| **Evaluation Function**   | A heuristic function used in games to approximate the value of a game state when it is impractical to search all the way to terminal nodes. |
| **Imperfect Information** | A type of game where players do not have full knowledge of the game state, such as in Poker where opponents' hands are hidden.              |

---

## **Key Concepts**

### **1. Zero-Sum Games**
- In **zero-sum games**, the total payoff for all players is constant. One player’s gain is exactly the other player’s loss.
- Example: Chess, where one player wins, and the other loses.

### **2. Strategies**
- **Pure Strategy**:
  - A deterministic approach where a player always selects the same move in a given situation.
- **Mixed Strategy**:
  - A probabilistic approach where a player assigns probabilities to different moves.

### **3. Nash Equilibrium**
- A situation where no player can improve their outcome by unilaterally changing their strategy.
- At equilibrium, all players are playing optimally given the strategies of others.

### **4. Minimax Principle**
- A decision rule used in two-player, zero-sum games.
- Each player minimizes the maximum possible loss:
  - **Maximizing Player**: Tries to maximize their utility.
  - **Minimizing Player**: Tries to minimize the maximizing player’s utility.

---


## **Payoff Matrix Example**
A **payoff matrix** illustrates the payoffs for two players based on their chosen strategies.

| **Player 2**    | **Strategy A** | **Strategy B** |
|-----------------|----------------|----------------|
| **Player 1: A** | (3, -3)        | (-1, 1)        |
| **Player 1: B** | (0, 0)         | (2, -2)        |

- Rows represent **Player 1’s** strategies.
- Columns represent **Player 2’s** strategies.
- Payoffs are listed as `(Player 1 payoff, Player 2 payoff)`.

---

## **Applications of Game Theory**
- **Adversarial Search**:
  - Used in games like chess or Go, where agents compete.
- **Economics**:
  - Modeling markets and competitive business strategies.
- **Negotiation and Conflict Resolution**:
  - Finding stable strategies in multi-party agreements.
- **Artificial Intelligence**:
  - Building rational agents that make strategic decisions.

---

## **Key Takeaways**
1. Game theory provides tools for modeling **competitive and strategic interactions**.
2. **Zero-sum games** highlight direct competition where one player’s gain equals the other’s loss.
3. Concepts like the **Minimax Principle** and **Nash Equilibrium** are essential for understanding multi-agent interactions.
4. Payoff matrices provide a simple way to analyze the outcomes of strategies.

---