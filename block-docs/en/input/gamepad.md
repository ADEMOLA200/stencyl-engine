# palette.user-input.gamepad

> Read our guide on [Gamepads]($pedia/gamepads/) before consulting this reference.

# map-gamepad-control -- Map Button to Control

Binds a physical button on the gamepad to a Stencyl [control]($pedia/controls/). Each model of controller has different names for its buttons, so you must either let the user configure their controls or [discover]($pedia/gamepads/) those names.

{ notes }

#### Example (for XBox 360 Controller)

```design-mode { alt="gamepad mapping example" img="gamepad-mapping-example.png"}
[map-gamepad-control "0, left hat" "left"]
[map-gamepad-control "0, right hat" "right"]
[map-gamepad-control "0, up hat" "up"]
[map-gamepad-control "0, down hat" "down"]
```

Read [our guide]($pedia/gamepads/) on Gamepads for an explanation.

# unmap-gamepad-button -- Unmap Button

Unbinds a gamepad button from its current control.

# unmap-gamepad-control -- Unmap Control

Unbinds all gamepad buttons for a given control.

# set-gamepad-sensitivity -- Set Analog Sensitivity

Sets the **deadzone** for an analog button (usually a joystick), so that a small tilt doesn't get interpreted as actions. Defaults to 0. Provide a value between [0-100], inclusive, where 0 means that any amount of tilt/press will be detected and 100 effectively disables the button. 

# get-button-pressure -- Get Pressure for Control

Gets the pressure for a given control as a value between 0 and 1, inclusive, where 0 means no tilt/press and 1 means full tilt/press. Assumes that said control is an analog control (such as joystick), not a digital control like a regular button.

# save-gamepad-config,load-gamepad-config -- Save / Load Gamepad Configuration

Players using a less common controller will need to manually configure their controller during the game. This block lets you save and load those mappings, so they don't have to repeat the process each time they play your game. The name provided is a virtual filename. For most cases, it doesn't matter what you put in.

{ images }

$blockImage([save-gamepad-config ""])<br/>
$blockImage([load-gamepad-config ""])