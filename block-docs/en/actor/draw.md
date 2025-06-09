# getanim -- Current Animation

Returns the current animation for the actor.

# setanim -- Switch Animation

Changes the animation for the actor to the specified one.

# is-anim -- Is an Animation playing?

Returns `true` if the actor's current animation is still playing. This is only relevant for non-looping animations since looping ones will always return `true`.

# set-frame -- Set Frame # for Animation

Sets the frame (by index) for the actor's current animation.

# get-frame -- Get Current Frame #

Returns the index of the current frame in the actor's current animation.

# get-num-frames -- Get Number of Frames in Current Animation

Returns the number of frames in the actor's current animation.

# get-frame-duration -- Get Duration of Current Frame

Returns the duration (in milliseconds) of the current frame in the actor's current animation.

# set-frame-duration -- Set Duration of Current Frame

Sets the duration (in milliseconds) of the current frame in the actor's current animation.

# getlayer -- Get Layer ID

Returns the ID of the layer that this actor is part of.

# getlayername -- Get Layer Name

Returns the name of the layer that this actor is part of.

# setlayer2 -- Switch Layer by ID / Name

Changes an actor's layer by either specifying the Layer ID or Layer Name. You can find both pieces of info in the Scene Designer's Layers Pane.

# backforward -- Switch Layer

A user-friendly way of making adjustments to an actor's layer. Can move to front/back/forward 1 layer/back 1 layer.

# movewithinlayer -- Switch Drawing Order (within layer)

A user-friendly way of making adjustments to an actor's **drawing order** (z-order) within a layer. Can move to front/back/forward 1 layer/back 1 layer.

# zindex -- Get Drawing Order (within layer)

Returns an actor's **drawing order** (z-order) within its layer.

# setzindex -- Set Drawing Order (within layer)

Sets an actor's **drawing order** (z-order) within its layer. This lets you make fine-tuned adjustments to layering without introducing a more layers to the game.

# actorswithinlayer2 -- Number of Actors within Layer

Returns the number of actors in the specified actor's layer. Can specify by Layer ID or Layer Name. You can find both pieces of info in the Scene Designer's Layers Pane.

# toggle-image -- Show / Hide Sprite

Makes the actor invisible or visible. Everything else about the actor still works, and the `[actor] is on screen` block will still return `true`.

# set-opacity -- Set Opacity

Sets the actor's opacity (alpha) value, which controls how "transparent" the actor is. Value must be between [0 - 100] inclusive. 0 means fully transparent. 100 is the default.

# get-opacity -- Get Opacity

Returns the actor's opacity (alpha) value as a value between [0 - 100] inclusive.

# anchor-screen -- Anchor Actor to Screen

Moves the actor to the HUD layer, which is on top of all regular layers. The actor will ignore the camera, so when the screen scrolls, the actor will still remain in the same place.

# unanchor-screen -- Unanchor Actor from Screen

Moves the actor back from the HUD layer.