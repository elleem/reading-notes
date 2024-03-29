## Ten Thousand 4

#### Things I Want to Know More About



### Dunder Methods

What is the purpose of dunder methods in Python? 

They let you emulate the behavior of built-in types, using a data model, as if it is an API. 

Provide an example of a commonly used dunder method.

`__init__` is a special method to construct objects. 

`__repr__` and `__str__` are for object representation, official and informal string representation

`__len__`, `__getitem__`, `__reversed__` for iteration when in classes

`__eq__`, `__lt__`  which are == and <

`dir()` explores the attributes and methods of an object or module, can be called w/ or w/o an object. 

use `__add__` to add and `__radd__` to reverse add. 

use `__call__` to make objects callable, tell the method what you want it to do with items in the object. In this example, it is told to print transacations and the start amount. 

`__enter__` and `__exit__` will function as context managers

### Statistics Probability

Probability: chance of event occurring, which can help us make predictions about how often events will happen based on data gathered. 

Python allows us to model this process in code. 

Probability distributions, ,thr normal distribution is significant to pobability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule. 

Central Limit Theorem: the distribution of these estimates will look like a normal distribution. We can hone in on a theoretical ideal given by probability even when we don't know the true probability. The average of many trials means will approach the true mean. 

Three Sigma Rule: empirical rule or 68-95-99.7 rule, how many of our observations fall within a certain distrance of the mean. The average distance an observation in the data set is from the mean. 

Given a normal distribution, 68% of your observations will fall between one standard deviation of the mean. 95% will fall within two, and 99.7% will fall within three. 

Z-score is a simple calculation that answers the question: given a data point, how many standard deviations is it away from the mean? compared w/ a z-table it tabulates the cumulative probablity of a standard normal distribution up until a given z-score. a standard normal is a normal distribution wiht a mean of 0 and a standard deviation of 1. 


### Intro to Statistics

Statistical features, such as boxplots, created via median, max, min values. 

Terms: Third quartile is 75% of the data, first quartile is 25% of the data. 

Boxplots deliver a lot of infromation: small data is close together, grande data is further apart, the median helps you understand where the weight it is on data set. 

Probability distribution,  percent chance that an event will occur, function of the probability of all possible values

Uniform distribution, on/ off distribution

Poisson distribution, discrete porbability distribution that a certain number of events will occur in a fixed time or space, given the average rate at which these events occur. ie: an average of 10 cars pass by an intersection per hour, we can use poisson to understand the probability of seeing 5 cars in a given hour. 

Bayesian statistics (does take into account added evidence, may be used when prior data may not be a good indicator of probability) versus frequentist statistics (analyze probability only with prior data)

Note: Naive Bayes classifier, up sampling, down samplling, dimensionality reduction

Statistical features like bias, vairance, and many others help us explore a dataset to gain valuable insights. <br>
Probability distributions define the % chance that some event will occur and can be used to understand the spread of data. <br>
Bayesian statistics express probability as a degree of belief in an event which can change as new infromation is gather, rather than a fixed value based on frequency <br>

### Ethics

In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?

Is it even a scam if you don't make it on Coffeezilla?

Does not properly credit people who he takes code from. Does not fork repos, instead clones them. Takes literally the whole code. 

Proper credits on projects. 

### Statistics Module

Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.

Library that provides a set of function for performing basic statistical operations on numerical data, at the level of graphing and scientific calculators. 

data = [10, 20, 30, 40, 50]

stdev = statistics.stdev(data)

print(stdev)

output: 15.811388300841896