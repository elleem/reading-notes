## CSS

#### CCS Helps you *Style* a Website

- html structures the doc
- applies rules to html elements (colors, size)
    - specify html element
    - then add {}       
    - values:what controls the value, such as the name of the color
    - generally broken into modules that you can research
    - [Background Color](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)
    - [Border color](https://developer.mozilla.org/en-US/docs/Web/CSS/border-color)
    - [Color](https://www.w3schools.com/cssref/pr_text_color.asp)
    - Note on color: *color*, initial, inherit
    - [Reference sheets](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
    - [Meyer's CSS Tool](https://meyerweb.com/eric/tools/css/reset/)


 #### CSS Specs

 > The browser support status is shown on every MDN property page in a section named "Browser compatibility" (use this to check if the property can be used on your website).

 - external (must be saved as CSS), internal (singular style), inline (applies to one element)
 > With an external style sheet, you can change the look of an entire website by changing just one file!

> Each HTML page must include a reference to the external style sheet file inside the "link" element, inside the head section.

> An internal style sheet may be used if one single HTML page has a unique style.

> The internal style is defined inside the "style" element, inside the head section.

> An inline style may be used to apply a unique style for a single element.

>To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

- multiple style sheets

### Cascading Order Is: 
Inline style (inside an HTML element)
External and internal style sheets (in the head section)
Browser default