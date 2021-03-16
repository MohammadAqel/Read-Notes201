# Writing Links

*Links are created using the <a> element. Users can click on anything between the opening <a> tag and the closing </a> tag. You specify which page you want to link to using the href attribute*

### Linking to Other Sites

*Links are created using the <a> element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.*

### Linking to Other Pages on the Same Site

*When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.*

### Relative URLs

*Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.*

## Email Links

*To create a link that starts up the user's email program and addresses an email to a specified email address, you use the <a> element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to*

### Opening Links in a New Window

*If you want a link to open in a new window, you can use the target attribute on the opening tag. The value of this attribute should be _blank.*

### Building Blocks

*CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.*

# Article LAYOUT

*The liquid layout uses percentages to specify the width of each box sothat the design will stretch to fit the size of the screen.*

*When trying this in your browser, remember to make the window smaller and larger.A Liquid Layout*

# Layout Grids

*On the right, you can see a set of thick vertical lines superimposed over the top of a newspaper website to show you how the page was designed according to a grid.* 

*This grid is called the 960 pixel grid and is widely used by web designers.*

*Grids set consistent proportions and spaces between items which helps to create a professional looking design.*

*If you flick back through the pages of this book you will see that it, too, has been constructed according to a grid(comprising three columns).*

*As you will see on pages 389-390, it is possible to create many different layouts using this one versatile grid.*

### While a grid might seem like a restriction, in actual fact it:

1. Creates a continuity between different pages which may use different designs.

2. Helps users predict where to find information on various pages.

3. Makes it easier to add new content to the site in a consistent way.

3. Helps people collaborate on the design of a site in a consistent way.

## Possible Layouts:

*These two pages illustrate a 960 pixel wide, 12 column grid. They demonstrate how it is possible to create a wide range of column layouts using this one grid.*

*The page is 960 pixels wide and there are 12 equal sized columns (shown in gray), each of which is is 60 pixels wide.*

*Each column has a margin set to 10 pixels, which creates a a gap of 20 pixels between each column and 10 pixels to the left and right-hand sides of the page.*

## CSS Frameworks

*CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.*


## multiple style sheets

*import.html HTML Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on.*

*Some authors take an even more modular approach to stylesheets, creating separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site.*

*There are two ways to add multiple style sheets to a page:*

1. Your HTML page can link to one style sheet and that stylesheet can use the @importrule to import other style sheets.

2. In the HTML you can use a separate <link> element for each style sheet.

### Summary

1. <div> elements are often used as containing elements to group together sections of a page.

2. X Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.

3. X The float property moves content to the left or right of the page and can be used to create multi-column.

4. layouts. (Floated items require a defined width.)X Pages can be fixed width or liquid (stretchy) layouts.

5. X Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).

6. X Grids help create professional and flexible designs.

7. X CSS Frameworks provide rules for common tasks.

8. X You can include multiple CSS files in one page.