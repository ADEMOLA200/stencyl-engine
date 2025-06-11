# get-dxy -- Get Speed

Returns the current [X / Y] speed for the actor.

# set-dxy -- Set Speed

Sets the [X / Y] speed for the actor.

# setvel -- Set Velocity (given Direction and Speed)

Sets the actor's velocity, given a direction and a magnitude (speed) rather than X/Y components like above.

# push-shove -- Push (given X/Y)

Pushes (or shoves) an actor, given an X/Y direction and force. Shoving is more "forceful" than pushing - experiment and see which works better for you.

# push-shove2 -- Push (given Angle)

Pushes (or shoves) an actor, given an angle and force. Shoving is more "forceful" than pushing - experiment and see which works better for you.

# twist -- Twist (rotate using force)

Twists (applies torque) to an actor, given a force.

# getangvel -- Get Turning Speed

Returns the turning speed (angular velocity) of the actor (in degrees).

# setav -- Set Turning Speed

Sets the turning speed (angular velocity) of the actor (in degrees). Positive turns clockwise. Negative turns counter-clockwise.

# toggle-grav -- Toggle Gravity

Enables or disables gravity for this actor.

{ code }

```
[ACTOR].setIgnoreGravity(false); //enable gravity
[ACTOR].setIgnoreGravity(true); //disable gravity
```

# toggle-rot -- Toggle Rotation

Enables or disableds rotation for this actor. 

# set-fric-bounce -- Set Friction / Bounciness

Sets the actor's friction and bounciness settings. Provide a value between [0.0 - 1.0] inclusive.

Read our [Physics guide]($pedia/working-with-physics/) for an explanation of what these fields mean.

# get-fric-bounce -- Get Friction / Bounciness

Gets the actor's friction and bounciness settings.

Read our [Physics guide]($pedia/working-with-physics/) for an explanation of what these fields mean.