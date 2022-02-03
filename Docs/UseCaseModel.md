# Use Case Model

**Authors:**

**Team123: Tianfang Xie, Rakesh Jeyaraman, Weneyan Du**

## 1 Use Case Diagram

![Use Case Diagram](https://github.gatech.edu/gt-omscs-se-2020spring/6300Spring20Team123/blob/master/GroupProject/images/Use%20Case%20Diagram.png)

## 2 Use Case Descriptions

Play Game
- Requirements: The application should allow the player to view a square board showing letters. The application shall also begin the time countdown. After the player clicking the re-roll button, the letters on the board should be refreshed. When the time countdown reaches zero, the game will be automatically shut down, and the final score of the game will be shown on the screen.
- Pre-conditions:
	* The player must launch the app.
	* The player must press the "PLAY GAME" button on the screen.
	* The app must generate the board by using the initial condition of the game settings.
	* The app must begin the time countdown based on the initial condition of the game settings.
	* Based on the letter weight of the game settings, the app should choose the corresponding letters and randomly show them on the board.
- Post-conditions:
	* The final game score must be automatically shown on the screen when the time countdown reaches zero.
	* The letters on the board must be refreshed when the player press the re-roll button.
	* The player can only choose the letter adjacent to the previous letter (horizontally, vertically, or diagonally).
- Scenarios:
	* The player presses the "PLAY GAME" button on the screen.
	* The time countdown begins and the square board with letters will be generated to let the player choose word.
	* The player choose the letters to generate a right word, the screen will show the letters that has been chosen.
	* After the player press the "SUBMIT WORD" button, the score of current word will be calculated.
	* If the player press the "RE-ROLL" button, the game board will be refreshed with new letters, the time countdown will not be reset or paused.
	* If the player press the "Exit" or the time countdown reaches zero, the final score of the game will be shown on the screen.
	* Then the player can choose to view the statistics or restart the game or return to the mainmenu by clicking different buttons.
	
  
Change game Settings
- Requirements: The application should allow the player to change the game settings, the player can choose the game time, the board size and decide the weight for each letters.
- Pre-conditions:
	* The player must launch the app.
	* The player must press the "ADJUST SETTINGS" button on the screen.
	* The app must show the spinner to let the player choose the corresponding value of each setting.
- Post-conditions:
	* The final chosen results should be shown at each spinner.
	* The new game should use these setting after press the "PLAY GAME" button.
	* If the player exit the game and replay the game, the app should use the last game settings.
- Scenarios:
	* The player presses the "ADJUST SETTINGS" button on the screen.
	* If the player wants to change the game time, the player needs to make a choice from the spinner shown after the word "Game End Time" and press the "SUBMIT SETTINGS" button.
	* If the player wants to change the board size, the player needs to make a choice from the spinner shown after the word "Board Size" and press the "SUBMIT SETTINGS" button.
	* If the player wants to change the letter weight, the player needs to choose a letter from the spinner shown after the word "Letter Weight" and choose the corresponding weight value from the next spinner. Finally, the player needs to press the "SUBMIT SETTINGS" button.
	* If the player wants to reset all the settings and return to the default settings, the player can click the "RESET SETTINGS" button.
	* After all changes have been made, the player needs to press the "RETURN TO MENU" to return to the main menu.
	* If the player wants to reset all the initial settings and clean all the game data, the player can click the "RESET DATABASE" button on the mainmenu, a warning dialog will be shown to double check the request. If the player press the "OK" button, the database will be regenrated to reset all the settings and game data.
	
	
View game statistics
- Requirements: The application should allow the player to view the game statistics information, the player will view the list of scores and view the list of words used.
- Pre-conditions:
	* The player must launch the app.
	* The player must press the "VIEW STATISTICS" button on the screen.
- Post-conditions:
	* The game statistics information should be shown on the screen.
	* If the player click the score information, the corresponding game setting and word information will be shown.
- Scenarios:
	* The player presses the "VIEW STATISTICS" button on the screen.
	* The player can choose to press the "SCORE STATISTICS"button or the "WORD STATISTICS" button to view the score statistics or the word statistics.
	* The screen will show the list of scores and the list of words used.
	* The player can click on the list or scores to see the corresponding game settings and other detailed information.
	* After viewing the statistics information, the player needs to press the "RETURN TO MENU" to return to the main menu.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MzQ2MjczNF19
-->
