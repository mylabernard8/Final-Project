# Final Project: Focusing on Physics Libraries

## Description:
- This project will have a single ball that bounces and rolls through a series of tilted platforms using real time physics. The user can click to spawn new balls in, which also reacts to gravity and the platforms. The balls motion is affected by friction and restitution/bounciness.


## Things I'm Modeling
- A 'Ball' class for dynamic bodies that bounce and roll and react
- A 'Platform' class for static and slightly tilted surfaces
- A 'Boundary' class for walls and the floor to keep the ball in bounds
- An optional 'Button'/ click function that will reset or spawn more balls

## Variables and Data Structures:
- Matter.js Core:
    - let Engine, World, Bodies
    - let engine, world
- Object collections:
    - let balls = ()
        - Array of bouncing balls
    - let platforms = ()
        - Slanted or flat surfaces/ platforms
    - let boundaries = ()
        - For walls and floors
    - let spawnButton
        - A button to add new balls
    - Physics:
        - Gravity
        - Restitution
        - Friction

