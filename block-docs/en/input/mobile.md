# palette.user-input.mobile

> **Note:** These blocks only work on iOS and Android. They have no effect on other platforms (or return 0/-1/useless values).

# accelerometer -- Accelerometer Value

Returns the current values for the [accelerometer]($pedia/mobile-accelerometer/).

**Portrait Orientation**

Name | Description
--- | ---
X (Positive) | Right
X (Negative) | Left
Y (Positive) | Up
Y (Negative) | Down

**Landscape Orientation**

Name | Description
--- | ---
X (Positive) | Up
X (Negative) | Down
Y (Positive) | Left
Y (Negative) | Right

# swipe-detect -- Swiped

Returns `true` if the user has swiped [up/down/left/right]. A swipe is defined as touching the screen, sliding the finger and then releasing.

{ notes }

#### Alernate Approach: Events

![swipe-event](https://static.stencyl.com/help/images/mobile-input-5.png)

We recommend using a swipe event instead of a swipe block. It's easier to work with.