# Hangman Word Game

Hangman Word Game is a python terminal game that is being hosted in a mock terminal on [Heroku](https://www.heroku.com/?)

Users are given the option to either look at the rules or start the game upon first glance. Once the user has entered a username the Hangman game will start. Hangman is a word guessing game where the users play against a computer, where their objective is to figure out the randomly picked hidden word based only on how long the word is, and by guessing letters to find out if they exist in the word or not. However, the user only has 8 guesses to do so as a Hangman will slowly be drawn out for every failed guess until it is fully drawn, and the player has lost. The player can win by being able to fully guess every letter of the hidden words before they run out of guesses. Instructions for how the game works are provided in the main menu screen.

[Live link to Hangman Word Game](https://p3-hangman-word-game.herokuapp.com/) (Right click to open in a new tab)

![Image of Hangman Word Game on a wide range of devices](docs/am_i_responsive.png)

---

## CONTENTS
* [Flowchart](#flowchart)
* [Features](#features)
  * [Existing Features](#existing-features)
  * [Future Features](#future-features)

* [Technologies Used](#technologies-used)
  * [Languages Used](#languages-used)
  * [Frameworks, Libraries & Programs Used](#frameworks-libraries--programs-used)

* [Deployment](#deployment)

* [Testing](#testing)
    * [Validator Testing](#validator-testing)
    * [Solved Bugs](#solved-bugs)
    * [Unfixed Bugs](#unfixed-bugs)

* [Credits](#credits)

---

## Flowchart
![Image of the Flowchart made on Lucidchart](docs/flowchart.png)

- I made this flowchart when I was first trying to figure out how to go about making the hangman part of the program to get a better idea on how to approach it.
---
## Features

### Existing Features

Below are the main features that users will come across when they use the program and play the game. The terminal clears it self after every segment to make it clean and avoid having confusing/confliciting information on the screen.

- The main menu is displayed with a message asking for the users input. Depending on the input, either the game will start by asking for the users username, or they'll be shown the rules/instructions.
![Image of the main menu when you first run the program](docs/features/main_menu.png)


- If the users input is "2" then they will be taken onto the rules page where they will be getting instructed onto how the game works. When the user is finished reading the rule set, they can press "Y" to continue onto the game or press "N" to go back to the main menu.
![Image of the rules when you type "2" and hit enter on the program](docs/features/rules.png)

- If the users input is "1" on the main menu, or "Y" in the rule they will taken to the username screen where they are asked to input a username that is 2-10 letters long. There is user validation to make sure the usernames dont contain too little or too many characters, or with numbers.
![Image of the username screen where user is asked to enter their username](docs/features/username.png)

- When the game has been started, the user is shown blank spaces for the word they need to guess, how many guesses they have and a list for letters they have guessed. Once they have made their guess, they will be shown whether the letters was correct, wrong or invalid.
![Image of the Hangman game once it's been started by the user](docs/features/hangman_game.png)
- This image shows when the users input was correct
![Image of the Hangman game when the users input was correct](docs/features/correct_guess.png)
- This image shows when the users input was wrong
![Image of the Hangman game when the users input was wrong](docs/features/wrong_guess.png)
- This image shows when te users input was the same as a previous guess
![Image of the Hangman game when the users input was the same as a previous guess](docs/features/same_guess.png)

- The user has won by managing to correclty guess all the hidden letters to make out the full word. They have the option to continue playing and get a new hidden random word, or they can go back to the main menu
![Image of the Hangman game when the users won](docs/features/user_win.png)

- The user has has failed to make out the full word with all their guesses and have now lost the game. They have the option to continue playing and get a new hidden random word, or they can go back to the main menu.
![Image of the Hangman game when the user lost](docs/features/user_lost.png)

- The following will showcase the programs input validation for when the input is not valid.
    - Letter used when only "1" or "2" are valid inputs
![Image of the Hangman game when there is wrong input in the main menu](docs/features/wrong_input_menu.png)
    - Numbers used when only "Y" or "N" are valid inputs
![Image of the Hangman game when there is wrong input in the rule screen](docs/features/wrong_input_rules.png)
    - Numbers used together with username when it is not a valid input.
![Image of the Hangman game when there is wrong input in the username screen](docs/features/wrong_input_username.png)
    - Any input that is not 1 letter will not be valid, and you will be told so.
![Image of the Hangman game when there is wrong input in the hangman game](docs/features/wrong_input_hangman.png)
    - Any input that is not "Y" or "N" will not be valid"
![Image of the Hangman game when there is wrong input in the "win" screen](docs/features/wrong_input_win.png)
    - Any input that is not "Y" or "N" will not be valid"
![Image of the Hangman game when there is wrong input in the "lost" screen](docs/features/wrong_input_lost.png)
    

### Future Features

- Would like to add a hint for every word as it can be extremely difficult to guess words at time without any kind of clue.

- Being able to guess the whole word if you think you know it.

- Add colors and more ASCII to make it look more interesting than just a normal terminal.

---
## Technologies Used

### Languages Used

Python was the only language used in making this program.

### Frameworks, Libraries & Programs Used

- Git - For version control.

- GitHub - To save and store the files.

- Visual Studio on Gitpod/CodeAnywhere

- [Lucidchart](https://www.lucidchart.com/pages/) was used to sketch out the flowchart when I was first figuring trying to plan out how to make the game.

- [random](https://docs.python.org/3/library/random.html) library to get a random word from a list.

- [os](https://docs.python.org/3/library/os.html) library was used for the clearterminal function to make the terminal appear "cleaner".

- [Am I Responsive](https://ui.dev/amiresponsive) - To show the program hosted on on a wide range of devices.

---
## Deployment

[Heroku](https://www.heroku.com/?) was used to deploy a mock terminal of this program.

Steps for deployment: 

1. Clone or fork the repository for this project, [p3-hangman-game](https://github.com/Hakesh/p3-hangman-word-game)
2. Create a new Heroku app.
3. Set the buildpacks to Python and Nodejs, in that specific order.
4. Link the Heroku app to the cloned or forked GitHub Repository
5. Click on deploy

---
## Testing

I manually tested this project by doing the following:

* Using the [CI PYthon Linter / PEP8 Validator](https://pep8ci.herokuapp.com/#) to validate and confirm that there are no problems
* Testing the input methods by giving invalid inputs, numbers where strings are expected and vice versa.
* Tested on my local terminal and when uploaded to the Heroku mock terminal


### Validator Testing

* PEP8
    * No errors were returned when passing it through the [Code Insitute Python Linter](https://pep8ci.herokuapp.com/#)
    ![Image of the CI Python Linter](docs/ci_python_linter.png)

    
### Solved Bugs

- Unless you knew (or was lucky/smart to type the first letter for the word capitalized) that all the words inside of words_list are capitalized there was no way to win the game as it didn't take that into account. This was fixed by making both all the random words picked from the list uppercase, as well as the input when the user was typing in their guess.

- For every time that you would guess, the hidden word would duplicate it self. This was due to the fact that the variable that stores the hidden word was outside of the while loop which repeats itself after you guess. This was solved by moving the hidden_word variable to inside of the while loop.

### Unfixed Bugs

- Not really a bug as its more that I never implemented it, but if you decice to continue playing after winning or losing the hangman ascii art wont show until after you've done your first guess.

- The "Hello {username}" does not get cleared when playing the hangman game in the mock terminal on Heroku. It does when you play it on the IDE terminal however.

---

## Credits

- [How to build HANGMAN with Python in 10 MINUTES by Kite](https://www.youtube.com/watch?v=m4nEnsavl6w)
  - This video was useful as it gave me an idea on how to go about making the Hangman game part.

- [Clear Terminal code by Poke](https://stackoverflow.com/questions/2084508/clear-terminal-in-python)
  - Wasn't sure how to clear the terminal mid-program but Poke had an excellent reply to the original question. I turned his code
  into a function to make it easy to call upon for when i wanted to tidy up the terminal after certain segments in the game.

- [Hangman ASCII Art](https://codereview.stackexchange.com/questions/101968/hangman-with-ascii)
  - I found these ASCII drawings in another persons python hangman game and thought they looked neat.
