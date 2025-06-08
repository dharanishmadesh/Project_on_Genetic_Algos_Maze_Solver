# 🤖 Genetic Algorithm for Maze Solvin

🧩 This project implements a **Genetic Algorithm (GA) to solve a maze** by evolving a population of possible paths towards the optimal solution. The algorithm uses selection, mutation, and crossover to navigate the maze efficiently.

## 🚀 Project Features
- 🧠 **Genetic Algorithm-based pathfinding**
- 🔀 **Mutation and crossover operators to evolve solutions**
- 🖥 **Visualization of the best-found path**
- ⚙️ **Configurable population size and generations**

## 📥 Installation & Setup
1️⃣ Clone this repository:
```bash
git clone https://github.com/your-username/maze-solver.git
```
2️⃣ Navigate to the project folder:
```bash
cd maze-solver
```
3️⃣ Install dependencies:
```bash
pip install matplotlib deap numpy
```

## 🏗 Maze Representation
- 🏠 **Start Position**: (0,0)
- 🎯 **Goal Position**: Bottom-right corner
- 🧱 **Walls** represented as `1`
- 🚶 **Open paths** represented as `0`

## ⚙️ Genetic Algorithm Details
- 🔄 **Selection**: Tournament selection
- 🔀 **Crossover**: Uniform crossover
- 🔬 **Mutation**: Random direction changes
- 🎯 **Fitness Function**: Uses Manhattan distance to goal

## ▶️ Running the Project
Run the script to start the Genetic Algorithm:
```bash
python maze_solver.py
```

## 📊 Example Output
- ✅ **Best path found at key generations (2, 10, 50, 100, 500)**
- 🎨 **Final best path is visualized** with:
  - 🟩 **Green**: Start Position
  - 🟥 **Red**: End Position
  - 🔵 **Blue**: Path Taken

## 🔧 Configuration
Modify the `run_ga` function to adjust parameters:
```python
def run_ga(generations=2000, pop_size=50):
    pop = toolbox.population(n=pop_size)
```

## 🤝 Contributing
Feel free to **fork the repository** and submit **pull requests** with improvements.

## 📜 License
This project is licensed under the **MIT License**.

---
🌟 **Contributions are welcome!** Feel free to fork, modify, and submit a pull request.

