# HTML Links, JS Functions, and Intro to CSS Layout

## HTML 

**Relative URLs** can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files. Here are the Relative links types:

1. **Same Folder**: To link to a file in the same folder, just use the file name. (Nothing else is needed.)
2. **Child Folder**: For a child folder, use the name of the child folder, followed by a forward slash, then the file name.
3. **Grandchild Folder**: Use the name of the child folder, followed by a forward slash, then the name of the grandchild folder, followed by another forward slash, then the file name.
4. **Parent Folder**: Use ../ to indicate the folder above the current one, then follow it with the file name.
5. **GrandParent Folder**: Repeat the ../ to indicate that you want to go up two folders (rather than one), then follow it with the file name.

**Tip**: Using target attribute with a value of _blank  for `<a>` tag to open a link in a new window.

## CSS

**Block-level elements**: Which start on a new line and take the whole line. If one block-level element sits inside another block-level element then the outer box is known as the *containing or parent element*.

**Inline elements**: Which flow in between surrounding text.

To control the position of elements, CSS has the following positioning schemes that allow you do that:

1. **Normal flow**: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-by-side, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).
2. **Relative Positioning**: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.
3. **Absolute positioning**: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

Also you can use the *float* property to make something called **Floating Elements**, which allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

## JS

**Functions**: Let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

**Methods**: Are the same as a function, except methods are created inside (and are part of) an object.

**OBJECTS**: To create models of the world using data, and that objects are made up of properties and methods. 

We have two major types of variable, which are:

1. **Global variables**: Use more memory. The browser has to remember them for as long as the web page using them is loaded.
2. **Local variables**: Are only remembered during the period of time that a function is being executed.