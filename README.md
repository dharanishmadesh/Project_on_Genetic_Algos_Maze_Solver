# Genetic Algorithm for Maze Solving

## Overview
This project implements a **Genetic Algorithm (GA) to solve a maze** by evolving a population of possible paths towards the optimal solution. The algorithm uses selection, mutation, and crossover to navigate the maze efficiently.

## Features
- **Genetic Algorithm-based pathfinding**
- **Mutation and crossover operators** to evolve solutions
- **Visualization of the best-found path**
- **Configurable population size and generations**

## Installation
To run this project, install the required dependencies:

```bash
pip install matplotlib deap numpy
```

## Usage
Run the script to start the Genetic Algorithm:

```bash
python maze_solver.py
```

### **How It Works**
1. **Defines a maze** with walls (1) and open paths (0).
2. **Encodes possible paths** as sequences of movements (U, D, L, R).
3. **Evaluates each path** based on how close it gets to the goal.
4. **Uses genetic operations** (selection, mutation, and crossover) to evolve paths.
5. **Visualizes the best path found** during key generations.

## Maze Representation
- The maze is represented as a **2D list** where `1` is a wall and `0` is an open path.
- The **start position** is at `(0,0)` and the **goal position** is at the bottom right corner.

## Genetic Algorithm Details
- **Selection**: Tournament selection
- **Crossover**: Uniform crossover
- **Mutation**: Random direction changes
- **Fitness Function**: Uses Manhattan distance to goal

## Example Output
- The algorithm prints the **best path found at key generations (2, 10, 50, 100, 500)**.
- The final **best path is visualized** with start, end, and traversed points.

## Example Visualization
- Green: Start Position
- Red: End Position
- Blue: Path Taken

## Configuration
Modify the `run_ga` function to adjust parameters:

```python
def run_ga(generations=2000, pop_size=50):
    pop = toolbox.population(n=pop_size)
```

## Contributing
Feel free to **fork the repository** and submit **pull requests** with improvements.

## License
This project is open-source and available under the **MIT License**.

