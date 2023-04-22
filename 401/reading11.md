## Data Analysis

#### Things I Want to Know More About



### What is Jupyter Lab

What are the key features and benefits of Jupyter Lab, and how does it differ from Jupyter Notebook?

Jupyter Lab is a text editor that offers a unified model for viewing and handling data formats, with many different allowable formats. 

It also allows multi-window support (side by side views), integrated terminal, drag and drop functionality.

It sounds like Lab allows for multiple files vs a single file with Notebook, but both are supported. 

- = to zoom, [] for rotation, 0 to reset. You could go wild with keyboard shortcuts. 

Command mode when opening the notebook. Use the arrow keys to navigate. a to add a cell above, b for below, dd to delete.  y to code, m for markdown, enter to edit the currently active cell. 

markdown note: create equations with $   $

shift enter to run the cell

### Numpy Tutorial

ssv semicolon separated values vs csv 

read the data into a list of lists

use the numpy.array function, pass in list of lists, will create a NumPy array with the same # of rows and columns. 

zero indexed



## Numpy Arrays

What are the main functionalities provided by the NumPy library, and how can it be useful in Python programming, particularly for scientific computing and data manipulation tasks?

Open source multi-dimensional array manipulation and mathematical functions, including trig, exponential and logarithms, linear algebra, and random numbers. Additionally, includes sorting, filtering, searching functions. 

Allows you to perform mathematical operations on large arrays of data. 

Explain the basic structure and properties of NumPy arrays, and provide examples of how to create, manipulate, and perform operations on them.

ndarray, which is a collection of items of the same type, each item in the ndarray takes the same size of block in the memory.  zero-based index, that can be sliced.  Includes more numerical types than python, usch as complex_


`print(wines[:3])`  or 

```python
import numpy as np 
a = np.array([[1,2,3],[4,5,6]]) 
print a.shape
```

`f = np.array([1, 2, 3]) * 2`

```python 
a = np.array([[1,2,3],[4,5,6]]) 
a.shape = (3,2) 
print a 
```
the above resizes an array, but you can also arange an ndarray, and return the length of each item in bytes. 
