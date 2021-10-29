# Code 201 Class 12 Reading notes:

## HTML & JS:

### Charts:


Creating a Chart It's easy to get started with Chart.js. All that's required is the script included in your page along with a single < canvas> node to render the chart.

### Drawing a line chart:

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

< canvas id="buyers" width="600" height="400"></ canvas>
Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

< script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</ script>
(We can actually pass some options to the chart via the Line method, but we’re going to stick to the data for now to keep it simple.)

Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins ‘var buyers=’:

var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}

### Drawing a pie chart:

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

**< canvas id="countries" width="600" height="400"></ canvas>**
Next, we need to get the context and to instantiate the chart:

var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
You’ll notice that this time, we are going to supply some options to the chart.

Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section:

var pieData = [
	{
		value: 20,
		color:"#878BB6"
	},
	{
		value : 40,
		color : "#4ACAB4"
	},
	{
		value : 10,
		color : "#FF8153"
	},
	{
		value : 30,
		color : "#FFEA88"
	}
];

Now, immediately after the pieData we’ll add our options:

var pieOptions = {
	segmentShowStroke : false,
	animateScale : true
}
These options do two things, first they remove the stroke from the segments, and then they animate the scale of the pie so that it zooms out from nothing.

### Drawing a bar chart:

Finally, let’s add  a bar chart to our page. Happily the syntax for the bar chart is very similar to the line chart we’ve already added. First, we add the canvas element:

**< canvas id="income" width="600" height="400"></ canvas>**
Next, we retrieve the element and create the graph:

var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);
And finally, we add in the bar chart’s data:

var barData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "#48A497",
			strokeColor : "#48A4D1",
			data : [456,479,324,569,702,600]
		},
		{
			fillColor : "rgba(73,188,170,0.4)",
			strokeColor : "rgba(72,174,209,0.4)",
			data : [364,504,605,400,345,320]
		}

	]
}
As you can see, the data is largely the same, except this time we’ve chosen to use RGBA to specify our colors which allows us to add transparency.


## Drawing shapes with canvas:

### Drawing rectangles:

Unlike SVG, < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

**fillRect(x, y, width, height)**
Draws a filled rectangle.

**strokeRect(x, y, width, height)**
Draws a rectangular outline.

**clearRect(x, y, width, height)**
Clears the specified rectangular area, making it fully transparent.

Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.

### Drawing paths:

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

**beginPath()**
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.

**closePath()**
Adds a straight line to the path, going to the start of the current sub-path.

**stroke()**
Draws the shape by stroking its outline.

**fill()**
Draws a solid shape by filling the path's content area.
The first step to create a path is to call the beginPath(). 
Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.

The second step is calling the methods that actually specify the paths to be drawn. We'll see these shortly.

The third, and an optional step, is to call closePath(). This method tries to close the shape by drawing a straight line from the current point to the start. If the shape has already been closed or there's only one point in the list, this function does nothing.



#### Want To Know More ? 

[Visit our Resources website](https://www.w3schools.com)
OR
[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
