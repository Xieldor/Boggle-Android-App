# Design information for the assignment


>  1.When the application is started, the player may choose to (1) Play a word game, (2) View statistics, or (3) Adjust the game settings.

To realize this requirement, I added "Game", "Statistics" and "Settings" to the register class to represent the player's different choices.


>  2.When choosing to adjust the game settings, the player (1) may choose for the game to end after a certain number of minutes, from 1 to 5, defaulting to 3, (2) may adjust the size of the square board, between 4(x4) and 8(x8), defaulting to 4, and (3) may adjust the weights of the letters of the alphabet between 1 and 5, defaulting to 1.

To realize this requirement, I added several attributes to the Setting class, and I gave the initial values for them as the default values.

>  3.When choosing to play a word game, a player will:
Be shown a ‘board’ of randomly generated letters.
Be shown a timer counting down the number of minutes available for the game, as set in the settings.
Start with 0 points, which is not required to be displayed during the game.
Until the game timer counts to zero and the game ends:
Enter a unique word made up of two or more letters on the board.  The word must contain only letters from the board that are each adjacent to the next (horizontally, vertically, or diagonally) and a single letter on the board may not be used twice.  The word does not need to be checked against a dictionary (for simplicity, we will assume the player enters only real words that are spelled correctly).
or
Choose to re-roll the board at a cost of 5 points.  The board will be re-created in the same way it is generated at the start of each game, replacing each letter.  The timer will not be reset or paused.  The player’s score may go into negative values.
or
Choose to exit the game early.
At the end of the game, when the timer has run out or the player chooses to exit, the final score for the game will be displayed.
Each word will score 1 point per letter (‘Qu’ will count as 2 letters), and the cost for each board reset will be subtracted.
After the player views the score, they will continue back to the main menu.

To realize these requirements, I added a interface ShowBoard to show the board of randomly generated letters.
I also added a linterface ShowTimer to show the timer.
I added a boolean attribute ended_game to the "Game" class, if the timer counts to zero, the game will end.
I let the "Game" class to calculate the current score, the "Player" class will get the final score for this player and I also created a interface to show the final score.
I also added a "WordScore" class to calculate the wordscore and the number of time that the word has been entered.
After the final score has been shown, the player can start another round of choices.

>  4.Whenever the board is generated, or re-generated it will meet the following criteria:
 The board will consist of a square full of letters.  The square should have the number of letters, both horizontally and vertically, indicated by the size of the square board from the game settings (4x4, 5x5, 6x6, 7x7, or 8x8).  
⅕ (rounded up) of the letters will be vowels (a,e,i,o,u). ⅘ will be consonants.
The letter Q will be displayed as ‘Qu’ (so that Q never appears alone).  
The location and particular letters should be randomly selected from a distribution of letters reflecting the weights of letters from the settings.  A letter with a weight of 5 should be 5 times as likely to be chosen as a letter with a weight of 1 (assuming both are consonants or both are vowels).  In this way, more common letters can be set to appear more often.
A letter may appear on the board more than once.

To realize these requirements, I added several attributes to the "Board" class, letter_number can calculate the number of letters, number of vowel number and consonant number are also calculated. The boolean contain_letter_Q will check if the board contains the letter Q.
The weights of letters can be modified in the settings, and the choices of these letters will be implemented in this class.

>  5.When choosing to view statistics, the player may view (1) game score statistics, or (2) word statistics.

To realize these requirements, I added two classes such as "GameScoreStatistics" and "WordStatistics".

>  6.For game score statistics, the player will view the list of scores, in descending order by final game score, displaying:
The final game score
The number of times the board was reset
The number of words entered in the game
The player may select any of the game scores from this list to view the settings for that game’s board size, number of minutes, and the highest scoring word played in the game (if multiple words score an equal number of points, the first played will be displayed).

To realize these requirements, I added several attributes to the class "GameScoreStatistics", and I built connections between the class "Settings" and "WordScore".

>  7.For the word statistics, the player will view the list of words used, starting from the most frequently played, displaying:
The word
The number of times the word has been played, across all games

To realize these requirements, I added several attributes to the class "WordStatistics".

> 8.The user interface must be intuitive and responsive.

This is not represented in my design, as it will be handled entirely within the GUI implementation.

> 9.The performance of the game should be such that students do not experience any considerable lag between their actions and the response of the application.

This is not represented in my design, as it will be handled within the implementation method.

> 10.For simplicity, you may assume there is a single system running the application.

I have used this kind of assumption.

