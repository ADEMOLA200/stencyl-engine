# palette.scenes.shaders

> Read our guide on [Shaders]($pedia/shaders/) for an explanation of these blocks.

# shader-apply -- Apply Shader

Applies the specified shader to the game. This replaces the existing shader. To use multiple shaders at a time, use the combine shader blocks below.

# shader-clear -- Clear Shaders

Removes the existing shader from the game.

# shader-hud -- Toggle shaders for HUD layer

Enables/disables shaders for the HUD (top, non-scrolling) layer.

# shader-combine -- Combine 2 Shaders

Combines 2 shaders together. If combining more than 2, stick further combines in the second slot.

# shader-combine3 -- Combine 3 Shaders

Combines 3 shaders together.

# shader-combine4 -- Combine 4 Shaders

Combines 4 shaders together.

# shader-file -- Load Shader from File

Loads a shader placed into a game's **extras** directory.

# shader-text -- Load Shader from Text

Define a shader inline using [GLSL](https://en.wikipedia.org/wiki/OpenGL_Shading_Language).

# shader-set -- Set Shader Property

Instantly set a shader's properties. This lets you tweak a shader (in ways that the blocks don't allow) and alter its appearance after creation.

Consult our [Shaders article]($pedia/shaders/) for property names.

# shader-tween -- Tween a Shader Property

Change a shader's properties over time. Consult our [Shaders article]($pedia/shaders/) for property names.

# shader-time -- Set Time Scale for Shader

Makes animated shaders run faster/slower. Useful for porting shaders written for other environments. 1.0 is normal time. 2.0 is twice as fast.

# shader-hue -- Hue

Adjusts the screen's hue in degrees.

# shader-csb -- Contrast / Saturation / Brightness

Adjust the screen's contrast, saturation or brightness, in percentages. 100% means original value, 200% means twice as much, 50% means half as much.

# shader-tint -- Tint

Apply a color-based tint to the screen using the specified opacity in pecentage between 0% (no tint), 100% (full tint).

# shader-filters -- Filters (Grayscale / Inverse / Sepia)

Apply simple filters (grayscale, inverse, sepia) to the screen.

# shader-blur -- Blur

Applies a directional blur to the screen. x/y collectively define a 'slope' for the direction, so -1,-1 is a diagonal blur.

# shader-sharpen -- Sharpen

Sharpen with the given intensity.

# shader-bloom -- Bloom

Causes highlights (bright areas) to bleed and glow.

# shader-grain -- Grain

Apply a dynamic, film grain effect to the screen.

# shader-scanline -- Scanlines

Apply TV-like scanlines to the screen.