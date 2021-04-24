# Class 14-a Summary

## Transforms

* Transforme property contains techniques to size, position and change elements .
* Transform property has two different settings : 2-dimensional & 3-dimensional. 

#### Transform Syntax:

* Transform syntax including transform property followed by the value.the value specifies transform type followed by the amount inside parentheses.

#### 2D Transforms:

* 2-dimensional transforms work on the x and y axes (horizontal and vertical axes)

#### 3D Transforms:

* 3-dimensional transforms work on x, y and z axis.(length, width and depth).

#### Combining Transforms:

* we can use multiple transforms at once, rotating and scaling the size of an element at the same time.
* To combine transforms, list the transform values within transform property one after the other without commas.

![transform](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

## Transition and Animations:

### Transitions:

* the ways for determining styles for different states using: (:hover,:focus,:active and :target) pseudo-classes.
* Transition Properties:
1. transition-property (not all properties may be transitioned, only properties that have an identifiable halfway point).
2. transition-duration (The duration in which a transition takes place).
3. transition-timing-function (used to set the speed in which a transition will move).
4. transition-delay (The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing).

* example:

![transition](https://www.imore.com/sites/imore.com/files/styles/xlarge/public/field/image/2014/10/PastedGraphic-14.jpeg?itok=PgEcEP70)

### Animation:

* when more control is rquired, use animations.
* Animations Keyframes:
use Animation keyFrames to set multiple points at which an element should undergo a transition. KeyFrames includes the animation name, any animation breakpoints, and the properties intended to be animated.

1. Animation Name (the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value).
2. Animation Duration, Timing Function, & Delay
3. Animation Iteration(an animation repeat itself numerous times the animation-iteration-count property may be used).
4. Animation Direction (declare the direction an animation).

* all information taken from the site.

**Sukina AbuHammad**