# Grid-Based Navigation using MDP

This project implements a Markov Decision Process (MDP) for a grid-based road navigation task using Value Iteration.

## Overview

- **Environment:** 5x5 grid
- **Agent Start State:** (0, 0)
- **Goal State:** (4, 4)
- **Obstacles:** Placed at selected grid cells
- **Actions:** Up, Down, Left, Right
- **Rewards:**
  - +10 for goal
  - -10 for obstacle collision
  - -1 for each movement

## Features

- Implementation of Value Iteration
- Policy extraction
- Visualization of agent path
- Optional value heatmap display
- Animated simulation (in Colab or exportable as GIF)

## How to Run

1. Open `grid_navigation_mdp.ipynb` in Google Colab or Jupyter Notebook.
2. Run all cells to generate the visualization.
3. Use `HTML(anim.to_jshtml())` to render the animation inline in Colab.


