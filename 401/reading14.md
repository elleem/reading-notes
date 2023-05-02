## Data Visualization

#### Things I Want to Know More About


1. What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.

Matplotlib is used for 2-D data representation, Seaborn offers even more customization than Matplotlib and built on top of Matplotlib. Bokeh is optimized for the web and is repsonsive and specific to dashboards. 

Matplotlib: plots

Seaborn: plots, but with even more features

Bokeh: data dashboards and interactive visuals


### Matplotlib Tutorial

Allows you to illustrate data, creating a figure, plotting area, plots lines, and decorates with labels, auto generates the x values, if you only provide one value.

Allows for customizing all sorts of properties, using step(), can separate lines for additional space. 

`plt.xlim(X.min()*1.1, X.max()*1.1)`
`plt.ylim(C.min()*1.1, C.max()*1.1)`

Allows customization of ticks, and spines. 

Use label to allow for a legend, use annoatate to add points on the illustration. 

Allows transparency for overlapping items. 

Allows for even more control using figures, subplot, and axes. 

A figure (numbering starts from 1) in matplotlib means the whole window in the user interface. Within this figure there can be subplots. While subplot positions the plots in a regular grid, axes allows free placement within the figure. 

Allows for animations, including drip drop, like rain. Must save this into a video in html in order to show it. 

Wow so many links to cool tutorials, as if the earthquake demonstration weren't cool enough!

There is a full list of galleries. [matplotlib gallery](https://matplotlib.org/2.0.2/gallery.html)

The colors are amazing. 

### Seaborn Tutorial

2. In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.

relational: correction/relationship visualization b/n 2 numerical variables, for example the scatter plots I just submitted for Lab l2. `replot()`

distribution: distribution of a numerical value, for example, density plot or violin plot, histograms.  `displot()`

categorical: Visualizing categorical data. Could show mean value and its confidence interval w/i each nested category, or a swarm plot. `catplot()` although there are a ton of different types belonging to 3 families. 

A library for making statistical graphics in Python, building on matplotlib and integrating with pandas. Lets you focus on the elements of your plots, rather than the details on how to draw them.

There is a default theme, but more options, and you can control style and scale. 

Use `load_dataset()` to get access to the data. 

`#Create a visualization`
`sns.relplot(`
   `data=tips,`
    `x="total_bill", y="tip", col="time",`
    `hue="smoker", style="smoker", size="size",`
`)`

customize a sequential palette using the string interface to `cubehelix_palette():`

The axes-level functions are `histplot()`, `kdeplot()`, `ecdfplot()`, and `rugplot()`. They are grouped together within the figure-level `displot()`, `jointplot()`, and `pairplot()` functions.

The normalization demonstration using the `stat` parameter is really interesting. 

### Bokeh Tutorial

Bokeh is an interactive libary that targets web browsers w/o using JavaScript. 

`from bokeh.io import output_notebook, show`
`from bokeh.plotting import figure`

visual shapes in bokeh are called glyphs.

You can create a scatter plot with many different shapes. 

Supports two types of image display, inlcuding `image` and `image-rgba`. There are many different themes and styles. 

works with lists, NumPy arrays, Pandas, converted to ColumnDataSource and used a data source thruout Bokah. 

Can overlay GoogleMaps. 

### Seaborn Cheat Sheet

[Link to cheat Sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Seaborn_Cheat_Sheet.pdf) 

3. Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?

Well a quick reference guide is a shortcut to finding the functionality of Seaborn and find the appropriate elements that a dev would need for executing their design. Special notes to the breakout of categorical, regression, matrix, and distribution plots. 