# DIGITAL EMPOWERMENT PAKISTAN
This repository includes all tasks included in the internship program for a period of 4 weeks.

## WEEK 1: TIC- TAC-TOE GAME USING MINIMAX ALGORITHM
In a game of tic-tack-toe, the goal is to get 3 crosses/circles consecutively in a row/column or diagonally. Here, I have implemented a simple game using the minimax algorithm where the computer plays against the user.
### STEPS:
1.	The output of the game is displayed in a typical tick-tack-toe format and the program checks if a space has been filled beforehand.
   
2.	We specify the conditions required to win the game i.e: to get 3 crosses consecutively in a row/column/diagonally.
   
3.	We construct the minimax algorithm. X would be the mini player, trying to minimize the final score and O would be the max player, trying to maximize the final score. If max_checking is True, it is the player’s turn and if it is False, it’s the computer’s turn.
   
4.	When it’s the computer’s turn to play, it iterates all the places on the board where an O can be placed. It recursively calls the minimax function with max_checking set to True to simulate the player’s response.

5.	When it’s the player’s turn, it iterates all the places on the board where an X can be placed. It recursively calls the minimax function with max_checking set to False to simulate computer’s response.

6.	Based on this logic, the computer only makes the best move according to the best_score.

7.	If conditions are met by X, then player wins. If conditions are met by O, then computer wins. If the board space is filled, and no conditions are met then it’s a tie.

### RESULTS:
Below we see how the output looks like:

### SCENARIO 1:
<p align="center">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Game_tied.png" width="500">
</p>

### SCENARIO 2:
<p align="center">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Computer_won.png" width="500">
</p>
