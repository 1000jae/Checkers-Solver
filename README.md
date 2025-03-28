# Checkers

Project for CSC384 offered by University of Toronto Mississauga, Fall 2024.
Tests, Source Code, and Description were given by the course.

Goal: Find the best result for the red players using Alpha-Beta Pruning.

Pieces:
- "R" or "B": king pieces (move all directions)
- "r" or "b": single pieces (move forward only)

Rules:
1. Red starts at the bottom three rows and Balck starts at top three rows. 
2. Movements:
    - simple move (move piece one square diagonally)
    - jump (move diagonally over an opponent's piece to "capture"/remove it)
4. Jumping is mandatory and prioritized over Simple moves. 
5. Multiple Jumps are done if possible. 
6. If a piece reaches the other end of the board, the piece becomes a King piece.
7. Player wins if all of the opponent's pieces are captured or if the opponent is not able to make any legal moves.


Input: each input is a state of an 8x8 board (64 characters). 
- ".": empty space
- "b" or "r": single piece
- "B" or "R": king piece

Output: all of the checkers board states for each move created as the two players play optimally. 

Command:
    python3 checkers.py --inputfile input_file --outputfile output_file
