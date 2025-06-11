# palette.actors.tweening

> Read our article on [Tweening]($pedia/tweening/) for an explanation of these blocks.

# moveToBy -- Slide

Slides (moves) the actor by the given distance (or to the given location) over the specified time.

# spinToBy -- Spin

Spins (rotates) the actor [by / to] the given amount in degrees over the specified time. For the "to" case, it will always spin clockwise.

# fadeInOut -- Fade In / Out

Fades the actor [in / out] over the specified time. This means that its opacity will either go to 100% (fade in) or 0% (fade out).

{ code }

```
[ACTOR].fadeTo(1, [NUMBER], [EASING]); //fade in
[ACTOR].fadeTo(0, [NUMBER], [EASING]); //fade out
```

# fadeTo -- Fade To

Sets the actor's opacity to the given amount (in percent) over the specified time. Amount must be between [0 - 100] inclusive.

# scaleTo -- Grow / Shrink

Resizes the actor's width and height (in percentage terms) over the specified time. Amounts are relative to the actor's original size -- 100% means original size, 200% means twice the size, 50% means half the size.