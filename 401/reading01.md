### Introductory readings

#### Pain vs Suffering
What’s your perspective?
Why are you doing this?
Do you want what comes at the end of this journey?
Are you doing this for you?

#### Beginners Guide to Big O ORDERS OF GROWTH

describes performance or complexity of the algorithm.
specific to the worst case scenario (the carrier pigeon)

O(1) always executes in the same time/space regardless of input

O(N) grows linearly, in direct proportion to the size of the data set

O(N ^2^) performance, directly proportional to the square of the size of the data set

O(2^N) doubles growth w/ ea addition to the data set, ie Fibonacci numbers

Logarithms 
binary search--rips the book in 1/2 and searches each half of the pages
can be described as O(log N)


#### Names and Values in Python

Names refer to values

Names are reassigned independently 
x=23
y=x
x=12 
y is still 23

values live until no reference
x="hello"
x="world"

assignment never copies data (two names refer to the same list)
nums = [1,2,3]
other = nums

Changes visible thru all names
nums = [1,2,3]
other = nums
nums.append(4)
print(other)
1,2,3,4 

mutable aliasing, which can results in surprise

immutable vales can't alias=ints, floats, strings, tuples
x = "hello"
y = x
x = x + "there"

x is now "hello there"

change vs rebinding vs mutating
rebinding x = x + 1
mutating nums.append(7)
rebind lists nums = nums + [7]

x += y is conceptually x = x + y
but actually it is calling the iadd method x = x.__iadd__(y) pseduo code

num_list += [4,5]
num_list.extend([4, 5]); <--you are mutating in place here, you are NOT rebinding

references can be more than just names
nums = [1,2,3]
x = nums [1] really both 2, each int is its own value being refered to by the list element

lots of things are references
object attributes
list elements
dict values, keys
anything on the left

a for loop is assigning over and over
I think to solve the ex, I would print(nums*10)

function arguments are assignments
stack frames

don't mutate values, <b>make a new list</b>

names have no type
values have no scope

call by assignment

Note: pythontutor.com

#### Codenewbie - A friendly intro to Big O Notation
7:55 linked lists, like arrays, 2 parts: one holds the data and one holds the reference and tells us where the next is located
nodes--don't have to live next to each other, as long as they know where to find the next node

9:20 singly link list, starting node that you traverse in one direction (forward)

10:32 the last node points to null

11:45 doubly linked list, two directions

12:45 circular linked list, creates a circle, points back to the first node

13:24 still have a head node, which is how you enter a linked list

16:28 can visualize this with grades

18:26 constant time, does matter how much your input grows

20:05 how can you do more things, when you have more things? 2 secs to add a book on top of the stack 









