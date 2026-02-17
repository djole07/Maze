# Pathfinding Optimization in Stohastic Grid-Based Environment

## Abstract
The goal is to visualize best action in each cell on the board. Board consist of 4 types of cells:
1. Regular (has reward of -1)
2. Teleport (same reward as Regular, but can transfer you *from* (**f0, f1,...**) one cell *to* (**t0, t1,...**) another)
3. Trap (has big negative reward)
4. Wall (obstacle, user cannot go through it)
5. Terminal - the goal

Also, for added complexity, each action has certain probability to be applied. In this example, we have "wind", which means that there is a chance that player would be dragged to the right after every chosen action.

For every cell on the map, there is an estimated value of that cell, as well as best action to choose in that cell.
<img width="600" height="452" alt="image" src="https://github.com/user-attachments/assets/50828720-3aae-431e-9392-5229c2d2c49f" />


<img width="609" height="416" alt="image" src="https://github.com/user-attachments/assets/5bf540a0-3f19-4d9a-87e6-5bb7aeec61f3" />



## Technical Implementation

The implementation is contained within a **Jupyter Notebook** environment, facilitating both the execution of the pathfinding algorithms and the visualization. Solution is based on both **Value iteration** and **Policy iteration** in regular and stohatic variant.

User can generate a board of with custom dimmensions, while also changing parameters such as _number of iterations_ of algorithms, _gamma_ factor that is decay factor and enabling 'wind'

## Usage
1. **Initialize Environment:**
   ```bash
   git clone https://github.com/djole07/Maze.git
   cd Maze
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
