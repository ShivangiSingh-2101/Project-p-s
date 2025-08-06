program 1-  Tic tac toe game 
Summary:
This is a simple two-player Tic-Tac-Toe game implemented in Python. 
The game uses a 1D list of 9 elements to represent the 3×3 grid.
Players take turns placing "X" or "O" in empty positions by entering a number between 1 and 9.
The game checks for a win, a tie, and switches players accordingly. 
It ends when someone wins or the board is full.

 Algorithm (Step-by-Step):
1. Initialize the Game
- Create a list board with 9 "–" symbols representing empty spaces.
- Set cp = "X" to start with Player X.
- Set a gameRunning = True flag.
2. Main Game Loop
- While gameRunning is True:
- Display the board (gameboard()).
- Take player input (playerinput()):
- Ask for input between 1–9
- If valid and empty, place the player's symbol.
- Else, print an error message.
- Check for a tie (checkTie()):
- If no "-" left on the board, declare tie and stop game.
- Check for a win (checkwin()):
- If a row, column, or diagonal has the same symbol (and not "-"), declare the winner and stop the game.
- Switch the player (SwitchPlayer()):
- Change "X" to "O" or "O" to "X".
3. End of Game
- If someone wins: display the winner.
- If it's a tie: display "It is a tie".
