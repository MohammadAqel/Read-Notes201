## Transforms :

- Transform Syntax : 
  -  transform type :
    - div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

- **2D Transforms** : Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. 
 - **2D Rotate** : The rotate value provides the ability to rotate an element from 0 to 360 degrees ,
   The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.
   
   
   **Ex: 
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}**
  
  - **2D Scale** : 
   - Using the scale value within the transform property allows you to change the appeared size of an element.
     The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while
     any value greater than or equal to 1.01 makes an element appear larger.
   
   - **EX :
   .box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: scale(1.25);
}**


- The scaleX value will scale the width of an element while the scaleY value will scale the height of an element. 
- **EX: 
.box-1 {
  transform: scaleX(.5);
}
.box-2 {
  transform: scaleY(1.15);
}
.box-3 {
  transform: scale(.5, 1.15);
}**


- **2D Translate**
  -Using the translateX value will change the position of an element on the horizontal axis while using the translateY
  value will change the position of an element on the vertical axis.
  
  - **EX :
  .box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}**


- **2D Skew**
  - Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis.
  To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then 
  the y axis  value.
  
  - **EX :
   .box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}**


- **Transform Origin**
 - The transform-origin property can accept one or two values. When only one value is specified, that value is used for both 
  the horizontal and vertical axes.
  - **EX :
  .box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}
.box-2 {
  transform: scale(.5);
  transform-origin: 100% 100%;
}
.box-3 {
  transform: skewX(20deg);
  transform-origin: top left;
}
.box-4 {
  transform: scale(.75) translate(-10px, -10px);
  transform-origin: 20px 50px;
}**

- **Perspective**
 -Using the perspective value within the transform property works great for transforming one element from a single.
 - **EX:
 .box {
  transform: perspective(200px) rotateX(45deg);
}**

- **3D Rotate** 
  - Using the rotateX value allows you to rotate an element around the x axis, as if it were being bent in half horizontally.
  Using the rotateY value allows you to rotate an element around the y axis, as if it were being bent in half vertically.
  Lastly, using the rotateZ value allows an element to be rotated around the z axis.
 
- **3D Scale** 
 - using the scaleZ three-dimensional transform elements may be scaled on the z axis.
 - however the rotateX value is added in order to see the behavior of the scaleZ value.
 
- **3D Translate**
  -Elements may also be translated on the z axis using the translateZ value. 
  - A negative value here will push an element further away on the z axis, resulting in a smaller element.
  Using a positive value will pull an element closer on the z axis, resulting in a larger element.
  
- **Transform Style**
  - The _transform-style_ property needs to be placed on the parent element, above any nested transforms.
  - The _preserve-3d_ value allows the transformed children elements to appear in their own three-dimensional 
   plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane.
   
   
 - **Backface Visibility**
   -  _backface-visibility_ is visible or hidden;
   
   ____________
   
   ## Transitions & Animations
   
   - **Transitions** : :hover, :focus, :active, and :target pseudo-classes.
    - including transition-property, transition-duration, transition-timing-function, and transition-delay. 
    
  - **Transitional Property**
   - The _transition-property_ property determines exactly what properties will be altered in conjunction with
    the other transitional properties.
    
    
  - **Transitional Properties**
  
   transitional properties include the following :
   
   - background-color
   - border-width
   - clip
   - font-size
   - left
   - margin
   - min-height
   - outline-color
   - padding
   - text-shadow
   - visibility
   - z-index
   - background-position
   - border-spacing
   - color
   - font-weight
   - letter-spacing
   - max-height
   - min-width
   - outline-offset
   - right
   - top
   - width
   - border-color
   - bottom
   - crop
   - height
   - line-height
   - max-width
   - opacity
   - outline-width
   - text-indent
   - vertical-align
   - word-spacing
   
 - **Transition Duration** 
  -  The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 
  
- **Transition Timing**
 - The transition-timing-function property is used to set the speed in which a transition will move.
 - include linear, ease-in, ease-out, and ease-in-out.  
 - The ease-in value identifies a transition that starts slowly and speeds up throughout the transition,
   while the ease-out value identifies a transition that starts quickly and slows down throughout the transition.
   The ease-in-out value identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.
   
- **Transition Delay**
 **transition-delay** :
  - The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. 


- **Shorthand Transitions**
  - transition, capable of supporting all of these different properties and values.
  - Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, 
    transition-timing-function, and lastly transition-delay.
  -  Do not use commas with these values unless you are identifying numerous transitions.
  
  
 - **Animations Keyframes**
  - The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
  - The vendor prefixes for the @keyframes rule look like the following:
     - @-moz-keyframes  - @-o-keyframes  - @-webkit-keyframes
   
 - **Animation Name** 
  - the animation-name property is used with the animation name .
  
- **Animation Duration, Timing Function, & Delay**
  -  To start, animations need a duration declared using the animation-duration property.
  - A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively.


- **Animation Iteration**
  - To have an animation repeat itself numerous times the __animation-iteration-count__ property may be used.
  - Values for the animation-iteration-count property include either an integer or the infinite keyword.

- **Animation Direction**
  - declare the direction an animation completes using the __animation-direction property__.
  - Values for the animation-direction property include _normal_, _reverse_, _alternate_, and _alternate-reverse_.
  
- **Animation Play State**
  - The __animation-play-state property__ allows an animation to be played or paused using the __running__ and __paused__ keyword 
    values respectively. 
    
- **Animation Fill Mode**
  - The __animation-fill-mode__ property identifies how an element should be styled either before, after, or before and after an animation
    is run.
  - The animation-fill-mode property accepts four keyword values, including __none__, __forwards__, __backwards__, and __both__.
  
 
___________________

## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS :

 1. Fade in : first ,you set the initial state; next, you set the change, for example on hover:.
 2. Change color : EX: .color:hover {background:#53a7ea;}
 3. Grow & Shrink : To grow an element , EX :.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}

-  To enlarge an element we specify a value greater than 1,EX:
.shrink:hover
{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}
 
 4. Rotate elements : is transforming the rotation of an element, EX: .rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}

5. Square to circle :is transitioning a square element into a round one ,EX :.circle:hover
{
        border-radius:50%;
}

6. 3D shadow : This effect is achieved by adding a box shadow,
  and then moving the element on the x axis using the transform and translate properties 
  so that it appears to grow out of the screen. EX: .threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
 
 7. Swing  EX: @-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
       transform: translateX(-5px);
    } 
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}

then : 
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}

8. Inset border :  EX: .border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}