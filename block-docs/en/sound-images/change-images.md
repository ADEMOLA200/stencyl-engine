# palette.images.change-images

> Read our [Image API]($pedia/image-api) guide for an explanation of these blocks.

# image-draw -- Draw Image onto Image

Draws the first image on top of the second image at the specified location.

# image-draw-text -- Draw Text onto Image

Draws the given text (using a font) on top of the image at the specified location.

# image-fill -- Fill Image with Color

Replaces all pixels in the image with the given color.

# rgb-to-color -- Make Color (from RGB)

Creates a color from red, green, blue channels. Numbers must be between [0-255] inclusive.

# image-clear -- Clear Part of Image

Clears out the specified part of the image by making those pixels transparent.

# image-clear-all -- Clear Whole Image

Clears out the entire image by making its pixels transparent.

# image-mask -- Clear / Retain Image using Mask

Clears out the image using the second image as a mask. The second image will "cut out" pixels from the first. If using "retain", will do the opposite -- it will clear out all pixels except for those that are in the mask.

# image-filter -- Apply Effect to Image

Applies the given [effect]($pedia/effects/) to the image.

# image-flip -- Flip Image

Flips the image horizontally or vertically.

# image-swap -- Swap Colors in Image

Replaces all pixels of the first color with the second color in the image.

# image-wrapper -- Batch Draw

When setting many pixels at a time, this tells the system not to push an image update until you have finished your work. A must-use for performance reasons.

# image-set-px -- Set Pixel

Sets a pixel in the image to the specified color.

# image-get-px -- Draw Image onto Image

Returns the color for the specified pixel in the image.