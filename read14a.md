# Read: 14a - CSS Transforms, Transitions, and Animations

## *CSS Transforms:


- In CSS3 there are a lot of ways to position and alter elemnets. 
- Now we can  use alternative ways to size and position a layout.
 
- The new ways can be done by using the **transform** property:

The **transform** property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.


### - Transform Syntax:

    div {
      -webkit-transform: scale(1.5);
        -moz-transform: scale(1.5);
          -o-transform: scale(1.5);
              transform: scale(1.5);
    }




## * CSS Transitions & Animations:

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.


### - Transitions :
    .box {
      background: #2db34a;
      transition-property: background;
      transition-duration: 1s;
      transition-timing-function: linear;
    }
    .box:hover {
      background: #ff7b29;
    }



## * Simple CSS3 Transitions to use:

1. **Fade in.**
2. **Change color.**
3. **Grow & Shrink.**
4. **Rotate elements.**
5. **Square to circle.**
6. **3D shadow**
7. **Swing**
8. **Inset border**
