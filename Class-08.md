# CSS Layout

The main key concept in positioning elements is by Building Blocks. CSS treats each HTML element **as if** it is in its own box. This box will either be a *block-level box* or an *inline box*. To control in how much space each box takes up, you have to do that by setting the width of the boxes and sometimes by setting the height too.

If one block-level element sits inside another block-level element then the outer box is known as **The Containing or Parent** element.
It is common to group a number of elements together inside a `<div>` (or other block-level like `<section>`) element.The `<div>` element that contains this group of elements is then referred to as **The Containing Element**.The containing element is always the direct parent of that element.

**Note**: Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide

There are three layout types in CSS, **Fixed**, **Liquid** and **Elastic**, here is one of them with it's own advantages and disadvantages:

**Fixed Width Layouts**: do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels. Here are the advantages and disadvantages for this type:

- Advantages:
1. Pixel values are accurate at controlling size and positioning of elements.
2. The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
3. You can control the lengths of lines of text regardless of the size of the user's window.
4. The size of an image will always remain the same relative to the rest of the page.

- Disadvantages:
1. You can end up with big gaps around the edge of a page.
2. If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
3. If a user increases font sizes, text might not fit into the allotted spaces.
4. The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
5. The page will often take up more vertical space than a liquid layout with the same content.

## CSS Frameworks

CSS frameworks aim to make your life easier by providing the code for common tasks, the main benefit from making framework in CSS is to include the CSS framework code in your projects rather than writing the CSS from scratch. Here are the advantages and disadvantages for using framework: 

- Advantages:
1. They save you from repeatedly writing code for the same tasks.
2. They will have been tested across different browser versions (which helps avoid browser bugs).

-Disadvantages:
1. They often require that you use class names in your HTML code that only control the presentation of the page (rather than describe its content).
2. In order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page (commonly referred to as code “bloat”).

## Multiple Style Sheets

There are two ways to add multiple style sheets to a page:

1. Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets, e.g:
`@import url("fileName.css");`
2. In the HTML you can use a separate `<link>` element for each style sheet, same as link the main CSS style sheet.