## SQL Notes

SELECT [stuff you want to select] FROM [table that it is in]; 
* splat = the whole table short cut

### ORDER BY
SELECT [stuff you want to select] FROM [table that it is in] ORDER BY [column you want]; 

  ASC and DESC

### LIMIT
SELECT * FROM artists LIMIT [# to limit by]; 

### OFFSET
SELECT * FROM artists LIMIT [# to limit by] OFFSET [# of rows to skip];

Filter and sort using DISTINCT to discard duplicate data, and ORDER BY to sort raw data. You may also need to limit results to a subset with LIMIT and OFFSET (for example like a reddit homepage)

### COUNT
COUNT(*); 
to see how much data


### AND OR
An AND is essentially multiplication. An OR is logic addition, so AND first and then OR, use parenthesis to specify the order of operations


### Operators
= equal
< less than
> greater than
<= less than or equal
>= greater than or equal
!= not equal
<> not equal 

LIKE a string matches a pattern
ILIKE case insensitive version of LIKE
SIMILAR TO a string matches a regex pattern

### Database Normalization

entity data in the real world is often broken down into pieces and stored across multiple orthogonal tables using a process known as normalization, so that data can grow independently of each other. 

### Database Maintenance

Use JOIN to combine row data across separate tables. 
INNER JOIN matches rows from the first and second table when they have the same key. 
Use INSERT to update tables
Use Update to take multiple column/value pairs and apply changes to each row that matches the WHERE statement

Schemas very similar to noSQL


### SQL BOLT screenshots
1-6 and 13-18

<img width="236" alt="Exercise 1" src="https://user-images.githubusercontent.com/96095918/225795921-d6f11cc9-e4e5-4635-9cb2-13c2f24bff40.png">
<img width="236" alt="Exercise 2" src="https://user-images.githubusercontent.com/96095918/225796052-d711f1c4-3240-4f78-9401-a9d587b9760e.png">
<img width="206" alt="Exercise 3" src="https://user-images.githubusercontent.com/96095918/225795508-fcc3642d-2d3d-4710-adac-6c648cca4390.png">
<img width="204" alt="Exercise 4" src="https://user-images.githubusercontent.com/96095918/225801624-64b23952-cb00-4268-b586-fb6cd649a3d9.png">
<img width="203" alt="Exercise 5" src="https://user-images.githubusercontent.com/96095918/225805150-61b7bc16-826c-4361-8379-4b6cdeb48b6a.png">
<img width="192" alt="Exercise 6" src="https://user-images.githubusercontent.com/96095918/225806422-1b7b302e-82f4-4640-bf31-106b52901589.png">
<img width="191" alt="Exercise 13" src="https://user-images.githubusercontent.com/96095918/225807577-926aa09b-1e05-4a87-b0a2-3efdf14cf956.png">
<img width="193" alt="Exercise 14" src="https://user-images.githubusercontent.com/96095918/225809112-0a15332b-a37e-4a40-b058-af41a82e7269.png">
<img width="187" alt="Exercise 15" src="https://user-images.githubusercontent.com/96095918/225809477-d8324625-78be-4053-902d-37f65f733270.png">
<img width="197" alt="Exercise 16" src="https://user-images.githubusercontent.com/96095918/225811558-f42a0da4-a826-4277-a5fe-f9041ece1ccb.png">
<img width="188" alt="Exercise 17" src="https://user-images.githubusercontent.com/96095918/225812046-db70e0d9-b7ca-493a-ad12-8f7b1515a857.png">




## Engineering Readings

What’s the one thing I bring to this career (and a potential employer) that nobody else can?
<br>
 A deep understanding of how to be efficient. That doesn’t mean always working and closing as many tickets as possible, but spending time documenting solutions/errors, as well as spending time to plan and organize my own day and keeping up with smaller, incremental task items that require sustained effort to solve, but I don’t always have big blocks of time to devote to solving. A dedication for long names on variables. 
 <br>
What are 3 things I’ll start doing to “un-stick” myself whenever I get stuck on tough piece of code, logic, or feature?
<br>
Rubber duck explanations to check my own understanding, especially using pseudo code and manually solving the problems
Before thinking, I am so stuck and I can’t get unstuck and I need help–thoroughly preparing my debugging steps so that I can explain what I have told my program to do. 
Practice micro-solutions. I have encountered some practice of smaller problems in 301 in javascript and I continue to practice these. 
<br>
Note: TopCoder, Codility.com



