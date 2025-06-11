# Block Documentation

A block's documentation is signified by this:

```
# blocktag -- Label
```

Documentation may consist of various sections, some of which are automatically generated (block images, generated code),
and some of which are supplied from the documentation sources (basic info, extra notes/examples/warnings).

The first paragraph after the block is declared is the { info } section. Any other section which you want to use must be
explicitly specified. If the auto-generated section is included, it will be overridden.

````
# blocktag -- Label

Description of block functionality.

{ images }

$blockImage([blocktag])

{ code }

```
$blockCode([blocktag])
```

{ notes }

#### Example

```design-mode { alt="alt text" img="blocktag-example.png" }
[if [true]]
  [blocktag]
```
````

This will generate into something like this:

````
### <a name="blocktag"></a> Label

$blockImage([blocktag])

Description of block functionality

```
$blockCode([blocktag])
```

#### Example

```design-mode { alt="alt text" img="blocktag-example.png" }
[if [true]]
  [blocktag]
```
````

After the sections have been layed out, special symbols will be processed:
- `$pedia` -> replaced with the root url of stencylpedia
- `$blockImage(__)` -> replaced with an image of a single block, suitable for use inline with text or in tables
- `$blockCode(__)` -> replaced with the generated code of a single block, suitable for use within code fences
- `design-mode { img="___"} ` -> specifies a code fence as containing design mode code, which will be replaced by an image of the equivalent design mode blocks. The image will contain the source within the code fence as metadata, so it can be copied into Stencyl.


# Combined Blocks

Multiple blocks can be documented in a single place.

```
# blocktag1,blocktag2,blocktag3,... -- Label
```

In this case, the auto-generated { images } and { code } sections will contain images/code for all of the specified blocks.


# Section Documentation

A section of the block palette can be documented

```
# palette.section.id

Extra info for this palette section
```

Example:

```
# palette.actors.tweening

> Read our article on [Tweening]($pedia/tweening/) for an explanation of these blocks.
```

The id can be taken from a category, a section, or a header.

Similarly, a section of the events palette can be documented

```
# events.section.id

Extra info for this events section
```

Example:

```
# events.collisions

> Read our [Collisions article]($pedia/collisions-and-groups/) for an explanation of these events.
```

# Source Structure

```
engine-extension-root/
  block-docs/
    {lang}/
      **/*.md
```

Files are found within a language-specific folder. All files in the folder will be scanned recursively. File names don't matter. Tooling may be used to keep files organized in some manner, such as placing each block's information in a file that corresponds to it's palette location.

What file a block's info is found in, as well as order of blocks within a file doesn't matter.

# Generated Structure

Documentation will be organized into files based on the palette structure

```
outputRoot/
  category/
    section.md
    section.md
```