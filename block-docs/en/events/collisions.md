# events.collisions

> Read our [Collisions article]($pedia/collisions-and-groups/) for an explanation of these events.

# collide -- Something Else

Triggers when this actor collides with any other actor.

# event-collide-actortoactor -- Specific Actor

Triggers when the specified actor collides with any other actor. For example, you could use this to detect a switch being pressed.

# event-collide-actortotype -- Actor of Type

Triggers when an actor of the specified Actor Type collides with any other actor.

# event-collide-actortogroup -- Actor of Group

Triggers when an actor of the specified Actor Group collides with any other actor.

# event-collide-typetotype -- Type and Type

Triggers when actors of the specified Actor Types collide. 1st actor corresponds to the actor in the first blank. 2nd actor corresponds to the actor in the second blank. Like the following...

![example]($pedia/collisions-and-groups/image16.png)

# event-collide-grouptogroup -- Group and Group

Triggers when actors of the specified Actor Groups collide. 1st actor corresponds to the actor in the first blank. 2nd actor corresponds to the actor in the second blank.