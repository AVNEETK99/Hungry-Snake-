# Hungry-Snake

Snake is a classic arcade game that originated in the 1970s and became popular in the 1990s with the release of Nokia mobile phones. The objective of the game is to control a snake on a game board, guiding it to eat food while avoiding obstacles such as walls and its own tail. As the snake eats more food, it grows longer and the game becomes progressively more difficult.

The game typically features a simple, two-dimensional graphics and is controlled using the arrow keys or other directional buttons. There are many variations of the game available today, including mobile versions and browser-based versions that can be played for free online. The game is considered a classic and remains popular today as a simple and addictive form of entertainment.

## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type ```python snake.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* First, the necessary modules are imported - ```Pygame, time, and random```.

* The Pygame library is initialized using ```pygame.init()```.

* Some color variables are defined in RGB format for later use in the game.

* The width and height of the game display screen are defined, and a new Pygame display surface is created using ```pygame.display.set_mode()```.

* The game clock is initialized using ```pygame.time.Clock()```.

* Two variables snake_block and snake_speed are defined to set the size of the snake block and the speed of the game, respectively.

* Two font variables font_style and score_font are defined to set the style of the text used in the game.

* Two functions are defined, ```Your_score()``` and ```our_snake()```, which respectively display the player's score and draw the snake on the game screen.

* Another function ```message()``` is defined to display a message on the game screen.

* The main game loop function ```gameLoop()``` is defined, which is the heart of the game.

* Inside the ```gameLoop()```, various game variables are initialized such as the snake's position, the length of the snake, and the position of the food.

* The game then enters a loop that runs until the player quits the game or loses the game.

* The loop first checks for any input events, such as key presses or mouse clicks.

* If the player hits a wall or collides with the snake's tail, the game_over flag is set to True, and the game_close flag is set to True.

* If the game_close flag is True, the game displays a message to the player indicating that they have lost and prompts them to either play again or quit the game.

* If the player chooses to play again, the ```gameLoop()``` function is called again.

* If the player chooses to quit the game, the game_over flag is set to True, and the game loop ends.

* If the player hits the food, the snake's length is increased by one, and a new random position is generated for the food.

* The game then updates the game display by redrawing the snake and the food and displaying the player's score.

* Finally, the game clock is ticked, and the Pygame library is quit when the game loop ends.

* The ```gameLoop()``` function is called to start the game.
