# die -- Kill Actor

Immediately kills the specified actor.

If killing the current actor from its own actor behavior, the remaining logic will continue to run. We recommending using the stop block to prevent errors from happening in this case.

# kill-leave-screen -- Kill Actor (after leaving screen)

Instructs the game to kill the actor if it exits the screen. This is useful for "bullets" and other temporary actors that aren't of much use to hold around once they're off the screen.

# isalive -- Is Actor alive?

Returns `true` if the specified actor is alive. Useful for checking prior to performing operations with that actor -- working with a dead actor may cause the game to crash.

# get-wh -- Get Width / Height

Returns the width or height of the actor.

# getatype -- Get Actor Type

Returns the actor's Actor Type.

# getgroup -- Get Group

Returns the actor's (Collision) Group.

# pick-type -- Choose Actor Type

Returns the chosen Actor Type.

# pick-group -- Choose Actor Group

Returns the chosen Actor Group. Useful for making comparisons in collision events.

# pick-type-by-name -- Get Actor Type (from name)

Retrieves an Actor Type by name and returns it if it exists.

# group-setresponse -- Set Collision Response

Override the default collision response between two groups.

# ignore-screen-tolerance2 -- Make Actor Always / Sometimes Active

Normally, actors stop updating after they're off-screen. This block can turn that option off and makes them always active no matter where they are. Choosing "sometimes" sets the actor to the default behavior.

# bullet-mode2 -- Toggle Continuous Collision Detection

Toggles whether an actor travels through terrain at high speeds.

# addshape-rectangle -- Add Rectangle Collision Shape

Adds a new box collision shape to the actor's current animation.

# addshape-circle -- Add Circle Collision Shape

Adds a new circle collision shape to the actor's current animation.

# addshape-polygon -- Add Polygon Collision Shape

Adds a new polygon collision shape to the actor's current animation. Specify the points using the next ``vertex`` block right below.

# addshape-vertex -- Add Point to Polygon Shape

Adds a point to the newly created polygon collision shape. Must be used in the `add polygonal collision shape` block above.

# foreach-shape -- For Each Collision Shape...

Lets you perform certain actions on each collision shape for the actor. Use the `make the shape solid / a sensor`, `remove the shape` and `scale the shape` blocks below.

# shape-sensorsolid2 -- Make Collision Shape Solid / Sensor

Sets the collision shape to be solid or a sensor (not solid but still can detect collisions).

# shape-destroy2 -- Remove Collision Shape

Removes the collision shape from the actor.

# shape-scale2 -- Resize Collision Shape

Resizes the collision shape in percentage terms, relative to the original size (100%).

# shape-group -- Get Collision Group for Shape

Returns the collision group assigned to a shape. Normally the group of the actor type the shape is attached to.

# shape-setgroup -- Set Collision Group for Shape

Sets the collision group for this shape.

# shape-last-added -- Last Added Shape

Returns the last collision shape added to the actor.

# actor-set-prop -- Set Actor Value

Associates a value with the given text key. Useful for storing (and later retrieving) arbitrary data in an actor without having to do this through other means in the toolset.

# actor-get-prop -- Get Actor Value

Returns the value that is associated with the given text key, if available. Returns `null` if it doesn't exist.