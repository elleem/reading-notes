## Operators

### Types of Operators

- assignment assigns value to its left operand based on the value of the right operand, that's why arthmitic is written x+=f()

        -ex: x=f()
        
- comparison
- arithmetic
- bitwise
- logical
- string
- conditional (ternary) is condition? val1: val2, if the condition is true, the operator has a value of val1, otherwise it has a value of val2 

        - ex: var status - (age>=18)? 'adult': 'minor';
- comma
- unary is operator operand or operand operator

        - ex: 3+3 or x*y

- relational
- binary is operand1 operator operand2

        -ex: x++ or ++x


### Object

- a collection of properties, or an associative array
- a poperty is an an assocation between a name and a value
- an object is a standalone entity with properties (variables), like a cup, which can have a design, weight, etc. 
- object.Name.propertyName are case sensitive, always begin with lower case, period was the punctuation

Here is an object: 

        const myCar = new Object();
        myCar.make = 'Ford';
        myCar.model = 'Mustage';
        myCar.year = 1969;

Here is an object initializer, a comma-delimited list of zero or more pairs of property names and associated values of an object, enclosed in {}

        const myCar = {
            mark: 'Ford'
            model: 'Mustang'
            year: 1969
        }

### Assignments 

- generally used within a variable declaration (const, let, var), or as standalone statements.


### Loops

- comma operators or , evaluates both operands and returns the value of the last operand. primarily used in a loop and allows multiple variables to be updated each time through the loop. Often 2 statements are used. 

- statements for loops in js are: 

        for statement
        do...while statement
        while statement
        labeled statement
        break statement
        continue statement
        for...in statement
        for...of statement

#### For

for repeats until aspecified condition evaluates to false

        for ([initialExpression]; [conditionExpression]; [incrementExpression]) statment


#### do...while

repeats until a specified condition evaluates to false

        do
        statement
        while (condition);


#### While

executes statements as long as the condition is true

        while (condition)
        statement


#### labeled

provides a statement with an indentifier that lets you refer to it elsewhere, value is any identifier that is not a reserved word

        label :
          statement

#### Break

use the break to term a loop

        break;
        break [label];

#### Continue 

use to restart a while, do-while, for, or label

        continue [label];

#### for....in

iterates a specified variable over all the enumerable properties of an object

        for (variable in object)
        statement

#### for...of 

creates a loop iterating over iterable objects, like array, map, set, arugments object, invoking a customer iteration hook with statements to be executed for the value of each distinct property

        for (variable of object)
        statement

