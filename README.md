


<body>
  <h1>Pacman Game Implementation using Turtle Module in Python</h1>
  <h2>Importing Required Modules:</h2>
  <ul>
    <li><code>randrange</code> and <code>choice</code> from the <code>random</code> module: Used for generating random numbers and making random choices.</li>
    <li><code>Turtle</code> from the <code>turtle</code> module: Used for creating graphical objects and animations.</li>
  </ul>
  <h2>Setting up the Game State:</h2>
  <ul>
    <li><code>state</code> dictionary: Keeps track of the score for Pacman and the ghosts.</li>
    <li><code>path</code>, <code>writer</code>, and <code>writer2</code> objects: Used for drawing and displaying text on the screen.</li>
    <li><code>aim</code> vector: Represents the direction in which Pacman is moving.</li>
    <li><code>pacman</code> list: Contains the position vector and movement vector for Pacman.</li>
    <li><code>pacman2</code> vector: Represents the position of the second Pacman.</li>
    <li><code>ghosts</code> list: Contains the position vector and movement vector for the ghosts.</li>
    <li><code>tiles</code> list: Represents the game map with different tiles, where 0 represents walls and 1 represents available paths.</li>
  </ul>
  <h2>Helper Functions:</h2>
  <ul>
    <li><code>square(x, y)</code>: Draws a square at the given coordinates (x, y).</li>
    <li><code>offset(point)</code>: Returns the index of the tile in the <code>tiles</code> list corresponding to the given point.</li>
    <li><code>valid(point)</code>: Checks if a given point is valid within the game map.</li>
  </ul>
  <h2>Game Initialization:</h2>
  <ul>
    <li>Set up the game window and initialize the necessary objects.</li>
    <li>Set the background color to black.</li>
  </ul>
  <h2>Game Logic:</h2>
  <ul>
    <li>The <code>move()</code> function is the main game loop that updates the positions of Pacman, ghosts, and the game state.</li>
    <li>It checks if the next move is valid and updates the positions accordingly.</li>
    <li>If Pacman or the second Pacman collects a point (represented by a tile with a value of 1), the score is incremented, and the tile is marked as collected.</li>
    <li>If Pacman collides with a ghost, the game ends.</li>
    <li>The <code>move()</code> function is called repeatedly using the <code>ontimer()</code> function to create animation.</li>
  </ul>
  <h2>User Input:</h2>
  <ul>
    <li>The <code>change(x, y)</code> function is called when the user presses the arrow keys.</li>
    <li>It changes the aim vector of Pacman to move in the desired direction if the move is valid.</li>
  </ul>
  <h2>Game Setup and Event Handling:</h2>
  <ul>
    <li>Set up the game window, set the screen update rate, and hide the turtle cursor.</li>
    <li>Create the writer objects for displaying the scores.</li>
    <li>Set up event handlers for user input.</li>
  </ul>
  <h2>Drawing the Initial World and Starting the Game:</h2>
  <ul>
    <li>Draw the game world based on the <code>tiles</code> list.</li>
    <li>Call the <code>move()</code> function to start the game loop.</li>
  </ul>
  <h2>Game Over:</h2>
  <ul>
    <li>When the game ends, the <code>done()</code> function is called to close the game window.</li>
  </ul>
</body>
