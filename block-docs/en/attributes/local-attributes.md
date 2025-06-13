# initlocal -- Initialize a local attribute

Initialize a new local attribute. Local attributes are not stored anywhere and can't be accessed remotely by other behaviors. They're useful for temporary calculations that are only needed within a single event.

{ code }

```
// [init [number] my number to [10]]
$blockCode([initlocal vd:{type:number,name:myNumber,label:"my number"} 10])

// [init [boolean] my boolean to <true>]
$blockCode([initlocal vd:{type:boolean,name:myBoolean,label:"my boolean"} [true]])

// [init [text] my text to [Find the fun!]]
$blockCode([initlocal vd:{type:text,name:myText,label:"my text"} "Find the fun!"])

// [init [list] my list to [create new list]]
$blockCode([initlocal vd:{type:list,name:myList,label:"my list"} [create-list]])
```

{ notes }

A local attribute can only be used within the scope where it's defined: all of the blocks underneath it at the same level.

#### Example:

```design-mode { alt="local attributes example" img="local-attr-example.png" }
[comment-short "local 1 is not yet defined here."]
[if [more [random] .5]]
  [initlocal vd:{type:number,name:local1,label:"local 1"} 5]
  [while [moreeq [getlocal-local1] 0]]
    [setlocal-local1 [minus [getlocal-local1] 1]]
    [print [str-combine [str-combine "counting down..." [getlocal-local1]] !]]
[comment-short "local 1 is no longer defined here."]
```