# collision-foreach -- For each collision point ...

Loops over each collision point in the current collision event.

# collision-xynxy -- Collision Point

Returns the (x,y) position of the current collision point. Must be used within the `for each collision point...` wrapper.

# tile-data-for-collision -- Get Data for Collided Tile

Returns the text associated with the tile you collided with. Must be used within the `for each collision point...` wrapper.

> **What is this for?** You can [tag tiles]($pedia/tiles/) with textual data that can be accessed during game. For example, a lava tile could convey that it's deadly to the touch, or a healing tile in an RPG could heal the character passing over it.  
> ![tile-editor]($pedia/tiles-and-tilesets/tile-metadata.png)

# tile-position-for-collision -- Get Position for Collided Tile

Returns the column or row of the collided tile.

{ code }

```
$blockCode([tile-position-for-collision d:column]) //column
$blockCode([tile-position-for-collision d:row]) //row
```