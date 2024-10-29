The Boggle module implements a Boggle game solver in Elixir. The core function, boggle/2, takes a board (2D tuple) and a list of words, returning a map of words that can be constructed from the board, along with the list of their positions.

Key parts:

Word Search (boggle/2): Iterates over each word, converting it to a list of characters and initiating a depth-first search on the board. The search checks if each word can be formed by connecting adjacent letters.
Depth-First Search (dfs_board): Finds the starting coordinates of the first letter in each word, then passes these to recursive_checker.
Recursive Checker (recursive_checker/4): Checks if each remaining letter in the word sequence can be found by exploring neighboring cells, ensuring letters are not reused.
Neighbor Check (check_around/4): Evaluates all adjacent cells to see if the next character matches, returning the next coordinate if a match is found.
Helper Functions: Includes utility functions to check values in specific cells and manage recursion over the board.
This solution supports finding multiple words with complex board traversal.
