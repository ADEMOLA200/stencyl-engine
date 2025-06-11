# palette.game.saving

> View our article on [Saving Games]($pedia/saving-and-loading-games/) for an explanation of these blocks.

# save-game -- Save Game

Tells the game to save. Saving will store the state of all game attributes into a file.

If the save operation succeeds, the embedded `save succeeded` block will return `true` and the enclosed blocks will run. If the save fails, the embedded `save succeeded` block will return `false`, and the enclosed blocks will still run.

{ notes }

#### Example

```design-mode { alt="save succeeded example" img="save-succeeded-example.png" }
[save-game]
  [if [save-success]]
    [print "Saved game!"]
  [else]
    [print "Could not save the game"]
```

# load-game -- Load Game

Tells the game to load. Loading will overwrite the values of all game attributes with those in the save file (if it exists).

If the load operation succeeds, the embedded `save succeeded` block will return `true` and the enclosed blocks will run. If the save fails, the embedded `save succeeded` block will return `false`, and the enclosed blocks will still run.