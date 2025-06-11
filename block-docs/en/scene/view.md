# palette.scenes.view

> Read our article on [Backgrounds]($pedia/backgrounds-and-foregrounds/) and [Camera]($pedia/the-camera/) for an explanation of some of these blocks.

# screen-xy -- Camera Position

Returns the camera's horizontal (X) or vertical (Y) position.

# screen-wh -- Screen Size

Returns the game's screen width/height.

# camera-move -- Move Camera

Moves the camera to the given point.

# camera-follow -- Move Camera to Actor

Moves the camera to the given actor's location.

# shake-start -- Shake Screen

Shakes the screen for the specified time. Good for conveying explosions or earthquakes. Intensity specifies how "violent" the shaking is.

# shake-stop -- Stop Shaking Screen

Immediately stop shaking the screen.

# set-color-bg -- Set Background to Color

Changes the background color to a solid color (if you don't have an image background covering it up).

# set-grad-bg -- Set Background to Gradient

Changes the background color to a vertical gradient (if you don't have an image background covering it up).

# layer-exists -- Layer Exists

Returns true if a layer with the given name or ID exists.

# set-bg-speed -- Set Autoscroll Speed (for layer)

Changes the speed that the specified background layer (automatically) scrolls at. The layer must be designated as scrolling to begin with for this to work.

# set-layer-scrollfactor -- Set Scroll Factor for (for layer)

Change the speed at which any layer scrolls, as a percentage of the baseline. In other words, 100% is the original value, 200% is twice as much and 50% is half as much.

# showhide-layer2 -- Show / Hide Layer

Shows/Hides the given layer.

# fadeTo-layer2 -- Fade Layer

Fades the given layer to the specified opacity value (0 - 100%) over time.

# layer-alpha -- Opacity of Layer

Returns the opacity of layer (0% - 100%) with the given name or ID.

# set-blend-layer2 -- Set Blend Mode (for layer)

Set the [Blend Mode]($pedia/blending-modes/) for the specified layer.

# set-bg-image -- Change Background Image (for layer)

Change the image displayed in the specified background layer.

# create-tile-layer -- Create Tile Layer

Add a new layer for tiles and actors. Provide the name of the new layer and the drawing order (z-order). 0 is the back, higher numbers display on top.

# create-bglayer-from-bg -- Create a Background Layer

Add a new background layer. Provide the name, the name of the Background resource and the drawing order (z-order). 0 is the back, higher numbers display on top.

# create-bglayer-from-image -- Create a Background Layer (from image)

Add a new background layer using an image. Provide the image, name and drawing order (z-order). 0 is the back, higher numbers display on top.

{ code }

```
addBackgroundFromImage([IMAGE], true, [TEXT], [INT]); //tiled background
addBackgroundFromImage([IMAGE], false, [TEXT], [INT]); //regular background
```

# remove-layer -- Remove Layer

Remove the specified layer. The behavior of objects that still exist on this layer when it is removed is unspecified.

# set-layer-order -- Set Drawing Order for Layer

Set the drawing order of the specified layer. 0 is the back, higher numbers display on top.

# get-layer-order -- Get Drawing Order for Layer

Get the drawing order of the specified layer. 0 is the back, higher numbers display on top.

# numlayers -- Number of Layers

Returns the number of layers in the current scene.

# offscreen -- Set Offscreen Bounds

Used to set how far actors have to be off-screen to be considered off screen. Applies only to the current scene.

{ notes }

To preserve the offscreen bounds across all scenes, set the following Engine property:

```haxe
Engine.preservePadding = true;
```