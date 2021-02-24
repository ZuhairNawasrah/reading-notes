# CSS Transforms, Transitions, and Animations

## CSS Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the `transform` property. Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. 

Regarding to 2D, the transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.

## CSS Transitions

 **Transition**: to make it, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the `:hover`, `:focus`, `:active`, and `:target` **pseudo-classes**.

 The `transition` property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

## CSS Animations

The animation shorthand CSS property applies an animation between styles. The animation property is specified as one or more single animations, separated by commas. The order within each animation definition is also important for distinguishing `animation-name` values from other keywords. When parsed, keywords that are valid for properties other than `animation-name`, and whose values were not found earlier in the shorthand, must be accepted for those properties rather than for `animation-name`.