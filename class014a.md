# CSS Transforms

*Transforms are a new way to change the position and alter images.*

*It can be two dimensional or three dimensional.*

*CSS transforms do not have the best support from the browsers that’s why they are normally used with prefixes.*

*The usage of these transforms is by writing the property and then the value which contains the type and then the amount between parenthesis.*

*The two dimensional transforms work on the x and y axis.*

*The three dimensional transforms work on the x, y and z axis which will play with the width, height, and depth of the element.*

## 2D Rotate: 

*the transform property accepts different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.*
## 2D Scale: 

*using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.*

## 2D Translate:

*using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.*

## 2D Skew: 

*the last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both.*

*It is common for multiple transforms to be used at once.*

## 3D Rotate: 

*with three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.*

## 3D Scale: 

*by using the scaleZ three-dimensional transform elements may be scaled on the z axis. This is a source of trouble when no other three-dimensional transforms are in place, as there is nothing in particular to scale.*

## 3D Translate: 

*a negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.*

*Elements cannot be skewed on the z axis.*

## CSS Transitions

*With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
Transitional Property: the transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties.*

### Transitional Properties: 

*it is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another.*

### Transition Duration: 

*the duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms).*

### Transition Timing: 

*the transition-timing-function property is used to set the speed in which a transition will move.
Transition Delay: determines how long a transition should be stalled before executing.
Animations*

*Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.*

### Animation Duration, Timing Function, & Delay: 

*once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds. There are some transition ideas that might make your website fun to use:*

1. fade in

2. change color

3. Grow and shrink

4. rotate elements

5. squares to circles

6. 3D shadow

7. swing

8. Insert border