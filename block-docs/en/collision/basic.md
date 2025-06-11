# palette.collisions.basic

## Actor 1 vs. Actor 2

Each block in this section lets you choose between Actor 1 and Actor 2. Collision events involve 2 actors. When the event is reported, the first actor in the event's block corresponds to Actor 1 and the second actor in the block corresponds to Actor 2.

![explained](https://static.stencyl.com/pedia2/blocks/collision/basic/1st2nd.png)

You can refer to Actor 1 and Actor 2 directly using the blocks embedded in the event itself.

![explained-more]($pedia/collisions-and-groups/image16.png)

# collision-top,collision-left,collision-bottom,collision-right -- Top / Left / Bottom / Right Side was Hit

Returns `true` if the actor's [top/left/bottom/right] side was hit. If the collision shape is not a box, we still approximate the shape as a box to calculate this.

{ images }

$blockImage([collision-top 0 0])
$blockImage([collision-left 0 0])<br/>
$blockImage([collision-bottom 0 0])
$blockImage([collision-right 0 0])

{ code }

```
$blockCode([collision-top 0 0])
$blockCode([collision-left 0 0])
$blockCode([collision-bottom 0 0])
$blockCode([collision-right 0 0])

$blockCode([collision-top 0 1])
$blockCode([collision-left 0 1])
$blockCode([collision-bottom 0 1])
$blockCode([collision-right 0 1])
```

# collision-shape-group2 -- Group of Colliding Shape

Returns the group of the shape for the "other" (or "second") object in the collision. In most cases, the group of the shape is the same as that of the actor, but that [isn't always the case]($pedia/collisions-and-groups/).

# collision-type2 -- Hit an Actor / Terrain / Tile / Sensor

Returns `true` if the "other" (or "second") object in the collision was an [actor / terrain region / tile / sensor].

{ code }

```
$blockCode([collision-type2 0 0 0])
$blockCode([collision-type2 0 0 1])
$blockCode([collision-type2 0 0 2])
$blockCode([collision-type2 0 0 3])
```