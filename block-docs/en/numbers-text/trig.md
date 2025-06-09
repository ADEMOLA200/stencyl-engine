# to-degreesradians -- Degrees <--> Radians

Converts the given number to degrees or radians.

# pi -- Pi

Returns the value of Pi (3.14159...).

# e -- e

Returns e, the base of natural logarithms. (2.718...)

# trig-master -- Sin / Cos / Tan

Returns the result of applying a trigonometric function to the given number. Dropdown for degrees/radians specifies what format the **incoming** number is in. Supports sin/cos/tan/asin/acos/atan.

{ code }

```
//Incoming number is Degrees
$blockCode([trig-master 0 0 0])

//Incoming number is Radians
$blockCode([trig-master 0 0 1])

//Other operations
$blockCode([trig-master 1 0 1])
$blockCode([trig-master 2 0 1])
$blockCode([trig-master 3 0 1])
$blockCode([trig-master 4 0 1])
$blockCode([trig-master 5 0 1])
```

# atan2 -- Inverse Tangent

Converts from rectangular to polar coordinates. The return value is in radians.

{ notes }

#### Example: Point Actor Towards Mouse

``` { .design-mode img="atan2-example.png" }
[step]
  [comment-short "Initial angle depends on the direction the actor sprite is facing."]
  [initlocal vd:{type:"number",name:"initialAngle",label:"initial angle"} 90]
  [initlocal vd:{type:"number",name:"x",label:"x"} [minus [mousexy 0 0] [get-xy c:this 2]]]
  [initlocal vd:{type:"number",name:"y",label:"y"} [minus [mousexy 0 1] [get-xy c:this 3]]]
  [initlocal vd:{type:"number",name:"angle",label:"angle"} [to-degreesradians 0 [atan2 [getlocal-y] [getlocal-x]]]]
  [setangle c:this [plus [getlocal-angle] [getlocal-initialAngle]]]
```

Using inverse tangent, we can calculate the angle to rotate the actor to based on the mouse's position.

# sqrt -- Square Root

Returns the square root of the given number.

# pow -- Power

Returns the given number to the specified power (e.g., x<sup>y</sup>).

# lnexp -- Natural Logarithm / e Raised to a Power

**ln** - Returns the natural logarithm of the given number.<br/>
**e^** - Returns the number e to the given power.