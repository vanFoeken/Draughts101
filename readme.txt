Draughts101

International draughts (10x10) with AI.

“Game”:  white or black.
“AI”:  1-5.

-Undo move.
-Moveable on/off.
-Rotate board.

Classes (3):
1. Board
Light board with dark tiles in the center of a JFrame (main).

2. Game
Loop and logic.

-turn -> get pieces (white and black), get moves and maxCapture -> gameover or move.
-move -> do move (animation) and return new color.

ActionListener -> undo move
MouseListener -> player move

3. MinMax
Basic minimax algoritme with alfa beta pruning.

Uses bitboards for faster and HashMap (board, value) for no dubble calculations.

1 depth = 2 moves, when depth == 0 continues as long as maxCapture > 0.

