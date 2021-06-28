# Read: 08 - More CSS Layout:

**Positioning Elements by Building Blocks:**

**CSS** treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.


### Building Blocks:
- Block-level elements
start on a new line
Examples include:

    < h1 > < p > < ul > < li >


- Inline elements
flow in between
surrounding text
Examples include:

    < img> < b> < i>



If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.


## Positioning Schemes in CSS:
They allow you to control the layout of a page , and they can be accessed by using the position property and the float property.


- **Normal Flow:**
Every block-level element
appears on a new line.

- **Relative Positioning:**
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left.

- **Absolute positioning:**
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position .

- **Fixed Positioning:**
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element. 
- **Floating Elements:**
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.



### Clearing all floats:
we use the (clear) class.
**Ex:**

      <p class="clear">
      
          In 1865, the velocipede (meaning
          "fast foot") attached pedals to the front wheel,
          but its wooden structure made it extremely
          uncomfortable.

      </p>

