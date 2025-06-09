# is-snippet-enableda -- Is Behavior enabled? (for Actor)

Returns `true` if the specified behavior (using its name) is enabled for the given actor.

# is-snippet-enabled -- Is Behavior enabled? (for Scene)

Returns `true` if the specified behavior (using its name) is enabled for the current scene.

# actor-enabledisable-snippet -- Enable / Disable Behavior for Actor

Enables (or disabled) the specified behavior (using its name) for the given Actor. Disabling a behavior will stop it from receiving **when updating** and **when drawing** events but does not prevent its other events and do-after/do-every tasks from running.

# scene-enabledisable-snippet -- Enable / Disable Behavior for Scene

Enables (or disabled) the specified behavior (using its name) for the current scene. Disabling a behavior will stop it from receiving **when updating** and **when drawing** events but does not prevent its other events and do-after/do-every tasks from running.

# disable-snippet -- Disable This Behavior

Disables the current behavior. Does **not** immediately stop its code from running - you'll need to use $blockImage([stop]) to achieve that.

Disabling a behavior will stop it from receiving **when updating** and **when drawing** events but does not prevent its other events and do-after/do-every tasks from running.

# has-snippet -- Does Actor have behavior?

Returns `true` if the specified behavior (given the behavior name) is attached to the given actor.

# scene-has-snippet -- Does Scene have behavior?

Returns `true` if the specified behavior (given the behavior name) is attached to the current scene.