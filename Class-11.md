# Images CSS and SEO with HTML

## Images 

You can control the size of an image using the width and height properties in CSS, just like you can for any other box. By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block-level element using the display property with a value of block. After that, to center an image, there are two common ways in which you can horizontally center an image:
1. On the containing element, you can use the `text-align` property with a value of center.
2. On the image itself, you can use the use the `margin` property and set the values of the left and right margins to auto.

`background-image` property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box, to prevent default we use `background-repeat` property with `no-repeat` as a value. When an image is not being repeated, you can use the `background-position` property to specify where in the browser window the background image should be placed.

There are many properties for back-ground images, in order to mention it, the properties must be specified in the following order, but you can miss any value if you do not want to specify it:
1. background-color.
2. background-image.
3. background-repeat. 
4. background-attachment.
5. background-position. 

## SEO

**Search Engine Optimization (SEO)**: Is a huge topic talking about optimizing techniques that help your site appear nearer the top of search engine results. There are three ways that SEO optimization work with:

1. **Basics**: The idea is working out which terms people are likely to enter into a search engine to find your site and then using these terms in the right places on your site to increase the chances that search engines will show a link to your site in their results.
2. **On-Page Techniques**: The main component of this is looking at keywords that people are likely to enter into a search engine if they wanted to find your site, and then including these in the text and HTML code for your site in order to help the search engines know that your site covers these topics. Ensuring that any images have appropriate text in the value of their alt attribute also helps search engines understand the content of images.
3. **Off-Page Techniques**: Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours.Search engines also look at the words between the opening `<a>` tag and closing `</a>` tag in the link. If the text in the link contains keywords (rather than just **click here** or your **website address**) it may be considered more relevant.