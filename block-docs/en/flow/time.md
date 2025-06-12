# dolater -- Do after N seconds

Runs the code after the given delay (in seconds, can be partial seconds).

{ code }

```
runLater(1000 * [NUMBER], function(task:TimedTask):Void {
  [ACTIONS]
}, [ACTOR]); //the actor this timed task is bound to, or null
```

{ notes }

> **Warning:** Do not use this block in a `when updating` event, unless constrained by an `if` block or other conditional.

# periodic -- Do every N seconds

Runs the code every [N] seconds (can be partial seconds).

{ code }

```
runPeriodically(1000 * [NUMBER], function(task:TimedTask):Void {
  [ACTIONS]
}, [ACTOR]); //the actor this timed task is bound to, or null
```

{ notes }

> **Warning:** Do not use this block in a `when updating` event, unless constrained by an `if` block or other conditional.

#### Example

```design-mode { alt="periodic example" img="periodic-example-2.png" }
[init]
  [periodic 2]
    [toggle-image c:this d:hide]
    [periodic 1]
      [toggle-image c:this d:show]
```

`do after n seconds` and `do every n seconds` can be combined together. In this example, we implement a "blinking" effect by alternating the actor between hidden and not-hidden, without relying on a variable to store state.

# cancel -- Cancel

Cancels the execution of a periodic (`do every n seconds`) task.