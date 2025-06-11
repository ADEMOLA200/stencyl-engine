# palette.images.show-images

> Read our [Image API]($pedia/image-api) guide for an explanation of these blocks.

# image-inst-create -- Create Instance of Image

Creates an Image Instance from the given image. Usually assigned to an attribute right away.

# image-inst-actor -- Attach Image Instance to Actor

Attaches the image instance to the specified actor at the given position.

{ code }

```
$blockCode([image-inst-actor "" "" 0 0 0]) // front
$blockCode([image-inst-actor "" "" 0 0 1]) // behind
```

# image-inst-layer2 -- Attach Image Instance to Layer

Attaches the image instance to the specified layer (via ID or name) at the given position.

{ code }

```
$blockCode([image-inst-layer2 "" 0 0 0 0 0]) // front
$blockCode([image-inst-layer2 "" 0 0 0 0 1]) // behind
```

# image-inst-hud -- Attach Image Instance to Screen

Attaches the image instance to the HUD layer at the given position. This will make it draw in front of everything and ignore the camera.

# image-inst-remove -- Remove Image Instance from Parent (the thing it is attached to)

Takes the image instance out of the game (by removing it from the object it is attached to).

# image-set-z -- Set Z-Order for Image Instance

Sets the drawing order (within the layer/actor) for the image instance.

# image-set-z-friendly -- Send Image Instance to Different Layer

Sets the drawing order (within the layer/actor) for the image instance in a user-friendly way.

# image-get-z -- Z-Order for Image Instance

Returns the drawing order (within the layer/actor) for the image instance.

# image-set-props0 -- Set Position for Image Instance

Sets the position of the image instance (relative to the actor/layer it is attached to).

# image-set-props1 -- Set Direction (Angle) for Image Instance

Sets the direction (angle, in degrees) of the image instance (relative to the actor/layer it is attached to).

# image-set-props2 -- Resize an Image Instance

Sets the width and height (in percentage) of the image instance. 100% keeps that dimension the same. 200% will double it. 50% will halve it.

# image-origin -- Set Origin Point for Image Instance

Sets the origin (pivot) point for the image instance. This affects how it's scaled and rotated.

# image-get-props -- Get Position / Direction / Scale / Opacity for Image Instance

Returns various properties for the image instance.

# image-tween-slide -- Slide an Image Instance

Slides (moves) the image instance over the specified time.

# image-tween-spin -- Spin an Image Instance

Spins (rotates) the image instance over the specified time.

# image-tween-fade -- Fade In / Out an Image Instance

[Fades In / Fades Out] the image instance over the specified time.

# image-tween-scale -- Grow / Shrink an Image Instance

Resizes the image instance in percentage terms over the specified time. 100% keeps that dimension the same. 200% will double it. 50% will halve it.

# image-blend -- Set Blend Mode for Image Instance

Changes the blending mode for the image instance.

# image-apply-filter -- Apply Effect to Image Instance

Applies the specified effect to the image instance. The effect persists until removed, so you do not need to call this each frame.

# image-clear-filter -- Remove All Effects from Image Instance

Removes all effects from the image instance.