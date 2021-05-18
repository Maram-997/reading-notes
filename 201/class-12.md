# Chart.js, Canvas
* Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.
1. firstly, The Setting up
The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in.
2. Then create a new html page and import the script:
3. Drawing a line chart: create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:
> `<canvas id="buyers" width="600" height="400"></canvas>`
4. Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:
> `<script>`
>   ` var buyers = document.getElementById('buyers').getContext('2d');`
>    `new Chart(buyers).Line(buyerData);`
>   `</script>`
5. Inside the same script tags we need to create our data: it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.
6. Drawing a pie chart:First, we need the canvas element:V
>`<canvas id="countries" width="600" height="400"></canvas>`
7. Next, we need to get the context and to instantiate the chart:
>`var countries= document.getElementById("countries").getContext("2d");`
>`new Chart(countries).Pie(pieData, pieOptions);`
8. Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section.
9. Drawing a bar chart: First, we add the canvas element. then, we retrieve the element and create the graph. And finally, we add in the bar chart’s data

## THE BASIC USAGE 
At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties.
## DRAWING SHAPES WITH CANVAS
#### Drawing rectangles:
`<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.
![img](/images/drawing-rectangels.png)
* Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size. 
#### Drawing paths
A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it
![img](/images/drawing-paths.png)

## APPLYING STYLES AND COLORS
#### Colors
If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
#### Transparency 
 We can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.
 * Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them.
 #### Line styles
 There are several properties which allow us to style lines:(lineWidth, lineCap, lineJoin, miterLimit, getLineDash(segments), lineDashOffset)
 ## DRAWING TEXTS
 The canvas rendering context provides two methods to render text:
`fillText(text, x, y [, maxWidth])`
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
`strokeText(text, x, y [, maxWidth])`
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
#### Styling text
There are some more properties which let you adjust the way the text gets displayed on the canvas:(font, textAlign, textBaseline, direction, )