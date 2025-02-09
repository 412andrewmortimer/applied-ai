# 5.0 Adversarial Search and Games

## Overview
- Adversarial search deals with **multi-agent environments**, where agents compete with one another.
- **Games** are a common example of adversarial environments and serve as a testbed for AI techniques.
- The goal of adversarial search is to maximize an agent’s utility while minimizing the utility of its opponent.

---

## **🧠 Key Concepts**
1. **Game Trees**:
   - Represent all possible **moves and counter-moves** in a game.
   - Used to **plan ahead** and evaluate possible outcomes.

2. **Minimax Algorithm**:
   - A **decision-making strategy** assuming **both players play optimally**.
   - **MAX** tries to maximize the outcome.
   - **MIN** tries to minimize MAX’s advantage.

3. **Alpha-Beta Pruning**:
   - An **optimization of Minimax** that eliminates unnecessary calculations.
   - Reduces the number of **nodes evaluated**, making the search faster.

4. **Evaluation Functions**:
   - Used when a **game tree is too large** to search exhaustively.
   - Assigns **heuristic values** to intermediate game states.

5. **Stochastic & Imperfect Information Games**:
   - **Stochastic Games**: Incorporate randomness (e.g., dice rolls in Backgammon).
   - **Imperfect Information Games**: Players lack full visibility (e.g., Poker).

---

### **2. Game Trees**
- Represent the possible moves and states in a game.
- Root node represents the current state.
- Children nodes represent possible actions from the current state.
- **Maximizing Agent**: The agent trying to maximize its utility.
- **Minimizing Agent**: The opponent trying to minimize the maximizing agent’s utility.

---

### **3. Minimax Algorithm**
- **Purpose**: Finds the optimal move in deterministic, perfect-information games.
- Assumes:
  - The maximizing agent plays optimally.
  - The minimizing agent also plays optimally.
- **Steps**:
  1. Generate the game tree up to a certain depth.
  2. Apply the utility function to terminal nodes.
  3. Propagate values back up the tree (min or max at each level).

---

### **4. Alpha-Beta Pruning**
- An optimization for the **Minimax Algorithm** that eliminates branches of the game tree that cannot affect the final decision.
- **Alpha (α)**: The best value that the maximizing agent can guarantee.
- **Beta (β)**: The best value that the minimizing agent can guarantee.
- **Pruning**: Stops evaluating a branch when α ≥ β.

---

### **5. Evaluation Functions**
- Used to approximate the utility of a game state when the tree cannot be searched to terminal nodes.
- Example for chess: A weighted sum of material count, board position, and other heuristics.

---

### **6. Stochastic Games**
- Incorporate chance nodes into the game tree (e.g., dice rolls).
- Utility is calculated using **expected values**:
  - Probability-weighted average of possible outcomes.

---

## **Key Algorithms**
1. **Minimax Algorithm**:
   - Finds optimal moves by considering both players' strategies.
2. **Alpha-Beta Pruning**:
   - Optimizes Minimax by reducing the number of nodes evaluated.
3. **Expectiminimax**:
   - Extends Minimax to stochastic games by incorporating chance nodes.

---

## **Key Takeaways**
1. **Adversarial Search** is essential for modeling competitive environments.
2. **Minimax** provides a foundation for strategic decision-making in games.
3. **Alpha-Beta Pruning** significantly improves search efficiency.
4. Heuristic evaluation functions are critical for handling complex games where exhaustive search is impractical.
5. Stochastic games require probabilistic reasoning to handle uncertainty.