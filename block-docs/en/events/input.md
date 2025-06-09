# events.input

> Read our articles on [Controls]($pedia/controls/), [Touch & Gestures]($pedia/mobile-input/) and [Gamepads]($pedia/gamepads/) for more information on handling user input.

# event-key-press-release -- Keyboard

Triggers when any [Control]($pedia/controls/) is pressed or released.

# event-key-any-press-release -- Any Key

Triggers when any key is pressed/released (even those not mapped to controls). This is useful for creating user input fields.

The embedded `key code` block tells you the hardware code for the key. This is useful for special keys (such as backspace, enter, etc.) that can't be recognized as a letter or number.

![example]($pedia/controls/keycode-example.png)

The embedded `character` block tells you what letter, number or character was pressed, if one was pressed.

# event-focus-changed -- Focus

Triggers when the game gains/loses focus. Useful for mobile apps for telling when your game has been sent to the background and later resumed.

# event-mouse-press-release -- Clicked / Moved

Triggers whenever the mouse pressed/released/moved/dragged. For mobile-devices, triggers whenever a finger touches, releases or is dragged around the screen.

# event-mouse-enter-exit-actor -- Clicked / Moved on Actor

Triggers whenever the mouse enters/exits/presses/releases/drags on an actor. For mobile-devices, triggers whenever a finger touches, releases or drags an actor.

# event-mouse-enter-exit-region -- Clicked / Moved on Region

Triggers whenever the mouse enters/exits/presses/releases/drags on a region. For mobile-devices, triggers whenever a finger touches, releases or drags a region.

# event-device-swipe -- Swipe

Triggers whenever the device is swiped in the specified direction.

# event-device-multitouch -- Multi-Touch

Detects multi-touch events. Use the mouse events for regular, single-touch detection. The embedded block tells you the position of the touch and the ID of the touch (so you can track a touch throughout its lifecycle).

Useful for on-screen virtual buttons (use the **On Screen Button** that we [ship]($pedia/pre-shipped-behaviors/) with Stencyl) or air hockey like games that require detection of independent finger motions.

# event-gamepad-any-press-release -- Any Button (Gamepad)

Triggers when any gamepad button pressed/released.

Read our [Gamepad article]($pedia/gamepads/) for further details -- you are not meant to use this to implement gamepad controls, only to detect what controls to map to or to build a control configuration component.