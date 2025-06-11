# custom-code,code-long -- Code Block (Single Line, Multi Line)

Lets you embed code into your Behavior. Can be used in many ways. Particularly useful for calling functions that Stencyl or Haxe provide but don't exist in block form. Take a look at our [API](https://static.stencyl.com/api/33/) to see what's available.

{ code }

# code-short -- Code Block (Inline)

Lets you embed a fragment of code into a block field.

{ code }

# game-url -- Game URL

Returns the URL of the website where this game is running (on Flash, HTML5). Returns an empty text on other platforms.

# language -- language

The language code of the system (device) on which the game is running.

# stepsize -- Step Size

Returns the number of milliseconds in each "step" of the game. This corresponds to the time elapsed between updates to `when updating` events. The default step size is 10 milliseconds.

# null -- null

Returns "null", which stands for the absence of a value.

# is-platform -- Running on Platform

Returns `true` if the game is running on the selected platform.

**Choices:**
* Flash
* HTML5
* Desktop
* iOS
* Android
* Web
* Mobile
* Windows
* Mac
* Linux

# is-device2 -- Running on Specific iOS Device

Returns `true` if the game is running on the selected kind of iOS device. Useful if you want to fine-tune a game's display or behavior on specific devices.

**Choices:**
* 3.5" iPhone
* 4.0" iPhone
* 4.7" iPhone
* 5.5" iPhone
* iPad

# do-on-platform -- Do only on Platform

Include the wrapped blocks only on the specified platform. On other platforms, the wrapped blocks will not exist at all.

**Choices:**
* Flash
* HTML5
* Desktop
* iOS
* Android
* Web
* Mobile
* Windows
* Mac
* Linux

# exit-game -- Exit Game

Quits out of a Desktop game or standalone Flash game. Does nothing on Flash/HTML5 running in a browser. On iOS/Android, it may send the app to the background (and goes against platform guidelines).

# palette.flow.advanced.mem

These blocks are deprecated. We now recommend handling [atlases]($pedia/mobile-atlases/) entirely using the Atlas page.

# load-unload-atlas -- Load / Unload Atlas

Tells the game to load (or unload) an atlas in the **next** scene. Specify the **Atlas ID**.

# atlas-loaded -- Is Atlas Loaded?

Returns `true` if the specified atlas (using Atlas ID) is currently loaded.