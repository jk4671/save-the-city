# Save the City

<p align="center">
 <img src="https://github.com/user-attachments/assets/7932bf5c-72aa-4a52-9925-c7ae7d7d9b05" alt="Main page" width="300">
 <img width="300" alt="Game screen" src="https://github.com/user-attachments/assets/50832e9d-fdfb-4a4f-8201-ad068fd6caff">
 <img width="300" alt="Final screen" src="https://github.com/user-attachments/assets/39b39fbe-3ec3-4799-800d-2ad2bdb2ca03">
</p>

The goal of the project was to incorporate newly learned concepts about callbacks, timer events, keyboard buttons, collision detection, inheritance, classes, and class global variables to design my own interactive video game using the Turtle module and various shapes and scenes drawn using L-system strings. To design my own game, I created a class named MyGame, with the player’s pixel movement, enemy number, and collision radius as parameters, in the file named mygame, which processed information to simulate my game. In the constructor of MyGame class, I created various instance variables: a TurtleInterpreter object created from the previous project, Screen object, main player Turtle object, player’s pixel movement, list of enemy Turtle objects, number of enemies in the list, minimum and maximum x positions that game enemies can occupy, the total number of enemies created, collision radius, score counting Turtle object, total score, explosion marking Turtle object, status of the game, and win or lose status of the player. Then, I created various methods to manipulate the instance variables based on different scenarios of the game as well as the user’s keyboard button input and timer events. Using the MyGame class, as well as the turtle, random, and time module and turtle_interpreter, home, doneDraw, and beginDraw files, I designed my own game called “Save the City.” The game allows the user to use up, down, left, and right keys to control a basket to catch a number of deployed bombs, depending on the level of the game, in Chicago. To win the game, the user has to catch at least 50% of the bombs deployed.

## Demo

https://youtu.be/jydmbxwM8mU

## Design

### Game Instructions

Depending on the level of the game you choose, you will be given a certain number of bombs that move down the screen at various steps. Use your arrow keys (left, right, up, down) to control the basket to catch the bombs that are deployed from the air. If you catch at least 50% of the deployed bombs, you win. You have 30 seconds to play the game. If you need to exit the game while bombs are being deployed, press the “Q” keyboard button.  

#### Start Phase

In the start phase of the game, I use command-line user input to let the user choose the level of the game (1, 2, or 3). Then, I display the start phase (Required Image 1) which contains the name of the game, game instructions, and how-to instructions for exiting the screen in the middle of the game. The start phase transitions into the main phase automatically.

#### Main Phase

The user is given 30 seconds to play the game. While the bombs are dropping from the sky, use the basket to hover over the bombs to catch them before they land. The number of bombs caught are displayed on the moon (Required Image 2). Your score is the number of bombs caught in the air. However, you will only win the game if the number of bombs caught in the air is greater than those they were deployed but not caught.

#### End Phase

After 30 seconds, I change the game screen to the end scene (Required Image 3) which tells the user that time’s up and game’s over. Additionally, I tell the user how many bombs they caught, how many bombs they missed, and whether they won the game. At this point, the user can exit the game by clicking on x of the Turtle Screen object.

## Sources and collaborators

For the project, I imported the following libraries and gif files:

https://docs.python.org/3/library/random.html
https://docs.python.org/3.8/library/turtle.html
https://docs.python.org/3/library/time.html 
https://www.pinclipart.com/pindetail/iTxmRoo_explosion-clip-art-bomb-explosion-cartoon-png-transparent/
https://www.pinclipart.com/pindetail/xhJRxJ_bomb-svg-clear-background-bomb-clipart/
https://www.stickpng.com/img/objects/baskets/fruit-basket

