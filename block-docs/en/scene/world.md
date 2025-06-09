# grav-xy -- Get Value of Gravity

Returns the value of the Horizontal (X) or Vertical (Y) components of gravity. Gravity is a force that is applied to all actors (that are affected by it).

# setgrav -- Set Gravity

Sets the world's gravity.

# scene-wh -- Scene Width / Height

Returns the current scene's [width/height] in [pixels/tiles].

# scenename -- Scene Name

Returns the current scene's name.

# tile-wh -- Tile Width / Height

Returns the current scene's tile width/height.

# tile-coord-at -- Convert to Tile Coordinates

Converts a coordinate from pixels (real location) to tiles. In other words, divides the coordinate by the tile width or height respectively.

# set-tile-at2 -- Set a Tile

Sets a tile at the given position and layer.

# tile-exists-at2 -- Does a Tile exist at location?

Returns `true` if any tile exists at the given position and layer.

# tileID-at2 -- Get ID for Tile at location

Returns the ID of the tile at the given position and layer, or -1 if no tile found.

# tileCollisionAt2 -- Does a solid tile exist at location?

Returns `true` if ANY collision shape exists. If layer ID is -1, loops through all layers.

# tileColID-at2 -- Get Collision ID for tile at location

Returns the ID of the collision shape for the tile at this position and layer, or -1 if no tile found.

# tilesetID-at2 -- Get Tileset ID for tile at location

Returns the ID of the tileset for the tile at this position and layer, or -1 if no tile found.

# remove-tile-at2 -- Remove tile at location

Remove the tile at this position.

# tile-data-at2 -- Get Metadata for tile at location

Get the tile data for the tile at this position. Returns empty text if no tile found.