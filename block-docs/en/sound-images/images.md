# palette.images.images

> Read our [Image API]($pedia/image-api) guide for an explanation of these blocks.

# image-autoscale -- Toggle Image API Auto-scaling

Set whether Image API output is scaled automatically. This is set to `true` by default. This setting affects how all the blocks below work.

When this is enabled, the coordinates and dimensions passed to all Image API blocks will be scaled by `Engine.SCALE`. By settings this to false, you can use the Image API blocks to manipulate images on a per-pixel basis, no matter how your game is upscaled.

# image-create -- Create Blank Image

Create a blank image of the specified width and height. Usually assigned to an Image attribute right away.

# image-copy -- Copy of Image

Returns a copy of the specified image. This is a true copy, so altering the copy will not affect the original.

# image-subimage -- Part of Image

Returns the specified part of the image as a new image.

# image-resize -- Resized Copy of Image

Returns a larger (or smaller) copy of the image. Width and height are given as percentages - 100% means keep it the same, 200% means double, 50% means half.

{ code }

```
//Smoothing
$blockCode([image-resize "" 0 0 d:smoothing])

//No Smoothing
$blockCode([image-resize "" 0 0 d:nosmoothing])
```

# image-screen -- Current Screen as Image

Captures the current screen as an image and returns that. This takes time (it may pause the game for a a tenth of a second), so use it sparingly.

# image-actor -- Image from Actor

Returns the current image for the specified actor. (In other words, the exact visual state of the actor at the time that you use this.)

# image-file -- Image from File

Returns an image that is loaded from a file. Images must be placed into the **extras** subfolder of your game.
Some blocks require the images to be saved with transparency enabled to work properly.

# image-url -- Load Image from URL

Returns an image that is loaded from a URL. When the image successfully loads, the enclosed blocks will run. Use the embedded `the image` block to refer to the loaded image. If the image does not load, the enclosed blocks will not run.

> For a Flash game you may need to give [permissions]($pedia/web-flash-security/) to access the web. 

# image-to-text -- Image to Text

Converts an image into text form and returns that. Useful for storing image data on servers (via an HTTP request). This takes time to run (a split second or longer).

# image-from-text -- Text to Image

Returns an image that was converted to text using the prior block. This takes time to run (a split second or longer).