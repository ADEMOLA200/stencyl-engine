# repeat -- Repeat

Repeats the wrapped blocks a given number of times. The embedded `current loop count` block returns how many times you've looped so far (starting from 0, ending at [NUMBER] - 1).

{ notes }

#### Example

``` { .design-mode img="flow-loop-example1.png" }
[initlocal def:{name:"number",label:"Number",type:"number"} 5]
[repeat [getlocal-number]]
  [print [loopindex]]
```
Prints out [0 1 2 3 4].

# while -- While Loop

Runs the wrapped blocks while the given condition is `true`. If the condition is `false` to begin with, nothing will run. Make sure that the condition becomes `false` at some point during the evaluation of the loop (or use the `exit loop` block), otherwise it will result in an infinite loop that will crash your game.

# repeatu -- Repeat Until Loop

Runs the wrapped blocks while the given condition is `false`. If the condition is `true` to begin with, nothing will run. Make sure that the condition becomes `true` at some point during the evaluation of the loop (or use the `exit loop` block), otherwise it will result in an infinite loop that will crash your game.

{ notes }

#### Example

``` { .design-mode img="flow-loop-fibonacci.png" }
[initlocal def:{name:"previous",label:"Previous",type:"number"} 1]
[initlocal def:{name:"current",label:"Current",type:"number"} 1]
[repeatu [more [getlocal-current] 10]]
  [initlocal def:{name:"temp",label:"Temp",type:"number"} [getlocal-current]]
  [setlocal-current [plus [getlocal-previous] [getlocal-current]]]
  [setlocal-previous [getlocal-temp]]
  [print [getlocal-current]]
```

This will calculate Fibonacci sequence numbers until the current number is greater than 10.

Loop Count | Result | Answer
--- | --- | ---
Prev | 1 | -
Curr | 1 | -
1 | 1 + 1 | 2
2 | 1 + 2 | 3
3 | 2 + 3 | 5
4 | 3 + 5 | 8
5 | 5 + 8 | 13 <-- Greater than 10, stop looping.

# break -- Exit Loop

Stops the execution of a loop's code.

# continue -- Return to Start of Loop

Skips the rest of the code for an iteration of the loop and proceeds to the next iteration (if another iteration will be done).

{ notes }

#### Example

``` { .design-mode img="flow-loop-example2.png" }
[initlocal def:{name:"number",label:"Number",type:"number"} 0]
[repeat [less [getlocal-number] 10]]
  [setlocal-number [plus [getlocal-number] 1]]
  [if [eq [remainder [getlocal-number] 2] 0]]
    [continue]
  [print [getlocal-number]]
```

The loop prints out odd numbers between [0-9], so this will print out [1 3 5 7 9].
