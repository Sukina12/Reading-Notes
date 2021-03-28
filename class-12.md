# Class 12 Summary:

## Charts:

* Charts for displaying data visually . They are easier to look at and convey data quickly but not always to create.

* Chart.js a great way to get started with charts. 

* java Script uses HTML5 canvas element to draw the graph.

* setting up charts:
1. download Chart.js
2. copy the chart.min.js into the directory.
3. create a new HTML page and import the script with single <canvas> to render the chart.
<canvas id="tutorial" width="150" height="150"></canvas>


## Canvas:

* canvas element has only 2 attributes (width & height), id attribute to identify it in a script.

* canvas can be styled such as (margin, border, background ... ).

* The canvas is blank. A script first needs to access the rendering context and draw on it. The <canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context.

## Drawing shapes with canvas:

* canvas supports two primitive shapes : rectangles & paths (lists of points connected by lines). the other shapes can be created by combining one or more paths.

##### Draw Rectangle:

fillRect(x, y, width, height) -------> Draws a filled rectangle.
strokeRect(x, y, width, height) -----> Draws a rectangular outline.
clearRect(x, y, width, height)-------> Clears the specified rectangular area, making it fully transparent.

##### Draw Paths:
1. create the path.
2. drawing commands to draw into the path.
3. stroke or fill the path to render it.

beginPath() -----> Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods ----> Methods to set different paths for objects.
closePath() -----> Adds a straight line to the path, going to the start of the current sub-path.
stroke() --------> Draws the shape by stroking its outline.
fill() ----------> Draws a solid shape by filling the path's content area.
moveTo(x, y) ----> Moves the pen to the coordinates specified by x and y.

##### Lines:

For drawing straight lines, use the lineTo() method.

lineTo(x, y) -----> Draws a line from the current drawing position to the position specified by x and y.

##### Colors:

fillStyle = color ------> Sets the style used when filling shapes.
strokeStyle = color ----> Sets the style for shapes' outlines.

##### Line Styles:
lineWidth = value -----> Sets the width of lines drawn.
lineCap = type --------> Sets the appearance of the ends of lines.
lineJoin = type -------> Sets the appearance of the "corners" where lines meet.
miterLimit = value ----> Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
getLineDash() ---------> Returns the current line dash pattern array containing an even number of non-negative numbers.
setLineDash(segments) --> Sets the current line dash pattern.
lineDashOffset = value --> Specifies where to start a dash array on a line.

##### Drawing Text:
The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth]) --------> Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth]) ------> Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

##### Styling Text:
font = value ----------> The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
textAlign = value ------> Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
textBaseline = value ---> Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
direction = value ------> Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

**Thank You**

**Sukina AbuHammad**
