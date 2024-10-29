Boggle defines a function to solve Boggle puzzles using efficient board traversal and recursive word search. The core function boggle takes a 2D list (the board) and a list of words, outputting a list of words found along with their coordinates on the board.

Key Functions:
boggle: Converts the board into an Array and builds a character-to-coordinates map using dfsBoardHelper. For each word, it checks if it can be constructed by finding connected characters on the board.
dfsBoardHelper: Scans the board, mapping each character to its coordinates, optimizing lookups for starting positions of each letter.
recursiveChecker: Recursively searches from a starting position to check if the subsequent letters in the word can be connected through valid adjacent positions, ensuring no position is reused within a single search.
checkAround: Given a position, it filters neighboring coordinates to find matches for the next letter in the word, excluding previously visited blocks.
listToBoardArray: Converts the board from a list of lists to an array for efficient indexing.
The implementation leverages efficient data structures and recursion, allowing for generalized board sizes and word lists.
