# tostring -- Convert to Text

Converts the given value to text.

# str-emptystring -- Empty Text

Returns an empty text ("").

# str-space -- Space

Returns a space (" ").

# str-length -- Text Length

Returns the number of characters in the given text.

# str-combine -- Combine Text

Combines the two given pieces of text into one and returns that result.

# str-trim -- Trim Text

Removes spaces from the beginning and the end of the given text and returns that result. (When given an attribute, the value of the attribute remains unchanged.)

# eq -- Equals (Text)

Returns `true` if both pieces of text are exactly the same.

# str-empty -- Is Text Empty?

Returns `true` if the length of the given text is 0.

# str-beforeafter -- Does Text come before/after?

Returns `true` if the first given text alphabetically comes before (or after) the second given text.

{ code }

```
//A comes BEFORE B
$blockCode([str-beforeafter "", "", 0])

//A comes AFTER B
$blockCode([str-beforeafter "", "", 1])
```

# str-char-at -- Find Character

Returns the character at the given position. Note that the first index in a text is 0, not 1. Throws a runtime error if the given position is out of bounds.

# str-indexof -- Get Text Position

Returns the index at which the given phrase (or character) appears in the given text. Returns -1 if the phrase is not found.

> **Example:** The word "dog" corresponds to these indices: d = 0, o = 1 and g = 2. If you selected the letters "og" from the word "dog" (enter "og" in the field on the left and "dog" in the field on the right), the result would be 1.

# str-replace -- Replace Text in Text

Replaces one phrase with another within the given text.

> **Example:**
> ``` { .design-mode img="str-replace-example.png" }
> [str-replace "ham" "cheese" "hamburger"]
> ```
> Returns `cheeseburger`

# str-substring -- Substring (Part of Text)

Returns part of the given text, given the starting and ending indices. More specifically, this block returns the characters beginning with the **start index** and ending with **one less than** the **ending index**.

> **Example:** The word "cats" corresponds to these indices: c = 0, a = 1, t = 2, s = 3. If you enter "cats" in the field on the left, and 1, 3 as your starting and ending index numbers, the block would return the letters "at", i.e. the letters that correspond to the index numbers 1 and 2 in the word "cats."

# str-toupperlower -- Get Text in Upper/Lower Case

Returns the given text in all uppercase (or lowercase).

# str-split-space -- Split into Words

Splits the given text up into a [list]($pedia/lists/), using **space** as the separator (delimiter).

# str-split -- Split using Separator

Splits the given text up into a [list]($pedia/lists/), using the given separator (delimiter) text.

# get-font-width2-new -- Get Width of Text using Font

Returns the width of the given text using the given font. Useful for calculating positions for drawing text.

# get-font-height2-new -- Get Height of Font

Returns the height of the given font. Useful for calculating positions for drawing text.