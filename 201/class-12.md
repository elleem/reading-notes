## Chart.js, Canvas

### Things I Want to Learn More About
<p>Need to look up Math.PI mentioned in drawing the smiley face. 

### Easily Create Stunning Animated Charts with Chart.JS
<p> chart.js plugin that easily creates graphs, bar charts, and pie charts. </p>
<p> Use canvas tag in html, then retrieve in JS</p>

### Chart.js
<p> reference page for installing chart.js </p>
<p> Be sure to give canvas it's own id for responsiveness. </p>
<p> https://www.chartjs.org/docs/latest/ </p>

### Mdn canvas
<p> width and height, option and can be set using DOM, there is a default. </p>
<p> Uses normal CSS styling, such as border, background, margin. </p>
<p> Does use the fallback content. Does use the close tag. </p>
<p> getContext method, usually specify 2d </p>

### Mdn drawing shapes
<p> Ability to draw rectangles, triangles, lines, arcs, curves. </p>
<p> x and y coordinates within the pixels. Then width and height values.</p>
<p> fillRect draws a filled rectangle, strokeRect draws a rect outline, clearRect.</p>
<p> Paths are a list of points, connected by segments of lines. 1.create a path, 2. use drawing commands, 3. stroke/fill the path to render it. </p>
<p> beginPath () to create a new path. closePath () adds a straight line to the path. stroke() draws the shape. fill()draws a solid shape by filling the path's content area. </p>
<p> When you call fill() any open shapes are closed automatically, so you don't have to call closePath(). But not when you call stroke(), still need to closePath()
<p> moveTo(x,y) is like lifting a pencil from one spot, and going to the next. </p>
<p> lineTo(x,y) will draw straight lines
<p> arc(x, y, radius, startAngle, endAngle, counterclockwise(boolean value)) arcTo(x1, y1,x2, y2, radius)</p>
<p> quadraticCurveTo (cp1x, cp1y, x, y) vs bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y) one versus two control points, can draw hearts and bubbles</p>
<p> wow--this pacman example is amazing. The most important things to note are the use of the fillStyle property on the drawing context, and the use of a utility function (in this case roundedRect()). Use utility functions can reduce the amount of code you need, as well as its complexity. </p>
<p>Path2D() cache or record drawing commands and play back paths quickly. Combine paths with addPath. </p>
<p> SVG paths--pass around pahth data and re-use in SVG and canvas</p>

### Styles and Colors
<p> fillStyle= color, strokeStyle= color, using CSS color values, wow so cool using the loops to create the gradients </p>
<p> Math.PI represent the ratio of the circumference of a circle to its diameter or PI. </p>
<p> translucent shapes: globalAlpha property or by assigning a semi-transparent color to stroke/fill style. </p>
<p> globalAlpha is set at 0.2 for all shapes in the example and layer over until the background disappears. </p>
<p> line properties for lineWidth, lineCap or ends of the lines in butt, round, square, lineJoin or corners in round, bevel, miter, miterLimit establishes a limit on the miter when two lines join at a sharp angle and control the appearence of the junction. </p>
<p> getLineDash, setLineDash with a descriptive value, lineDashOffset with a value. </p>
<p>If you consider a path from (3,1) to (3,5) with a line thickness of 1.0, you end up with the situation in the second image. The actual area to be filled (dark blue) only extends halfway into the pixels on either side of the path. An approximation of this has to be rendered, which means that those pixels being only partially shaded, and results in the entire area (the light blue and dark blue) being filled in with a color only half as dark as the actual stroke color. This is what happens with the 1.0 width line in the previous example code. </p>
<p> createLinearGradient (x1,y1,x2, y2), createRadialGradient(x1, y1, r1, x2, y2, r2), createConicGradient (angle, x, y)</p>
<p> addColorStop() between 0.0 and 1.0
<p> createPattern() with values of repeat, repeat-x, repeat-y, no-repeat. </p>
<p> shadows have 4 properties: shadowOffsetX=float, horizontal distance the shadow should extend, shadowOffsetY=float vertical distance the shadow should extend, shadowBlur= float, size of the blur effect, default of 0, shadowColor= color, CSS colors. 
<p> Canvas fill rules: when using fill you can provide a fill rule algorithm to determine if a point is inside or outside a path, and if it gets filled. </p>
<p> Use evenodd or nonzero.</p>

### Drawing Text
<p> fillText(text, x, y, [, maxWidth]), fill a given text at x, y </p>
<p> strokeText(text, x, y [,maxWidth]), strokes at a given text at x, y </p>
<p> textBaseline=value can be top, hanging, middle, alpha, ideographic, bottom </p>
<p> direction=value ltr, rtl, inherit. </p>
<p> measureText() allows you to find out details about text. </p>
<p> No more Geckos!</p>

### CSS grid garden
<p> grid fits in flexbox, when you have a child in a grid and want to start putting it places use grid-column-start: </p>
<p> Use grid-column-end to extend the item across multiple columns "up to the right hand side"</p>
<p> The first line of the column is counted </p>
<p> You can use negative values to place items. -1 specifies first grid line from the right</p>
<p>
<p>
<p>
<p>
