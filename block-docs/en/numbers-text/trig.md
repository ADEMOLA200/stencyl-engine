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
$blockCode([trig-master d:sin 0 d:degrees])

//Incoming number is Radians
$blockCode([trig-master d:sin 0 d:radians])

//Other operations
$blockCode([trig-master d:cos 0 d:radians])
$blockCode([trig-master d:tan 0 d:radians])
$blockCode([trig-master d:asin 0 d:radians])
$blockCode([trig-master d:acos 0 d:radians])
$blockCode([trig-master d:atan 0 d:radians])
```

# atan2 -- Inverse Tangent

Converts from rectangular to polar coordinates. The return value is in radians.

{ notes }

#### Example: Point Actor Towards Mouse

```design-mode { alt="atan2 example" img="atan2-example.png" }
[step]
  [comment-short "Initial angle depends on the direction the actor sprite is facing."]
  [initlocal vd:{type:number,name:initialAngle,label:"initial angle"} 90]
  [initlocal vd:{type:number,name:x,label:x} [minus [mousexy d:hoverloc d:x] [get-xy c:this d:x.center]]]
  [initlocal vd:{type:number,name:y,label:y} [minus [mousexy d:hoverloc d:y] [get-xy c:this d:y.center]]]
  [initlocal vd:{type:number,name:angle,label:angle} [to-degreesradians d:degrees [atan2 [getlocal-y] [getlocal-x]]]]
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