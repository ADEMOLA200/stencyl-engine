# event-mobile-keyboard -- Keyboard

Triggers when the mobile (soft) keyboard is shown, hidden, typed into, or submitted.

View our article on [Mobile Keyboards]($pedia/mobile-features/) for further details.

# show-hide-keyboard -- Show / Hide Keyboard

Immediately shows or hides the [virtual keyboard]($pedia/mobile-features/). Use mobile keyboard events to track what's been typed.

```design-mode { img="keyboard-text-example.png" }
[event-mobile-keyboard d:typed]
  [set-game-att highScoreName [mobile-keyboard-text]]
```

# set-keyboard-text -- Set Keyboard Text

Imagine that the keyboard is inputting into an invisible text field. This sets the text that's in that text field.

# clear-keyboard-text -- Clear Keyboard Text

Imagine that the keyboard is inputting into an invisible text field. This clears out the text that's in that text field.

# vibrate -- Vibrate

[Vibrates]($pedia/mobile-features/) the device for the given number of seconds. On some devices, vibration duration cannot be controlled.

# show-alert -- Show Alert

Displays a native modal (blocking) dialog to the user. Provide the title and message.

# ios-badge-number -- Set Icon Badge (iOS)

iOS-only. Sets your app icon's badge number. For example, on an e-mail app, this would report the number of unread messages. For a game, perhaps the number of notifications / events that have happened in your game. 