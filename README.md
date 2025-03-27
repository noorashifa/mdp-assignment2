# Grid-Based Navigation using MDP

This project implements a Markov Decision Process (MDP) model for a grid-based road navigation task. The goal is to simulate how an agent can make sequential decisions to reach a goal state in a 5x5 grid environment, while avoiding obstacles and optimizing for rewards using value iteration.

## Problem Setup

- **Grid Size:** 5x5
- **Start State:** (0, 0)
- **Goal State:** (4, 4)
- **Obstacles:** (0,3), (1,1), (2,4), (3,1)
- **Actions:** Up, Down, Left, Right
- **Transition Model:** Deterministic

## Rewards

- `+10` for reaching the goal state
- `-10` for entering an obstacle
- `-1` for all other valid movements (to encourage shortest path)

## MDP Components

- **States:** Each cell in the grid represents a unique state
- **Actions:** Move to adjacent cells if valid
- **Transition Probabilities:** 1 for valid action, 0 otherwise
- **Reward Function:** Defined as above
- **Policy:** Derived using Value Iteration

## Value Iteration

The value iteration algorithm updates state values iteratively using the Bellman equation until convergence. The optimal policy is then extracted by choosing actions that lead to states with the highest value.

## Output & Visualization

- The agent's optimal path from the start to the goal is animated.
- Obstacles are displayed in red, the goal in green, and the agent as a moving blue circle.

## How to Run

Open the notebook in Google Colab or Jupyter:

```python
# For Colab display:
from IPython.display import HTML
HTML(anim.to_jshtml())
```

## Author

Noora Shifa  
CMPT 602/702 – Decision-Making and Control in Autonomous Systems  
Spring 2025

