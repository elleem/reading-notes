## Javascript Continued

### Expressions and Operators

- types of operators

   -  assignment, comparison, arithmetic, bitwise, logical, string, conditional *(ternary)*, comma, unary, and relational
   - in js there are binary and unary operators and one special ternary operator, the conditional operator
    - ex of a binary: operand1 operator operand2
    - ex of a unary: operator operand or operand operator
 
    > An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

    > Assigning to properties
    If a variable refers to an object, then the left-hand side of an assignment expression may make assignments to properties of that variable.

    > For more complex assignments, the destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.

    - Chaining and nesting is discouraged.

    > By chaining or nesting an assignment expression, its result can itself be assigned to another variable. It can be logged, it can be put inside an array literal or function call, and so on.

    ### Comparison Operators

    > A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === (equal) and !== (not equal) operators, which perform strict equality and inequality comparisons. (quiz day 6)

    ### Logical Operators

    >Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value.

    ### String Operators

    > In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

    ### Functions

    - functions make sense to me currently
    - fucntion, you name the function, then you give it parameters, then you tell it what you want it to do with those elements, enclose with curly brackets. 
    - alter this by taking out parameters and assigning values 
    - naming functions help with debugger's stack traces
    - operators can exist within functions?
    - calling the function performs the specified actions with the indicated parameters

         > console.log(square(5));

        >   /* ... */

        >function square(n) { return n * n }

    >A function defined in the global scope can access all variables defined in the global scope. A function defined inside another function can also access all variables defined in its parent function, and any other variables to which the parent function has access.
        // The following variables are defined in the global scope

        var num1 = 20,

        num2 = 3,

        name = 'Chamakh';


        // This function is defined in the global scope

       function multiply() {

    return num1 * num2;

        }

    multiply(); // Returns 60

    // A nested function example

function getScore() {

  var num1 = 2,

      num2 = 3;


  function add() {

    return name + ' scored ' + (num1 + num2);

  }

  return add();
}

getScore(); // Returns "Chamakh scored 5"

- A function that refers to itself and calls itself is recursion via the function's name, agruments.callee, and an in scopre variable that refers to the function. 

- Nested functions and closures: nest a function within another function. The inner function is private to its containing outer function. This also forms a closure. The outer funciton does not have access to the variables and functions defined instide the inner function. Inner functions wil lhave persistent and encapsulated data for inner functions to work with. 

- can be multiply-nested
- name conflicts, more nested scopes take precedence, the innermost will take precedence. 

- default parameters-- you can define how you want things to be interacted with and bypasss a manuel check in the fuction body

- rest parameters--collect arguments from the second one to the end

- javascript has several top-level, built in functions

### Control Flow

- order in which the computer executes statements in a script
- 1st to last line, unless the computer runs across a conditional or a loop
- ex: if a field is left blank on a user input form
- parts of scripts set to execute when events occur
- *when you read a script pay attention from start to finish and look at program structure to see how it influences order of execution* 

