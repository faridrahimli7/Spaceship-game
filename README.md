This is a classic arcade-style game developed in Python, where the player controls a spaceship that can shoot missiles to destroy rocks. The game uses the SimpleGUI library and provides controls to move, rotate, thrust, and shoot missiles from the spaceship.

In this game, the player:

Controls a spaceship that can rotate, move, and shoot missiles.
Must avoid or destroy asteroids that appear randomly on the screen.
Gains points by hitting asteroids with missiles, and loses lives if they collide with asteroids.


Key Features
Spaceship Control: Rotate the spaceship left and right, apply thrust to move forward, and shoot missiles.
Asteroids: Rocks spawn randomly, moving at various speeds and angles.
Missiles: The spaceship can shoot missiles in the direction it is facing.
Collision Detection: The game includes basic collision detection between the spaceship, missiles, and asteroids.


Game Controls
Arrow Keys:
  Left: Rotate spaceship counterclockwise.
  Right: Rotate spaceship clockwise.
  Up: Engage thrust to move forward.
Space: Fire a missile.

Game Logic
Thrust and Rotation: The spaceship accelerates in the direction it faces and slows down due to friction.
Missile Firing: Missiles are spawned at the ship's front, moving at a constant speed in the direction of the ship.
Asteroids: Spawn at random locations with random velocities and rotate, providing obstacles to avoid or destroy.
Screen Wrapping: Game elements wrap around the screen edges, creating a continuous play area.

Code Overview
ImageInfo Class: Stores information about game images, such as center, size, and lifespan.
Helper Functions: angle_to_vector for angle conversion and dist for calculating distances.
Ship Class: Defines the spaceship, handling drawing, movement, thrust, and missile shooting.
Sprite Class: Represents game objects like asteroids and missiles, handling movement and drawing.
Game Loop: The draw function updates game elements, spawns rocks, and manages collisions.
Event Handlers: keydown and keyup control spaceship movement and actions, while rock_spawner generates new rocks.
