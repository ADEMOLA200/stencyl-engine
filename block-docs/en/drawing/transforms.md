# draw-transtoby -- Move Pen (Drawing Origin)

Moves the origin point of drawing to or by the specified amount.

**To** = Sets to the specified amount.<br/>
**By** = Adds the specified amount to the existing amount.

# to-screen-space -- Switch to Screen Space

By default, when drawing on actors, the coordinates are relative to the actor. This blocks switches the origin point of drawing to screen coordinates. This allows you to draw HUD's and other graphics that are anchored to the screen (and are unaffected by the camera).

# to-local-space -- Switch to Actor Space

Moves the origin point of the drawing to match the position of the specified actor.

# set-drawing-layer -- Set Drawing Layer

Set the layer for drawing.

# set-drawing-layer-scene -- Draw on Scene

Set the layer for drawing to the HUD layer, above all other layers.

# set-drawing-layer-actor -- Draw on Layer with Actor

Set the layer for drawing to the layer with the specified actor.