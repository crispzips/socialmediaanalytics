# Social Media Analytics with NodeXL
Below you will find a brief tutorial for retrieving, visualizing, and analyzing graph network data from twitter using the free NodeXL platform provided by the non-profit Social Media Research Foundation (SMRF)

## Table of Contents
* [About](#about)
* [Lingo](#lingo)
* [Prep Work - Download and Installation](#prep-work)
* [Dipping Your Toe In](#dipping-your-toe-in)
  * [The Look and Feel](#the-look-and-feel)
  * [Network Graph Introduction to NodeXL](#network-graph-introduction-to-nodexl)
* [Getting Data](#getting-data)
* [Rendering Graphs](#rendering-graphs)
* [Analyzing Networks](#analyzing-networks)
* [Further Reading](#further-reading)
  
## About
Last Updated Feburary 2017  
Created by [Paul Vieth](http://paulkelleyvieth.org/)  
University of Oklahoma Libraries

## Lingo
* vertex (_pl. vertices_) = node = point on graph (depicts object: could be a social media user, an image from flickr, or anything really)
* edge = line that connects two vertices (depicts relationship between two objects)

## Prep Work
### [Download and install the NodeXL Microsoft Excel plugin](http://www.smrfoundation.org/nodexl/installation/)
* NodeXL comes as a Microsoft Excel template. After you install, the program will present itself as an Excel workbook. Each time you intend to work with NodeXL, you will first open this workbook, so store it somewhere handy.
* The Social Media Research Foundation (SMRF) provides a free version of NodeXL. This has limitations on functionality, but is perfect for familiarizing yourself with social media analytics. SMRF provides a PRO version, for more advanced usage with full functionality, and offers discounts for academic users.

## Dipping Your Toe In
### The Look and Feel
When you open the NodeXL template, most everything you're comfortable with about Excel will be there waiting for you.
Just to make sure we're on the same page, your screen should look like this:

![NodeXL Screen Layout](/images/netpres01.PNG)

You'll notice some changes. This isn't a fresh Excel workbook, but has been prepopulated with everything you'll need to work NodeXL's magic.
* The second row of the sheet is filled with labels for all of the ingredients of a network graph: vertex 1, vertex 2, color, width, style, opacity, visibility, label, label text color, label font size, (and an option to add your own columns).
  * Only the first two columns (vertices 1 & 2) are needed to create a network graph, the remaining columns could be considered stylistic extras -- but this is a graph -- so those stylist changes in form symbolically correspond to changes in content. They allow the reader to extract richer meaning from the connections. The width, color, and style (dotted, dashed, solid) of the edges, could convey the intensity, frequency, or probability of a connection between those vertices.
* If you look to the bottom of the window, you will see a series of worksheet tabs. The one currently selected (and which I just described) is the edges tab. There are also tabs for "vertices," "groups," "group vertices," and "overall metrics."
  * The "vertices" tab invokes each vertex and allows you to adjust its style properties (color, shape, size, opacity, image file, visibility, label, label fill color, label position, tooltip, etc.)
  * The group and group vertices tabs allow you to cluster your vertices into groups, or display those groups you generated using algorithms or by certain group properties (more on all this later).
  * The overall metrics tab displays the results of analytic process you ask NodeXL to perform on your network.
* To the right of the worksheets, in a pane labled "Document Actions," is where you generate network graphs from the row/column data generated in/imported into the worksheet section. This is where you can apply different modeling algorithms to your network and visually sift through these algorithmically-generated models. The algorithms NodeXL includes are:
  * [Fruchterman-Reingold](https://en.wikipedia.org/wiki/Force-directed_graph_drawing)
  * [Harel-Koren Fast Multiscale](https://www.researchgate.net/figure/220875983_fig1_Figure-1-a-Harel-Koren-HK-fast-multi-scale-layout-of-a-clustered-network-of-Twitter)
  * Circle
  * Spiral
  * Horizontal Sine Wave
  * Vertical Sine Wave
  * Grid
  * Polar
  * Polar Absolute
  * [Sugiyama](http://www.cs.usyd.edu.au/~shhong/fab.pdf)
  * Random

Here's a good overview of some of the different graphing algorithms (it's pretty self-explanatory which shape algorithms correspond to which examples below):

![Graph Algorithm Example Images](/images/netpres02.png)

* NodeXL makes one more change to the basic Excel template.
 * In the top row tabs ("File," "Home," "Insert," etc.) you will see a tab called "NodeXL Basic" (if you installed the free version)
 * This tab contains everything that can be done with NodeXL:

![NodeXL functions](/images/netpres03.PNG)

### Network Graph Introduction to NodeXL
Another neat, and multimodal, way to learn about NodeXL's functionality is to let NodeXL tell you using NodeXL's functionality. That sounds meaningless, but will become clear.
  
* In the NodeXL tab (between "View" and "Design") --> Help section --> "About" dropdown menu, you will see an option called "Sample Workbook"

Opening that sample workbook automatically opens a new Excel window, creates a new NodeXL template workbook, and populates that workbook with sample (but not random, lorem ipsum-esque) vertices and nodes, and their properties.

* On the right-hand pane labled "Document Actions", you will see a button in its top left corner called "Show Graph." As mentioned above, this creates a network graph from the information in the NodeXL workbook using one of various algorithms to be chosen from a drop down menu. The default algorithm is the Fruchterman-Reingold. Keep this algorithm, and generate the graph for the sample workbook.

You'll get something like this:

![NodeXL Functionality Graph](/images/netpres04.PNG)

This is, in broad strokes, everything that NodeXL (the central hub of this graph) can do. As for the secondary nodes, those connected directly to the hub, this workshop will go through three of them in detail:
* "Data" -- by importing data from twitter
* "Graph" -- by generating graphs using different algorithms from the twitter data we collect
* "Analysis" -- by grouping our nodes according to network relationships and having NodeXL gather metrics on our graph

## Getting Data

Under the NodeXL tab --> "Data" section --> "Import" dropdown menu, you will see a list of all the potential data sources.

![NodeXL Import Options](/images/netpres05.PNG)

If your data has already been collected, you can import it into NodeXL as a Pajek, GraphML, or UCINET Full Matrix DL file. We're not going to get into that today, and that would ignore some of NodeXL's best functionality anyway.

Notice, from the bottom half of the "Import" dropdown, that data can also be taken from
* email networks
* facebook
* twitter
* flickr
* youtube

Well, at least in theory. To import data from most of these sources you need to have NodeXL Pro installed. But NodeXL basic does allow you to import "From Twitter Search Network," meaning you can pull up tweets containing keywords or hashtags, and can control the parameters of that data cull. Like this: 

![NodeXL Import from Twitter Search Network](/images/netpres06.PNG)



## Rendering Graphs

## Analyzing Networks

## Further Reading
