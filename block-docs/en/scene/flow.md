# palette.scenes.game-flow

> Read our guide on [Changing Scenes]($pedia/changing-scenes/) and [Pausing]($pedia/pausing/) for an explanation of these blocks.

# scene-change-color -- Switch Scene (Fade In/Out)

Switches to a different scene using a fade in/out transition.

{ code }

```
//Using fade in and out
switchScene([SCENE].getID(), createFadeOut([NUMBER], [COLOR]), createFadeIn([NUMBER], [COLOR]));

//Other Transition types
createBlindsOut([NUMBER], [COLOR]), createBlindsIn([NUMBER], [COLOR]),
createBubblesOut([NUMBER], [COLOR]), createBubblesIn([NUMBER], [COLOR]),
createCircleOut([NUMBER], [COLOR]), createCircleIn([NUMBER], [COLOR]),
createPixelizeOut([NUMBER], [COLOR]), createPixelizeIn([NUMBER], [COLOR]),
createRectangleOut([NUMBER], [COLOR]), createRectangleIn([NUMBER], [COLOR])
```

# scene-change-through -- Switch Scene (Crossfade / Slide)

Switches to a different scene using a crossfade or slide transition.

# scene-reload-color -- Reload Current Scene (Fade In/Out)

Reloads the current scene using a fade in/out transition.

{ code }

```
//Using fade in and out
reloadCurrentScene(createFadeOut([NUMBER], [COLOR]), createFadeIn([NUMBER], [COLOR]));

//Other Transition types
createBlindsOut([NUMBER], [COLOR]), createBlindsIn([NUMBER], [COLOR]),
createBubblesOut([NUMBER], [COLOR]), createBubblesIn([NUMBER], [COLOR]),
createCircleOut([NUMBER], [COLOR]), createCircleIn([NUMBER], [COLOR]),
createPixelizeOut([NUMBER], [COLOR]), createPixelizeIn([NUMBER], [COLOR]),
createRectangleOut([NUMBER], [COLOR]), createRectangleIn([NUMBER], [COLOR])
```

# scene-reload-through -- Reload Current Scene (Crossfade / Slide)

Reloads the current scene using a crossfade or slide transition.

# scenebyname -- Get Scene (using name)

Returns a Scene by its name. Use inside a scene-switching block for an easy way to switch scenes by name.

# is-transitioning -- Scene is transitioning?

Returns `true` if the game is in the process of transitioning to another scene, transitioning from another scene, or reloading.

# create-actor3-next -- Create Actor in next scene

Notifies the game to creates an actor in the next scene (or the reload of the current one). This is useful, for example, for top-down games (like Zelda) where you'll exit the screen on one side and want to seamlessly reappear on the "correct" side.

# pause-unpause -- Pause / Unpause Game

[Pauses]($pedia/pausing/) (or unpauses) the game. You can selectively opt out actors on the Physics > Advanced page of their editor.

# is-paused -- Game is Paused?

Returns `true` if the game is paused.