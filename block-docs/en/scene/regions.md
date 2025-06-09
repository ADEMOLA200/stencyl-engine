# palette.scenes.regions

> Read our guide on [Regions]($pedia/regions/) for an explanation of these blocks.

# region -- Choose Region

Returns a Region of choice (whether an instance of one, an attribute or other form).

# is-in-region -- Actor is Inside Region?

Returns `true` if the actor is inside the specified region.

# create-region -- Create Box Region

Creates a rectangular region with the given location and size. Assign to a Region attribute (using the "Last Created Region" selection) to refer to it in the future.

# create-circular-region -- Create Circle Region

Creates a circular region with the given location and size. Assign to a Region attribute (using the "Last Created Region" selection) to refer to it in the future.

# delete-region -- Delete Region

Deletes a region from the current scene. (It will return if you leave the scene and come back.)

# move-region -- Move Region

Moves the region to the given point.

# follow-region -- Move Region to Actor

Moves the region to the given actor's location using its origin point.

# reset-region -- Reset Region Size

Resets the region to its original size.

# resize-region1 -- Resize Circle Region

Sets the size of a circular region to the given diameter.

# resize-region2 -- Resize Box Region

Sets the size of a box region to the given width and height.

# get-region-pos -- Position of Region

Gets the [X/Y] location of the region.

# get-region-size -- Width / Height of Region

Gets the [Width/Height] of the region.