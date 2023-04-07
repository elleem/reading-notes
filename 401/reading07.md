## Ten Thousand @

#### Things I Want to Know More About



### Python Scope

Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

Scope rules how variables and names are looked up in your code, determining the visibility of a variable w/n the code. Follows Local Enclosing Global Built-in rule. 

Global values are the top-most scope and visible to all your code. 

Local values are only visible within the code, created at the function call, so you can have as many different scopes as function calls. 

You can have built in scope via key words.

```py
global_variable = "I am global"

def print_variables():
    local_variable = "I am local"
    print(local_variable)
    print(global_variable)

print_variables()
print(global_variable)
```

How do the global and nonlocal keywords work in Python, and in what situations might you use them?

allows you to modify the standard behavior of a global or local value by taging the value with the key word and then space and then the name of the value.



### Big O

In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

Gives the worst case time and space calculation of your alogrithm based on the input.

### Rolling Dice Examples

Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

I would simulate a dice roll by 
1. importing the random module
2. specifying the bounds of the random generation (1,6)

To extend this above I would
1. specify the number of trials
2. decide the number I am looking for
3. count how many times I rolled the desired number
4. Finally, then I could use the count to divide the number of trials and calculate the probability.

```python
import random
count = 0
trials = 1000
num = 6

def roll():

for i in range(trials):
  dice_roll = random.randint(1,6)
    if dice_roll == num:
        count += 1

probability = count/trials
```