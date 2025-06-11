# events.basics.basics -- ""

# init -- When Creating

Happens just once -- when this behavior is first initialized. For an actor, this happens when the actor is created. For a scene, this happens when you enter the scene.

> **Tip:** If some logic needs to run at the "beginning" of a scene but *after* the scene's actors and behaviors finished initializing, use a `do after 0.01 seconds` block to accomplish this.

# draw -- When Drawing

All drawing code goes here. Happens once every frame. The number of frames per second (FPS) is variable, capped at 60 frames per second. 

# step -- When Updating

The "meat" of a behavior's logic goes here. Happens for every step of the game. A step happens every 10 milliseconds, therefore there are 100 steps per second.