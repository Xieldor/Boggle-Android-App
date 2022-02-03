# Test Plan

**Authors:**

**Team123: Tianfang Xie, Rakesh Jeyaraman, Weneyan Du**

The purpose of this document is to define the testing strategy, scope, resources, coverage, technology and the test scenarios required to do the testing activities of "A Simple Word Game Project" which is a
simple single player word game designed to run on android.

## 1 Testing Strategy

### 1.1 Overall strategy

This section describes the overall testing strategy followed in "A Simple Word Game Project". The primary objective of testing is to make sure all the requirements are working as expected and not deviating from the requirements specifications.
In order to achieve the same, all the requirements listed by George P. Burdell for this project is taken into account and the same are tested by different modules and also by using different testing types such as below:

  * Unit Testing
  * System Testing
  * Integration Testing
  * Regression Testing
  * User Acceptance Testing

- Unit Testing
    * What is it? - Testing done at method level. To make sure an implemented method does what it is supposed to do.
    * Who are all involved? - Developers who implements the method.
    * How it is done? - As the implementation is done using Java, unit level testing will be done manually in Android Studio Emulator and Android phone.

- System Testing
    * What is it? - Testing done at module level which are grouped together to achieve a specific piece of requirement.
    * Who are all involved? - Testers
    * How it is done? - Using manual testing. Testers will run the test cases written for system tests against each module.

- Integration Testing
    * What is it? - Testing done after putting together different modules to make sure the application is working by communicating across modules.
    * Who are all involved? - Testers
    * How it is done? - Using manual testing. Testers will run the test cases written for integration tests against all requirements.

- Regression Testing
    * What is it? - Testing the existing functions to make sure the iterative work done for a requirement did not impact the ones implemented already.
    * Who are all involved? - Testers
    * How it is done? - Using manual testing. Testers will run the test cases written for regression tests against application.

- User Acceptance Testing
    * What is it? - Testing done by the real time user to make sure the product/application is delivered as expected.
    * Who are all involved? - Testers, Developers and Customer
    * How it is done? - Using manual testing. Customer will play the game and check the application behavior.

### 1.2 Test Selection

As discussed above in the overall test strategy, different types of testing will be done by following the approaches below:

  * Unit Testing - Black box technique Manually
  * System Testing - Black Box technique using Manual Testing
  * Integration Testing - Black Box technique Manually
  * Regression Testing - Black Box technique Manually
  * User Acceptance Testing - Black box technique using Manual Testing

### 1.3 Adequacy Criterion

This section defines the quality of tests and the coverage provided for "A Simple Word Game Project".

  * Traceability Matrix - This helps in tracking the coverage of user requirements against the test cases. Based on the teams decision, any test management tool can be used for this purpose.
  * Test Coverage - Using static review techniques (Peer review, code walkthrough)

### 1.4 Bug Tracking

This section defines how the bugs are managed in this project.

The project will be using any test management tool or a spread sheet to keep track of the bugs and its status. A bug or a defect will be raised or created to address an issue in an application behavior when it fails.
to meet the expected result. It will be assigned to the developer for resolution and the same will be tracked with proper comments and checking its validity (if its a real bug).

### 1.5 Technology

Below are the list of technologies planned to be used in this Project

  * Java
  * SQLite


## 2 Test Cases



| S.No | Test Case Description                                     | Test Steps                                                | Expected Result                                                  | Actual Result                                                   | Test Status | Comments/Defect ID's |
| ---- | --------------------------------------------------------- | --------------------------------------------------------- | ---------------------------------------------------------------- | --------------------------------------------------------------- | ----------- | -------------------- |
| 1    | Verify if the application displays home page              | Power on the android device                               | Application should display the home page with 5 options          | Application displays the 5 options upon opening the Application | PASS        |                      |
|      |                                                           | Tap the word game Application                             |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 2    | Verify the user is able to start a Game                   | Power on the android device                               | Application should display the game board                        | Application displays game board with timer counting down        | PASS        |                      |
|      |                                                           | Tap the word game Application                             |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap play a word Game                                      |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 3    | Verify the user is able to view statistics                | Tap the word game Application                             | Application should allow the user to view different statistics   | Application lets the user to view different statistics          | PASS        |                      |
|      |                                                           | Tap view statistics                                       | based on user Selection                                          |                                                                 |             |                      |
|      |                                                           | Tap game score statistics                                 |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap back to go back to previous screen                    |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap word statistics                                       |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap home button                                           |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 4    | Verify the user is able to adjust the game settings       | Tap the word game Application                             | Application should allow the user to perform different actions   | Application allows the user to adjust settings                  | PASS        |                      |
|      |                                                           | Tap adjust the game settings                              | in the settings screen                                           |                                                                 |             |                      |
|      |                                                           | Modify the default settings                               |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap the back button                                       |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap adjust the game settings                              |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap set it to default                                     |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 5    | Verify the user is able to exit the Application           | Tap the word game Application                             | Application should allow the user to close/exit                  | User is able to exit the Application                            | PASS        |                      |
|      |                                                           | Slide down/up to close the Application                    |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap the close link                                        |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 6    | Verify the user is able to exit the word Game             | Tap the word game Application                             | Application should allow the user to exit the Game               | User is able to exit the Game                                   | PASS        |                      |
|      |                                                           | Tap play a word Game                                      |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap back button                                           |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap play a word game again                                |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap close or exit link/button                             |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 7    | Verify the user is able to play a Game                    | Tap the word game Application                             | Application should allow the user to play a game and display     | User is able to play a game successfully                        | PASS        |                      |
|      |                                                           | Tap play a word Game                                      | a score at the end                                               |                                                                 |             |                      |
|      |                                                           | Enter a word until the timer is counted down to 0         |                                                                  |                                                                 |             |                      |
|      |                                                           | View the score                                            |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 8    | Verify the score is calculated properly when the User     | Tap the word game Application                             | Application should allow the user to do any actions and displays | Scores are calculated as per the requirements                   | PASS        |                      |
|      | performs different actions                                | Tap play a word Game                                      | scores correspondinly                                            |                                                                 |             |                      |
|      |                                                           | Enter a word using the displayed letters                  |                                                                  |                                                                 |             |                      |
|      |                                                           | Enter nothing and submit                                  |                                                                  |                                                                 |             |                      |
|      |                                                           | Enter a single letter and submit                          |                                                                  |                                                                 |             |                      |
|      |                                                           | Enter a word randomly without using the displayed letters |                                                                  |                                                                 |             |                      |
|      |                                                           | Enter a word by duplicating the displayed letters         |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 9    | Verify the user is able to re-roll the board              | Tap the word game Application                             | Application should allow the user to reroll the game board       | User is able to reroll and points 5 are deducted                | PASS        |                      |
|      |                                                           | Tap play a word Game                                      | by deducting 5 points                                            |                                                                 |             |                      |
|      |                                                           | Enter a word using the displayed letters                  |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap reroll board                                          |                                                                  |                                                                 |             |                      |
|      |                                                           | view the points for the User                              |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 10   | Verify the board is displayed with vowels (1/5) and consonants (4/5)  | Tap the word game Application                             | Application should display the game board with vowels and        | Application displayed the board with vowels and consonants as expected                                                               |     PASS        |                      |
|      |                                                           | Tap play a word Game                                      | consonants as per the requirements                               |                                                                 |             |                      |
|      |                                                           | View the board displayed for the Game                     |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 11   | Verify the player is not allowed to enter values outside  | Tap the word game Application                             | Application should not allow the user to change the settings     | Application didn't allow beyond max range                       | PASS        |                      |
|      | the range                                                 | Tap adjust settings                                       | beyond the maximum range                                         |                                                                 |             |                      |
|      |                                                           | Set the game end time to 10 mins                          |                                                                  |                                                                 |             |                      |
|      |                                                           | Set the board size to 10                                  |                                                                  |                                                                 |             |                      |
|      |                                                           | Set the weight to 10                                      |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 12   | Verify the timer is counted down when the game is in      | Tap the word game Application                             | Application should keep counting down as longs the game is in    | Timer is counted down properly when game is in progress         | PASS        |                      |
|      | progress                                                  | Tap play a word Game                                      | progress                                                         |                                                                 |             |                      |
|      |                                                           | View the timer count                                      |                                                                  |                                                                 |             |                      |
|      |                                                           | Hide the application in the background                    |                                                                  |                                                                 |             |                      |
|      |                                                           | Resume the application                                    |                                                                  |                                                                 |             |                      |
|      |                                                           | Check the timer is still counting down                    |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 13   | Verfiy the word is counted only if the letters are        | Tap play a word Game                                      | Application should increase the points when the  word is formed  | Only adjacent letters are accepted                              | PASS        |                      |
|      | adjacent to the next                                      | Select the letters adjacent to the next horizontally      | using letters adjacent to the next ones                          |                                                                 |             |                      |
|      |                                                           | or vertically                                             |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap submit button                                         |                                                                  |                                                                 |             |                      |
|      |                                                           | Check points                                              |                                                                  |                                                                 |             |                      |
|      |                                                           | Select the letters adjacent to the next diagonally        |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap submit button                                         |                                                                  |                                                                 |             |                      |
|      |                                                           | Check points                                              |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 14   | Verify the points are deducted when the user selects      | Tap play a word Game                                      | Application should reduce 5 points                               | Application reduces 5 points upon reroll                        | PASS        |                      |
|      | to reroll the board                                       | check the points for the User                             |                                                                  |                                                                 |             |                      |
|      |                                                           | Select reroll                                             |                                                                  |                                                                 |             |                      |
|      |                                                           | Check the points                                          |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 15   | Verify the points are not calculated if the word contains | Tap play a word Game                                      | Application should not increment the points for the User         | System displays message when letters not adjacent are selected  | PASS        |                      |
|      | letters that are not adjacent                             | check the points for the User                             |                                                                  |                                                                 |             |                      |
|      |                                                           | Enter a word by selecting letters not adjacent to next    |                                                                  |                                                                 |             |                      |
|      |                                                           | Submit the Word                                           |                                                                  |                                                                 |             |                      |
|      |                                                           | Check the points                                          |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 16   | Verify the game score statistics                          | Tap the word game application                             | Application should display the score statistics in               | Score stats are displayed as per requirements                   | PASS        |                      |
|      |                                                           | Tap view statistics                                       | descending order                                                 |                                                                 |             |                      |
|      |                                                           | Check the order in which the score is displayed           |                                                                  |                                                                 |             |                      |
|      |                                                           | check the entry for other statistics                      |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 17   | Verify the word game statistics                           | Tap the word game Application                             | Application should display the word statistics                   | Word stats are displayed as per requirements                    | PASS        |                      |
|      |                                                           | Tap view statistics                                       |                                                                  |                                                                 |             |                      |
|      |                                                           | check the word statistics                                 |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 18   | Verify the user can access the settings by selecting a score   | Tap the word game Application                             | Application should display the game settings after selecting     | System displays game settings upon tapping a score              | PASS        |                      |
|      |                                                     | Tap view statistics                                       | a score from statistics screen                                   |                                                                 |             |                      |
|      |                                                           | select the game score                                     |                                                                  |                                                                 |             |                      |
|      |                                                           | check the settings for that score                         |                                                                  |                                                                 |             |                      |
|      |                                                           |                                                           |                                                                  |                                                                 |             |                      |
| 19   | Verify the responsiveness of the Application              | Tap the word game application                             | Application should respond without any latency                   | Application responds without any latency                        | PASS        |                      |
|      |                                                           | Tap play a word Game                                      |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap return to main menu                                   |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap view settings                                         |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap return to main menu                                   |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap view statistics                                       |                                                                  |                                                                 |             |                      |
|      |                                                           | Tap return to main menu                                   |                                                                  |                                                                 |             |                      |
