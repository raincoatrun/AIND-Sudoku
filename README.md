# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Constraint Propagation is using local constraints in a space, like the constraints of each square, column, row and diagonal units to dramatically reduce the search space. Since each box only allows a single digit to occupy space, when same two digit appears in two boxes, we can conclude that either of a digit can appear in two space. Also, we can reason that no other box, within a unit constraint space can have either of the two digit, and we can call it "Naked Twins strategy". This enables us to eliminate possibilities and increase the efficiency of our algorithm.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: For the diagonal sudoku problem, we use the same constraint propagation method as for regular Sudoku. Here by adding two diagonal units like (column and row units) we further restrict the space. Thus we can use constraint propagation like column, row, square and diagonal constraints to solve the Sudoku.

 
### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
