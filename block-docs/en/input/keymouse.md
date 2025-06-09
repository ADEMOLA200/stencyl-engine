# palette.user-input.keyboard-mouse

> Read our article on [Controls]($pedia/controls/) for more information on handling user input.

# keystate -- Key Status

Returns `true` if the given [control]($pedia/controls/) [is down, was pressed, was released].

State | Description
--- | ---
is down | Key is currently pressed down.
was pressed | Key was **just** pressed down. Called once per press-release cycle.
was released | Key was **just** released. Called once per press-release cycle.

# is-special-down -- Special Key is Down

Returns `true` if [shift / ctrl] is currently being held down. On a Mac, ctrl is equivalent to command.

# simulate-key -- Simulate Keys

Simulates a key [press / release] using the given control. Primarily used for implementing virtual controls as on-screen buttons in mobile games. Could also be used to make cutscenes.

# keycode -- Get Key Code

Returns the hardware code for certain keys [enter, backspace, shift, delete, ctrl / command]. Compare this number with the code returned by an **Any Key** event. Could be used to implement a text field.

{ notes }

#### Example

![keycode-example]($pedia/controls/key-input-example.png)

A simple implementation of a text-field behavior. See the "Example: Text Input" section of our [Controls guide]($pedia/controls/) for an explanation.

# palette.user-input.keyboard-mouse.mouse-touch

Mouse and Single Touch (vs. Multi-Touch) are handled using the same blocks, as described in our [Touch article]($pedia/mobile-input/).

# mousestate -- Mouse / Touch Status

Returns `true` if the mouse [is down, was pressed, was released].

State | Description
--- | ---
is down | Mouse button is currently pressed down.
was pressed | Mouse button was **just** pressed down. Called once per click-release cycle.
was released | Mouse button was **just** released. Called once per click-release cycle.

# amousestate -- Mouse on Actor / Touched Actor

Returns `true` if the mouse [is down on, was pressed on, was released on] the given actor.

State | Description
--- | ---
is down | Mouse button is currently pressed down.
was pressed | Mouse button was **just** pressed down. Called once per click-release cycle.
was released | Mouse button was **just** released. Called once per click-release cycle.

# mousexy -- Mouse / Touch Position

Returns the last known (x, y) position of the [mouse (cursor), mouse press, mouse release]. Before using mouse press/release, first check if the mouse has been pressed or released.

> On mobile, only mouse press/release are available since there's no concept of a mouse hovering over the screen.

# mousedisp -- Mouse Cursor

Shows or hides the mouse cursor. Doesn't apply to mobile games. Useful for implementing custom cursors (using an actor that follows the mouse).