# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

In my case DFS is typically more efficient for solving Sudoku puzzles because it focuses on a single path until a solution is found or backtracking is needed, reducing memory usage compared to BFS. BFS, is more exhaustive but is more memory-intensive, which is better for finding multiple solutions, though this is rare in Sudoku.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The choice of a stack for DFS and a queue for BFS directly changes the traversal order: DFS traverses deeper paths first, while BFS traverses all nodes at a level before moving deeper. Alternatives like priority queues or recursion (DFS) can achieve similar objectives, and design patterns like constraint propagation or heuristic-driven searches (A*) can improve functionality by focusing on promising paths.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

The Sudoku solver can be adapted for larger puzzles or other grid-based games by optimizing constraint-checking mechanisms, implementing heuristic-driven searches, and using advanced techniques like recursive backtracking with memoization. Using more memory efficent languagues might also help for larger puzzles.  Lessons from this assignment—such as the importance of efficient algorithms, problem-specific heuristics, and modular design—are important for real-world like challenges in scheduling.