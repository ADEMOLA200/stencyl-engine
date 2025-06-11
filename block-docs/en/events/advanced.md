# event-custom -- Custom Event

A [Custom Event]($pedia/custom-events/) is an event that can be called from this behavior (using the `trigger event` block), or as a response to messages that get sent by other behaviors (using one of the `trigger event ... in ...` blocks). The former is like a function call. The latter is different from function calls since sending out a message doesn't specify a recipient, so multiple recipients could exist.

![example]($pedia/custom-events/image02.png)

# event-custom-block -- Custom Block

Lets you create a regular [Custom Block]($pedia/creating-custom-blocks/).

# event-custom-block-global -- Global Custom Block

Lets you create a global (static) [Custom Block]($pedia/creating-custom-blocks/).

# events.advanced.custom-code -- Custom Code

# event-custom-code -- Arbitrary Code

Not an event. Lets you insert arbitrary code into your behavior at the "class" level. You could use this to define functions or add class-level fields, for example. Use code blocks within this wrapper.

# event-custom-import -- Import Statements

Not an event. Lets you add **import statements** to the beginning of your behavior's "class". Use code blocks within this wrapper.