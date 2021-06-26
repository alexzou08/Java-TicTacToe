![x wins1](https://user-images.githubusercontent.com/84696428/123515070-b695b580-d6c8-11eb-9f25-b55c0e05d079.png)
![o wins2](https://user-images.githubusercontent.com/84696428/123515073-bac1d300-d6c8-11eb-961b-b51fee11b2e1.png)
![tie](https://user-images.githubusercontent.com/84696428/123515076-bc8b9680-d6c8-11eb-8642-b59fa2efa590.png)
![2D Array Indicies](https://user-images.githubusercontent.com/84696428/123515078-bdbcc380-d6c8-11eb-991c-423c055947f2.png)
# Java_Udacity_Project1_TicTacToe
Rules of the Game
Tic-Tac-Toe is a 2 player board game. One player is X and the other player is O. The game starts with an empty 3x3 grid with 9 cells. The players take turns marking each cell with either an X or an O. The goal for the X player is to get 3 X’s in one line either vertically, horizontally or diagonally. The goal for the O player is to get 3 O’s in one line either vertically, horizontally or diagonally.

Once a line is formed the game ends and the player who formed that line wins!

Sometimes there is no winner. This occurs when all of the cells are filled in but there is no line of 3 X's or 3 O's. This often happens, especially when both players are good. In this case, this game ends as a tie.

Code design
The source code includes 2 main Java files, Game.java and GameUI.java.

Game.java is where all the game logic code exists.
GameUI.java is where all the user interface code exists. You can take a look at GameUI.java if you like, but it is not necessary to change any code there to complete the project.
Your job is to implement the checkGameWinner() function in the Game.java file.

String checkGameWinner(char [][] grid) has a 2D char array as an input representing the game grid (see below for details) and it returns a String message indicating which player has won (X wins , O wins, Tie, or None if the game hasn't ended yet)

doChecks() is another function that is responsible for calling checkGameWinner every time a player takes a turn, so you should not worry about fitting this function into the rest of the program, this is already taken care of.

Requirements
In checkGameWinner() you should access those cells in the 2D array to find out if X or O has won the game by checking if there’s 3 of the same kind in a row either horizontally, vertically or diagonally!

If you detect a winner, set the variable result to either “X wins” or “O wins” depending on the player who won.
If the game ends as a tie, set result to “Tie.”
If the game has not ended yet set result to “None.”
Then make sure the function returns that variable result at the end (you can also return the string literal directly as you detect a winner or tie).
