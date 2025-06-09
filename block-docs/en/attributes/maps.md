# palette.attributes.maps

> Read our article on [Maps]($pedia/maps/) for an explanation of these blocks.

# create-map -- Create New Map

Creates a new, empty map. Usually, you'll assign it to a map attribute right away.

# copy-map -- Copy of Map

Returns a shallow copy of the map.

# set-map -- Set (Assign Key to Value)

Assigns the specified key to the given value for this map.

# remove-map -- Remove Item (using Key)

Removes the entry for the specified key from the map.

# empty-map -- Remove All Items

Removes all entries from the map.

# key-value -- Get (Value for Key)

Returns the entry for the given key, or null if it doesn't exist.

# key-exists-map -- Map has Key?

Returns `true` if an entry exists for the given key.

# value-exists-map -- Map has Value?

Returns `true` if the value exists in the map.

# count-map -- Number of Items in Map

Returns the number of entries in the map.

# map-is-empty -- Map is Empty?

Returns `true` if the map contains no entries.

# map-as-list -- Keys / Values of Map (as list)

Returns the `list` of [keys or values] for this map. No specific order is guaranteed. (In other words, do not count on it being the same order in which you added the entries.)

# for-each-map -- For Each Item in Map ...

Lets you perform logic on each item in the map. Use the embedded `item` block to retrieve the current item being examined.

{ code }

```
//loop over keys
$blockCode([for-each-map 0])

//loop over values
$blockCode([for-each-map 1])
```