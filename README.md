## Link to the solver
[Link](https://avi4h.github.io/sudoku-solver/)

## How to Use
- **Enter Initial Sudoku State** : Start by entering the initial state of the Sudoku puzzle into the solver.
- **Click Submi**t : Once you've inputted the starting numbers, click the "Submit" button to initiate the solving process.
- **Get the Solution** : The solver will work to find the solution, and the solved Sudoku grid will be displayed once the solution is found.

## How it Works

A Sudoku solver uses backtracking and typically implements with recursive functions. Here's a short explanation of the key steps in the code:

1. **Select an Empty Cell** : Start by finding an empty cell (usually denoted by 0 or another placeholder) in the Sudoku grid. If no empty cells are left, the puzzle is solved.

2. **Try a Number** : Choose a number from 1 to 9 and attempt to place it in the empty cell.

3. **Check Validity** : Verify whether the chosen number violates the Sudoku rules in the current row, column, and 3x3 subgrid.

4. **Recursive Backtracking** : If the number is valid, move on to the next empty cell and repeat steps 2 and 3. If there are no valid numbers for the current cell, backtrack to the previous cell and try a different number. This process continues recursively.

5. **Repeat** : Continue trying numbers and backtracking until a solution is found or it's determined that no solution exists.

6. **Return Solution** : Once a solution is found, the algorithm returns the solved Sudoku grid.
   
The code recursively explores possible solutions by filling in cells and backtracking when it encounters an invalid placement. This process continues until a valid solution is found or all possibilities are exhausted.
