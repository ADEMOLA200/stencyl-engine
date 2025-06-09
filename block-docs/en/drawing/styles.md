# rgb-to-color -- Create Color (from RGB)

Creates a **Color** value from red, green, blue channels. Numbers must be between [0-255] inclusive.

# set-color -- Set Color

Sets the color used for filling shapes (does not apply to fonts). You can select the color using the color picker, drag in a color attribute or drag in any block that returns a color.

# set-font-new -- Set Font

Sets the font used in drawing text. You can pick the font directly or drag in a font attribute block.

# letter-spacing -- Set Spacing

Sets the spacing between characters of the font.

# set-alpha -- Set Opacity

Sets the opacity (alpha) used in drawing to the specified percentage. Number must be between [0-100] inclusive.

# set-stroke-color -- Set Stroke Color

Sets the stroke color used when drawing shapes (does not apply to fonts). You can select the color using the color picker, drag in a color attribute or drag in any block that returns a color.

# set-thickness -- Set Stroke Thickness

Sets the stroke thickness (width) used when drawing shapes. Set to 0 to disable.

# get-font-width -- Get Width of Text for Current Font

Returns the width of the specified text using the current font. Useful for calculating text drawing positions. May only be used in a `when drawing` event.

# get-font-width2-new -- Get Width of Text for Specific Font

Returns the width of the specified text using the given font. Useful for calculating text drawing positions.

# get-font-height -- Get Height for Current Font

Returns the height of text using the current font. Useful for calculating text drawing positions. May only be used in a `when drawing` event.

# get-font-height2-new -- Get Height for Specific Font

Returns the height of text using the given font. Useful for calculating text drawing positions.