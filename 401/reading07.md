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

allows you to modify the standard behavior of a global or local value by taging the value with the key word and then sapce and then the name of the value.



### Big O

In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

### Rolling Dice Examples

Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.