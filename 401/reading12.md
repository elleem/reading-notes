## What is Pandas

#### Things I Want to Know More About



### Pandas in 10

Explain the purpose and basic functionality of the Pandas library.

Pandas must be imported, and helps with data manipulation and analysis. 


What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?

You can call functions for a variety of purposes, including to view the data, specifically DataFrame.head() and DataFrame.tail() to view top and bottom rows. 

Also DataFrame.index and DataFrame.columns for understanding rows and columns. 

use describe() to show a summary of your data. 

You can select your data in a variety of methods. 

np.nan to represent missing data, which is not included in computations. 

You can use df.apply() to inject a user defined function into your data. 

histogramming is pretty cool. 

Be careful of adding things to your data, since it could be costly in time and space. 

There are some elements that look like excel, such as pivoting your data. And some elements that look like SQL, with merging and joining your data. 


### Pandas Getting Started

What are the primary data structures in Pandas, and how do they differ in terms of use cases?

2-D data structure, that can store data of different types, strings, int, floats, etc

Each column is a series. Columns have labels stored in the columns attribute.  Rows have labels or indexs, stored in the index attribute.  

`read_*` methods read data to pandas, and the `to_*` methods store the data. 

`info()` will provide technical information about the dataset

when selecting subset of data, square brackets are used. You can use single col/row label, a list, a slice, a conditional or a colon. 

use loc when using the row/ col names.   use iloc when using the positions in the table. 

plot(), scatter() plot.box() or plot.area (figsize = (12,4) subplots = True) for a  visual of the information. 

You can also define the x and y labels. Any plot created by pandas is a Matpotlib object. 

create a new column by assigning the output to the df with a new col name between []

operations are element-wise--no loops!!

use rename with a dict or function to rename row labels or col names. 


### Pandas Tutorial


### What is Pandas


### Master Pandas






Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?