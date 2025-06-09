# palette.attributes.lists

> Read our article on [Lists]($pedia/lists/) for an explanation of these blocks.

# create-list -- Create New List

Creates and returns an empty list. Usually, you'll want to set this immediately to a list attribute.

# copy-list -- Copy of List

Returns a shallow copy of the specified list.

# add-list -- Add Item to List

Adds the given value to the end of the list.

# insert-list -- Insert Item into List

Inserts the given value at the specified index of the list. This will push everything at that index and after down one position. The index must be between 0 and (size of list - 1) inclusive.

# remove-item -- Remove Item from List

Removes the given value from the list, if it exists. If it does not exist, nothing happens.

# remove-index -- Remove Item from Index

Removes the value at the specified index from the list. The index must be between 0 and (size of list - 1) inclusive.

# replace-list -- Replace Item in List

Replaces the item at the specified index with another for the list. The index must be between 0 and (size of list - 1) inclusive.

# clear-list -- Empty out List

Removes all values from the list.

# get-item -- Get Item from Index

Returns the item at the specified index in the list. The index must be between 0 and (size of list - 1) inclusive.

# position-of-item -- Position of Item in List

Returns the index of the item in the list. If the item is in the list multiple times, this returns the first index found. If the item isn't in the list, this returns -1.

# contains-item -- List contains Item?

Returns `true` if the list contains the specified item.

# length-list -- List Size

Returns the number of items in the list.

# is-empty -- Is List Empty?

Returns `true` if the list contains no items.

# for-each -- For Each Item in List ...

Lets you perform logic on each item in the list. Use the embedded `item` block to retrieve the current item being examined.