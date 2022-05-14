## Images, Color, Text

### Things I Want to Know More About
<p>How to ensure my pages are readable, how to create a fall back color? </p>

### Images
<p> Use an image folder. Tags for images <\img> <\src> <\alt> <\title> <\height> <\width>. Be sure to specify height and width because images take longer to load. Placement impacts the display when paired with text and are dictated by the elements in the html, such as block (heading1) and inline <\img>. </p>
<p> Save images in the right format, size, use the correct resolution (most computers only show 72 px per inch). Save images at the same width and height you want to use on your page. Save images with a resolution of 72 ppi. </p>
<p> Images with different colors should be jpegs. Use gif or png when saving images with few colors or large areas of the same color. <p>
<p> Vectors are resolution independent, created by placing points on a grid and drawing lines between those points. SVG isn't widespread...</p>
<p> <\figure> and <\figcaption></p>
<p> Use JPEG for images that contain nature or variation in color and intensity is smooth. </p>
<p> Use PNG for any images that needs transparency or for images with text and objects like logos. Use GIF for animations. </p>
<p> Lossless (PNG, also higher storage and GIF) and lossy (JPEG) compression either lose data during compression, or does not. JPEGs are not transparent. PNGs and GIFs are. JPGs support a lot of colors. PNG and GIF only 256. </p>

### Color
<p>Color can be coded with RGB (red, green, blue) values, HEX codes, HSLA (hue, saturation, lightness, alpha(transparency)), and 147 color names, which are not commonly used.</p> 
<p> Padding seperates text from the edges of the box. </p>
<p> Shoot for medium contrast. You can specify opacity via CSS between 0.0 and 1.0. </p>
<p> Saturation (the amount of gray), lightness (the amount of white or dark)

### Text
<p> Two categories: those that directly impact the font and those that would have the same effect on text no matter what font is selected. </p>
<p> Serif with the extra details, sans serif w/o those details, monospace is every letter is fixed width. Font stack/font-family so that if a font isn't installed the browser has a choice. </p>
<p> Ems, width of one m. The default size of font is 16 in browsers, so scale accordingly. </p>
<p> You can tell text to be uppercase or lowercase with CSS, may want to consider letter spacing or line-height.  </p>
<p> Text decoration propetry allows for bold, etc. </p>
<p> Text can be align, left, center, right, justify. </p>
<p> Vertical align: baseline, sub, super, top, text-top, middle, bottom, text-bottom. </p>
<p> Text-indent values are in px. </p>
<p> Text shadow noted in px.</p>
<p> Pseudo elements (with tag first) include :first-letter, :first-line, :link, :visited, :hover, :active, :focus </p>
