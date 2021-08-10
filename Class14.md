# Code 201 Class 14 Reading notes:

## CSS:

### Transformers:

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

#### Transform Syntax:

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.


div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

#### 2D Transforms:

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. 

- 2D Rotate
- 2D Scale
- 2D Translate
- 2D Skew

#### Transform Origin:

As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.

The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

Individually the values are treated like that of a background image position, using either a length or keyword value. That said, 0 0 is the same value as top left, and 100% 100% is the same value as bottom right. More specific values can also be set, for example 20px 50px would set the origin to 20 pixels across and 50 pixels down the element.


#### 3D Transforms:

- 3D Rotate
- 3D Scale
- 3D Translate
- 3D Skew


#### Transform Style:

he transform-style property needs to be placed on the parent element, above any nested transforms. The preserve-3d value allows the transformed children elements to appear in their own three-dimensional plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane.


#### Backface Visibility:


When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.

The other value to backface-visibility is visible which is the default value, always displaying an element, no matter which direction it faces.

### Transitions & Animations:


For a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the **:hover, :focus, :active, and :target pseudo-classes**

#### There are four transition related properties:

#### Transitional Property:

Determines exactly what properties will be altered in conjunction with the other transitional properties. 

background property is identified in the transition-property value. Here the background property is the only property that will change over the duration of 1 second in a linear fashion. 

If multiple properties need to be transitioned they may be comma separated within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.

background
- colorbackground
- positionborder
- colorborder
- widthborderspacing
- bottom
- clip
- color
- cropfont
- sizefont
- weightheightleftletter
- spacingline
- height
- margin
- maxheight
- maxwidth
- min-height
- min-width 
- opacity
- outline-color
- outline-offset
- outline-width
- padding
- righttext
- shadowtopvertical
- align
- visibility
- width
- word spacing
- z-index

#### Transition Duration:

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

#### Transition Timing:
The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

#### Transition Delay:
On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property.

### Animations:
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

#### Animations Keyframes:
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

#### Animation Name

Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

#### Animation Duration, Timing Function, & Delay

Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if 
desired. To start, animations need a duration declared using the animation-duration 
property. As with transitions, the duration may be set in seconds or milliseconds.




#### Want To Know More ? 

[Visit our Resources websites](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
