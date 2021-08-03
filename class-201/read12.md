### EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS

* Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool.

* The first thing we need to do is download Chart.js.

* **Drawing a line chart** 
     1. create a `canvas` element in our HTML in which Chart.js can draw our chart. 
     2.  write a script that will retrieve the context of the canvas
     3. create our data


* **Drawing a pie chart**
     1.  need the canvas element: `<canvas id="countries" width="600" height="400"></canvas>`
     2. need to get the context and to instantiate the chart 
    

#### Basic usage of canvas
* The `<canvas>` element has only two attributes, width and height.
* The `<canvas>` element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas.
* The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it.
*  The` <canvas>` element has a method `called getContext()`, used to obtain the rendering context and its drawing functions.` getContext()` takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D.

#### Drawing rectangles
There are three functions that draw rectangles on the canvas:

1. **fillRect(x, y, width, height)** Draws a filled rectangle.
2. **strokeRect(x, y, width, height)** Draws a rectangular outline.
3. **clearRect(x, y, width, height)** Clears the specified rectangular area, making it fully transparent.


##### Drawing paths
A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color,Here are the functions used to perform these steps:

1. **beginPath()** Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. Path methods : Methods to set different paths for objects.
     1. **closePath()** Adds a straight line to the path, going to the start of the current sub-path.
     2. **stroke()** Draws the shape by stroking its outline.
     3. **fill()**Draws a solid shape by filling the path's content area.

  optional :**closePath()** This method tries to close the shape by drawing a straight line from the current point to the start. If the shape has already been closed or there's only one point in the list, this function does nothing.


#### Drawing a triangle
**moveTo(x, y)** Moves the pen to the coordinates specified by x and y.

#### Lines
**lineTo(x, y)** Draws a line from the current drawing position to the position specified by x and y.


#### Arcs

1. **arc(x, y, radius, startAngle, endAngle, anticlockwise)** Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
2. **arcTo(x1, y1, x2, y2, radius)** Draws an arc with the given control points and radius, connected to the previous point by a straight line.
