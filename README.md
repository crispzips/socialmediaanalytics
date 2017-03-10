#Social Media Analytics with NodeXL
Below you will find a brief tutorial for retrieving, visualizing, and analyzing graph network data from twitter using the free NodeXL platform provided by the non-profit Social Media Research Foundation (SMRF)

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
* The Social Media Research Foundation (SMRF) provides a free version of NodeXL. This has limitations on functionality, but is perfected for familiarizing yourself with social media analytics. SMRF provides a PRO version, for more advanced usage with full functionality, and offers discounts for academic users.

## Dipping Your Toe In
### The Look and Feel
When you open the NodeXL template, most everything you're comfortable with about Excel will be there waiting for you.
Just to make sure we're on the same page, your screen should look like this:
![NodeXL Screen Layout](netpres01.png)
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
  * [Circle](
