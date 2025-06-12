# draw-text -- Draw Text

Draws the specified text to the given location using the current font. Color and stroke settings do not apply to fonts.

# draw-line -- Draw Line

Draws a line from the starting point to the ending point, using the current stroke color and thickness.

# draw-pixel -- Fill Pixel

Draws a single pixel to the given location, using the current color. We recommend using the [Image API]($pedia/image-api) if you intend to fill many pixels at a time.

# draw-image-actor -- Draw Image for Actor

Draws the specified actor's image to the current pen position. Will base this upon the actor's current animation (and current frame). Still works if the actor is hidden. Useful for drawing things behind an actor.

{ notes }

#### Example

```design-mode { alt="draw image for actor example" img="draw-image-actor-example.png" }
[draw]
  [draw-transtoby d:by 25 0]
  [draw-image-actor c:this]
```

Draws the following.

![example](https://static.stencyl.com/pedia2/blocks/drawing/drawing/actor_example2.png)

# drawfill-rect -- Draw Rectangle

Draws an outline of (or fills) a rectangle at the specified position and size, using the current stroke color and thickness (and color for filling).

# drawfill-roundrect -- Draw Rounded Rectangle

Draws an outline of (or fills) a rounded rectangle at the specified position and size, using the current stroke color and thickness (and color for filling).

# drawfill-circle -- Draw Circle

Draws an outline of (or fills) a circle at the specified position and size, using the current stroke color and thickness (and color for filling).

# drawfill-poly -- Draw Polygon

Draws an outline of (or fills) a polygon at the specified position, using the current stroke color and thickness (and color for filling). Use the `add point to polygon` block to add points to the polygon.

{ code }

```
//draw
$blockCode([drawfill-poly d:draw])

//fill
$blockCode([drawfill-poly d:fill])
```

# add-to-poly -- Add Point to Polygon

Adds the specified point to the polygon. Must be used within the `draw a [oulined/filled] polygon` wrapper, and at least 3 points must be specified. You do not have to "close" the polygon by repeating the starting point.

# new-shape -- Create a New Shape

Creates a new, empty shape. When drawing an object that doesn't change every frame, drawing with a new shape every frame wastes efficiency. It's better to create a shape attribute for each of the individual objects you want to draw, and reuse them.

# draw-shape -- Draw a Shape

Update a shape's graphics, and draws the updated shape onto the screen. This block is required to use the other drawing blocks.