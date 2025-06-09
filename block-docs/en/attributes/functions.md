# tween-number -- Tween a Number Attribute

Applies a [tween]($pedia/tweening/) to the given number attribute.

{ code }

```
$blockCode([tween-number _ _ _ _])

//Or in one line (slower, uses dynamic typing)
tweenNumber([TEXT], [NUMBER], [NUMBER], [EASING]) //internal name, value, duration (seconds), easing
```

# cancel-tween-number -- Cancel Tween

Stops an ongoing number tween.

# value -- Has Value?

Returns `true` if the given attribute has a value (is not "null").

# clear -- Clear Value of Attributes

Disassociates the given attribute from any value. (Sets its value to "null", does not have any effect on primitive types like numbers/booleans)