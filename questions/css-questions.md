# CSS Questions:

* What is CSS selector specificity and how does it work?
--The selector specificity determines which style declarations are applied to an element:
- Inline styles - an inline style is attached directly to the element to be styled...i.e. h1, p
- IDs - a unique identifier for the page elements.  Specified on an element, and denoted in CSS with a # tag.
- Classes, attributes, and pseudo-classes - this includes:
  - classes, an identifier specified on the element and denoted in CSS with a . before the class name.
  - [attributes] and pseudo-classes such as :hover, :focus.
- Elements and pseudo-elements - includes element names and pseudo-elements, such as h1, div, :before, and :after.

[Specificity Reference](https://www.w3schools.com/css/css_specificity.asp)

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
Majorly:
- CSS resets aim to remove all built-in browser styling.  All HTML elements, like h1 and p, will have the same styling, and need to be styled manually.
- Normalize CSS aims to make built-in browser styling consistent across browsers.  Elements like h1 will appear bold, larger, etc...across all browsers... you then add only the differences in decoration your design needs.
- If the design allows, and normal conventions of styling are followed, using normalize.CSS, instead of CSS reset, will make CSS smaller and faster to write.

[Normalize CSS vs. Reset CSS](https://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css)

* Describe Floats and how they work.
--The float property is used for positioning elements and layout on web pages, and it can have one of the below values:
- left - the element floats to the left of its container.
- right - the element floats to the right of its container.
- none - the element does not float (will be displayed where it occurs in the text).  Default.
- inherit - the element inherits the float value of its parent.

- In simple use, the float can be used to wrap text around images.

--The CSS clear property specifies what elements can float beside the cleared element and on which side.

[Floats](https://www.w3schools.com/css/css_float.asp)



* Describe z-index and how stacking context is formed.
--The CSS z-index property specifies the stack order of an element.  An element with greater stack order is always in front of an element with a lower stack order.  The z-index only works on positioned elements (relative, absolute, fixed.)
[z-index](https://www.w3schools.com/cssref/pr_pos_z-index.asp)

* Describe BFC(Block Formatting Context) and how it works.
--BFC is a part of the visual CSS rendering of a web page. It's the region in which the layout of block boxes occurs and in which floats interact with other elements.
- A BFC contains everything inside of the element creating it, they are important for the positioning and clearing of floats, as they only apply to things within the same BFC, not things outside of their BFC.
- A block formatting context is created by a few things, see the ref for more info:
[MDN-BFC](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context)

* What are the various clearing techniques and which is appropriate for what context?
-

* How would you approach fixing browser-specific styling issues?
* How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
* What are the different ways to visually hide content (and make it available only for screen readers)?

* Have you ever used a grid system, and if so, what do you prefer?
- Yes, I've used CSS Grid, and the built in grid in the Materialize framework.  Depending on the application, I prefer to use the frameworks, as for consistency and fluidity of style in the document.  Alternatively, I have used Flexbox.
[CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
[Materialize Grid]()
[CSS Flexbox]()

* Have you used or implemented media queries or mobile specific layouts/CSS?
* Are you familiar with styling SVG?
* Can you give an example of an `@media` property other than `screen`?
* What are some of the "gotchas" for writing efficient CSS?
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* What is the CSS `display` property and can you give a few examples of its use?
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?
