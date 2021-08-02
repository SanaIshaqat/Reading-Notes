# Code 201 Class 08 Reading notes:

## Css :


### CSS Layouts:

Controls where each element sits on a page and how to create attractive page layouts.

- Different ways to position elements using normal
flow, relative positioning, absolute positioning and floats.
- Various devices have different screen sizes
and resolution, and how this affects the design process.
- Difference between fixed width and liquid layouts,
and how they are created.
- Use grids to make page designs look more professional.


**Block-level boxes** start on a new line and act as the main building blocks
of any layout, **while inline boxes** flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). 

To separate boxes, you can use
borders, margins, padding, and background colors.

Block-level elements start on a new line.

Examples include:

< h1> < p> < ul> < li>

Inline elements flow in between surrounding text.
Examples include:

< img> < b> < i>

**Containing Elements**

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

**Controlling the Position of Elements**

CSS has the following positioning schemes that allow you to control the layout of a page: **normal flow, relative positioning, and absolute positioning** . 

You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.


**Normal flow**
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).
**Relative Positioning**
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.
**Absolute positioning**
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.
**Fixed Positioning**
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.
**Floating Elements**
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.

### Screen Sizes :

**A Fixed Width Layout**

- To create a fixed width layout,
the width of the main boxes on
a page will usually be specified
in pixels (and sometimes their
height, too).

- The fixed width layout will stay
the same width no matter what
size the browser window is,
whereas the liquid layout will
stretch (or shrink) to fill the
screen.
 
**A liquid Layout**

The liquid layout uses
percentages to specify the width
of each box so that the design
will stretch to fit the size of the
screen.

### Summary:

* < div> elements are often used as containing elements
to group together sections of a page.
* Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts.
* Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.










#### Want To Know More ? 
[Visit our Resources website](https://www.w3schools.com)
OR
[Books](https://www.wiley.com/en-us/Web+Design+with+HTML%2C+CSS%2C+JavaScript+and+jQuery+Set-p-9781119038634)