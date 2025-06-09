# plus,minus,times,div -- Add / Subtract / Multiply / Divide

Adds/Subtracts/Multiplies/Divides the two provided numbers. Note that only Chuck Norris can divide by 0.

{ images }

$blockImage([plus 0 0]) $blockImage([minus 0 0])<br/>
$blockImage([times 0 0]) $blockImage([div 0 0])

# neg -- Negate

Flips the sign of the given number.

# mod -- Remainder (Modulo)

Returns the integer remainder after dividing the first number by the second.

# randint -- Random Integer

Returns a random integer between the first and second numbers, inclusive. Provide integers for both numbers.

# randomfloat -- Random Float Between Numbers

Returns random floating point number between the first number (inclusive) and the second number (exclusive).

# random -- Random Float Between Zero and One

Returns a random floating point number between 0 and 1, inclusive.

# incdec -- Increment / Decrement Number

Adds (or subtracts) the given number to/from a **number attribute**.

# abs -- Absolute Value

Returns the absolute value of the given number. (If it is negative, makes it positive.)

# minmax -- Smaller / Larger of Two Numbers

Returns the smaller (or larger) of the two numbers.

# roundnew -- Round / Floor / Ceiling

Returns the nunber as an integer, with rounding applied as follows:

**Round** - Rounds up if the fractional part is 0.5 or more. Otherwise, rounds down.

**Floor** - Always rounds down.

**Ceiling** - Always rounds up.

# as-number -- Number Conversion

Converts the given value (can be any type) to a number. In practice, this is mainly useful for text and booleans (where true = 1, false = 0).