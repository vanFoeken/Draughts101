Draughts101

International draughts (10x10) with AI.

“Game”:  white or black.
“AI”:  1-5.

-Undo move.
-Moveable on/off.
-Rotate board.

Classes (3):
1. Board (main)
Light board with dark tiles (only dark tiles are used so there aren't any light ones).

main -> JFrame

2. Game
Loop and logic.

-turn -> get pieces (white and black), get moves and maxCapture -> gameover or move (mouse or MinMax).
-move -> do move (animation) and return new color.

ActionListener -> undo move
MouseListener -> player move

3. MinMax
Basic minimax algoritme with alfa beta pruning.
Uses bitboards for faster calculations and HashMap (board, value) to prevent dubble.
1 depth = 2 moves -> depth == 0 continues as long as maxCapture > 0.
