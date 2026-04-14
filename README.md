🧩 Sudoku Solver (Python - AI Based)
📌 Description

This project is a Sudoku Solver developed in Python that uses advanced Artificial Intelligence techniques to solve 9×9 Sudoku puzzles. The solver treats Sudoku as a Constraint Satisfaction Problem (CSP) and applies efficient algorithms like Backtracking, Arc Consistency (AC-3), Forward Checking, and Heuristics (MRV & LCV) to find solutions. It can handle puzzles of different difficulty levels and also tracks performance using backtracking statistics.

🎯 Project Objectives

The main objectives of this project are:

To implement a Sudoku solver using AI techniques
To understand and apply CSP (Constraint Satisfaction Problem) concepts
To optimize solving using heuristics and constraint propagation
To analyze algorithm performance using tracking metrics
⚙️ Technologies Used
Programming Language: Python
Concepts Used:
Constraint Satisfaction Problems (CSP)
Backtracking Algorithm
Arc Consistency (AC-3)
Forward Checking
Heuristics (MRV & LCV)
🧠 Working Explanation

This Sudoku solver works in multiple stages to efficiently reach the solution:

1. Input Reading
The program reads Sudoku puzzles from text files
Each file contains a 9×9 grid
Empty cells are represented using 0
2. Constraint Setup
Each cell is treated as a variable
Possible values (1–9) are assigned as domains
Constraints ensure:
No repetition in rows
No repetition in columns
No repetition in 3×3 subgrids
3. Arc Consistency (AC-3)
Applied before search begins
Removes inconsistent values from domains
Reduces the search space and improves efficiency
4. Backtracking Search
The main solving algorithm
Assigns values recursively
Backtracks when a constraint is violated
Ensures a correct solution is found if it exists
5. Heuristics Optimization

To improve performance, two heuristics are used:

MRV (Minimum Remaining Values):
Selects the variable with the fewest remaining values
LCV (Least Constraining Value):
Chooses the value that restricts neighbors the least
6. Forward Checking
After assigning a value, invalid options are removed from neighboring cells
If any cell has no possible values left, the algorithm stops early and backtracks
📂 Project Files
SUDOKU GAME.py → Main Python solver file
EASY.txt → Easy level Sudoku
MEDIUM.txt → Medium level Sudoku
HARD.txt → Hard level Sudoku
HARD2.txt → Additional hard puzzle
▶️ How to Run the Project

Follow these steps to run the solver:

Clone the repository
Open the project folder
Run the Python file using:
python "SUDOKU GAME.py"

The program will automatically solve all input files and display results.

🖥️ Output

The output includes:

Solved Sudoku grid
Performance statistics:
Total backtracking calls
Total failures
🔍 Key Functions Overview
read_sudoku() → Reads puzzle from file
print_board() → Displays Sudoku grid
get_neighbors() → Defines constraints
initialize_domains() → Sets possible values
ac3() → Applies arc consistency
revise() → Removes inconsistent values
select_unassigned_variable() → Implements MRV
order_domain_values() → Implements LCV
forward_check() → Applies forward checking
backtrack() → Core solving algorithm
solve_sudoku() → Controls full execution
📊 Performance Tracking

The project includes performance analysis using:

Backtrack Calls: Number of recursive attempts
Backtrack Failures: Number of unsuccessful paths

This helps evaluate efficiency of the algorithm.

🚀 Features
Solves Sudoku puzzles of varying difficulty
Uses AI-based optimization techniques
Efficient constraint handling
Performance tracking included
Supports multiple input files
📚 Learning Outcomes

Through this project, you can learn:

How to model problems as CSP
Implementation of AI search algorithms
Use of heuristics to improve performance
Problem-solving and algorithm design skills
🔮 Future Improvements
Add graphical user interface (GUI)
Allow user input puzzles
Add difficulty generator
Visualize solving steps
Convert into web or mobile app
👨‍💻 Author

Developed by: AAIRUS IRFAN
