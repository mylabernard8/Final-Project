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

## setup()
- Set up canvas
  - createCanvas(800,600)
- Create the 'Matter.js' engine and world
- Define both gravity and the other engine options
- Add in the floor, walls, and platforms using the 'Platform' and 'Boundary' classes
- Add in the initial ball using the 'Ball' class
- Add in the spawnButton (UI button) to add in new balls


## draw()
- Update the Matter.js engine:
    - Engine.update(engine)
- Clear the background
- Loop through each array (balls, platforms, etc.) and call .show() to draw
- Check if any balls are off-screen, and remove them if necessary
- Optionally display the number of balls or a message when the screen is empty

## Classes
- Ball:
    - Properties:
      - this.body - a Matter.js circle body
      - this.r - radius
    - Actions:
      - show() - draws the ball at its current position
      - isOffScreen() — returns true if the ball falls out of view
        
- Platform:
   - Properties:
      - this.body — a static rectangle body
      - this.w
      - this.h
      - this.angle
  - Actions:
      - show() — draws the platform with rotation

- Boundary:
   - Properties:
      - this.body — a static rectangle
      - this.w
      - this.h
  - Actions:
      - show() — draws walls/floor





