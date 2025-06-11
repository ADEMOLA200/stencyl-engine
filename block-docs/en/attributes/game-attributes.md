# palette.attributes.game

> The following blocks are useful if you want to build a behavior that can get/set game attributes by name, using a text attribute or other means. They can also be useful as a general way of storing data (pass in a name that isn't used), without specifying it in the toolset. For regular usage, we recommend sticking to the blocks that Stencyl auto-generates for your [Game Attributes]($pedia/game-attributes/).

# palette.attributes.game.dynamic -- Game Attribute Getter / Setter

# get-game-att -- Get Game Attribute

Gets the value of the specified game attribute (using its name).

# set-game-att -- Set Game Attribute

Sets the value of the specified game attribute (using its name). You are responsible for making sure that you don't set the value to a different type. For example, if the game attribute is a number, don't stick text into that slot.

# set-game-att-save -- Saving Attributes

Change whether a game attribute will be saved (enabled by default).

# restore-game-attributes -- Restore Game Attributes

Restores all game attributes defined in Stencyl to their original value.