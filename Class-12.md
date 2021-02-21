# Chart.js & Canvas with HTML

## Charts.js

**Charts** are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of other options.

## Canvas

 `<canvas>` element looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. It has only two attributes and both are optional, **width** and **height**. When no width and height attributes are specified, the canvas will initially be *300 pixels* wide and *150 pixels* high.

 **Tip**: If your renderings seem distorted, try specifying your width and height attributes explicitly in the Canvas attributes, and not using CSS.

 The Canvas element has a method called `getContext()`, used to obtain the rendering context and its drawing functions. `getContext()` takes one parameter, the type of context. Canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes. 
 
 There are three functions that draw rectangles on the canvas:
 1. `fillRect(x, y, width, height)`: To draws a filled rectangle.
 2. `strokeRect(x, y, width, height)`: To draws a rectangular outline.
 3. `clearRect(x, y, width, height)`: To clears the specified rectangular area, making it fully transparent.
 
 Each of these three functions takes the same parameters. `x` and `y` specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. `width` and `height` provide the rectangle's size.

For Charts, if we want to apply colors to a shape, it isn't using `color` or `background-color` properties, there are two new important properties we can use:
1. `fillStyle`: Sets the style used when filling shapes.
2. `strokeStyle`:Sets the style for shapes' outlines.

As well as regarding to canvas rendering context, there are two specific methods to render text:
1. `fillText(text, x, y [, maxWidth])`: Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2. `strokeText(text, x, y [, maxWidth])`: Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.