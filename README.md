# Snake-Solving-Algorithms

These are algorithms to solve the classic Snake game. While only "methodical_snake" is successful, though the others are fun to watch!

"methodical_snake" simply guides the snake along a circuit to solve the game. The snake follows the same path until it reaches the maximum possible length, at which point the game is solved.

"avoiding_snake" makes use of many if statements to understand the best way to avoid itself. For instance, if the snake head is moving left but encounters its body in its path, it will change course to go down. But if the snake encounters an obstacle both left and down, it will go up. Additionally, the snake does know where the food is, but will move in one direction until it is in line of food, then change course to eat it. This algorithm fails when the snake inevitably finds itself in a loop made of its own body.

"pathfinding_snake" knows there the food is and will find the shortest path to it. This algorithm is similar to A*, but does not predict obstacles, instead it handles obstacles as the snake head passes by them. This algorithm, like "avoiding_snake", fails when it finds iteself in a loop. 

"snake_up_and_to_the_left" was made by my friend. As the name suggests, the snake only moves up and left. It makes use of the "wrapping" capablity of the game, focusing on food first, moving until it is in line with the food, eating the food, then immediately turning left. It also knows to avoid itself, but will only turn up or left to do so. This algorithm fails when the snake has obstacles both directly above and to the left.

Improvements can be made by making a state machine. If the snake is unable to find a path to the food, it enters a survival mode to make the best use of limited space. I have also seen other programmers use artificial intelligence to train the snake to solve the game. This will be a fun challenge I intend to take once I have the knowledge.

While my friend and I made these algorithms, the code was borrowed from Github user "straker". Feel free to use these algorithms, but please give the original user credit. Their repository can be found here:
https://gist.github.com/straker/ff00b4b49669ad3dec890306d348adc4

