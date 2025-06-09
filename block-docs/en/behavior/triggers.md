# palette.behaviors.triggers

> Read our article on [Custom Events]($pedia/custom-events/) for an explanation of these blocks.

# say -- Trigger Event in Specific Behavior (for Actor)

Triggers the custom event for a specific behavior that is attached to the specified actor.

# shout -- Trigger Event in All Behaviors (for Actor)

Triggers the custom event for all behaviors that are attached to the specified actor.

# scene-say -- Trigger Event in Specific Behavior (for Scene)

Triggers the custom event for the specified behavior that is attached to the current scene.

# scene-shout -- Trigger Event in All Behaviors (for Scene)

Triggers the custom event for all behaviors that are attached to the current scene.

# say-this -- Trigger Event (this Behavior)

Triggers a custom event in this behavior. This is a direct function call, so an event with the specified name must exist, otherwise it will cause a compilation error.