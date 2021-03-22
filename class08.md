# Layout

### Layout in Css:

*CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.*

*The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width).*

*Pages can be fixed width or liquid (stretchy) layouts.*

*Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.*

*Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.*

*Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.*

*Many designers use a grid structure to help them position items on a page, and the same is true for web designers.
CSS Frameworks provide rules for common tasks.*

## Building Blocks

*CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.*

## Containing Elements

*If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.*

## Controlling the Position of Elements

*CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.*

*To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.*

### Normal Flow

*In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be:*

#### position: static

## Relative Positioning

1. position:relative Relative positioning moves an element in relation to where it would have been in normal flow. For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right. You can indicate that an element should be relatively positioned using the position property with a value of relative.

2. position:absolute When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. (They act like it is not there.) The box offset properties (top or bottom and left or right) specify where the element should appear in relation to its containing element.

3. position:fixed Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed. It positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place. It is a good idea to try this example in your browser to see the effect. To control where the fixed position box appears in relation to the browser window, the box offset properties are used.

## Floating Elements

#### float

*he float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside the containing element will flow around the element that is floated.*

## Screen Sizes

*Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.*

## Screen Resolution

*Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.*

## Page Sizes

*Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).*

## Fixed Width Layouts

*Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.*

## CSS Frameworks

*CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.*