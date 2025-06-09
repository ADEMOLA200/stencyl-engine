# palette.actors.effects

> Read our article on [Effects]($pedia/effects/) and [Blend Modes]($pedia/blending-modes/) for an explanation of these blocks.

# set-blend-actor -- Set Blend Mode

This block sets an actor's blend mode. [Blend Modes]($pedia/blending-modes/) control how a game draws semi-transparent graphics.

# apply-filter -- Apply Effect

Applies the specified effect to the actor. Effects stack on each other in the order they were added.

# clear-filter -- Remove all Effects

Removes all effects from the actor.

# filter-tint -- Tint using Color

Applies a "tinting" effect to an actor given a color and a percentage amount (where 0 means no tint and 100 means that the actor is completely colored).

# filter-hsb -- Hue

Shifts the hue of the actor, given an amount in degrees. The full spectrum spans 0 - 360 degrees inclusive and wraps around if you exceed that in either direction.

# filter-sat -- Saturation

Adjust how "vivid" the actor's colors are in relative percentage amounts. 0% would make an actor grayscale. 100% would restore the default saturation. 200% would make it look very vivid.

# filter-bright -- Brightness

Adjust how bright (or dark) the actor is in relative percentage amounts. 0% means total darkness. 100% is the default. 200% would make it brighter than usual.

# filter-grayscale -- Grayscale

Makes the actor draw in grayscale.

# filter-negative -- Negative

Inverts the actor's colors.

# filter-sepia -- Sepia

Applies an "old photograph" look to the actor. Sort of like grayscale but with a tinge of brown.
