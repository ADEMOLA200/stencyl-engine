# if -- If

Checks whether the condition is `true` or `false`. If the condition is `true`, the blocks wrapped inside will execute.

# else -- Otherwise

Use directly below an "If" block. If the condition in the preceding "If" block is `false`, the blocks wrapped inside the "Otherwise" block will execute.

# else-if -- Otherwise If

Use directly below an "If" block. If the condition in the preceding "If" block is `false`, and the condition of this wrapper is `true`, the blocks wrapped inside the "Otherwise If" block will execute. Equivalent to doing the following:

``` { .design-mode img="otherwise-if-equivalent.png" }
[else]
  [if ""]
```

# palette.flow.conditions.booleans

Booleans (denoted by a hexagon shape) are conditions that resolve to `true` or `false`.

# and -- And

Returns `true` if both of the provided conditions are `true`. If the first condition is `false`, the second condition will not be evaluated.

# or -- Or

Returns `true` if at least one of the provided conditions is `true`. If the first condition is `true`, the second condition will not be evaluated.

# not -- Not

Returns `true` if the condition resolves to `false`. Testing `if not [CONDITION]` is equivalent to `if [CONDITION] = false`.

# true,false -- True / False

Literal values of `true` and `false`.

# eq -- Equals

Returns `true` if both values are equal.

# noteq -- Not Equal

Returns `true` if the values are not equal.

# less,lesseq,more,moreeq -- Comparators

Returns `true` if...

Operator | Description
--- | ---
$blockImage([less 0 0])|First number is smaller than second number.
$blockImage([lesseq 0 0])|First number is smaller than or equal to than second number.
$blockImage([more 0 0])|First number is larger than second number.
$blockImage([moreeq 0 0])|First number is larger than or equal to second number.

# as-boolean -- Boolean Conversion

Converts the given value (typically text) into a Boolean. May throw a compile-time or runtime error if conversion is not possible.

# stop -- Stop

Skips the rest of the code in this event for the current step/frame.