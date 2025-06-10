# initlocal -- Initialize a local attribute

Initialize a new local attribute. Local attributes are not stored anywhere and can't be accessed remotely by other behaviors. They're useful for temporary calculations that are only needed within a single event.

{ notes }

A local attribute can only be used within the scope where it's defined: all of the blocks underneath it at the same level.

#### Example:

``` { .design-mode img="local-attr-example.png" }
[init]
  [comment-short "local 1 is not yet defined here."]
  [if [more [random] .5]]
    [initlocal vd:{type:number,name:local1,label:"local 1"} 5]
    [while [moreeq [getlocal-local1] 0]]
      [setlocal-local1 [minus [getlocal-local1] 1]]
      [print [str-combine [str-combine "counting down..." [getlocal-local1]] !]]
  [comment-short "local 1 is no longer defined here."]
```