## Automation

#### Things I Want to Know More About


### Pythons Regular Expressions Tutorial

1. How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary library to work with them?

Based on the reading I would probably try `search()`, which returns a match object if the text matches the pattern anywhere in the string. Honestly, I was worried about all the work we did in 301 to try to match expressions and it seems like this library is a huge step up!

`import re`

apply `r` to interprete a raw string literal. 

With the search function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match.

+ - Checks if the preceding character appears one or more times starting from that position. (greedy)

* - Checks if the preceding character appears zero or more times starting from that position. (greedy)

? - Checks if the preceding character appears exactly zero or one time starting from that position.

{x} - Repeat exactly x number of times.
{x,} - Repeat at least x times or more.
{x, y} - Repeat at least x times but no more than y times.

The group feature of regular expression allows you to pick up parts of the matching text.  Can also be done with <>

When you need to use an expression several times in a single program, using compile() to save the resulting regular expression object for reuse is more efficient than saving it as a string.

### shutil
2. What is the purpose of the shutil library in Python, and provide an example of a common use case for file or directory management with this library?

It allows you to manage copying, moving, renaming, deleting files and diretories. 

`print('BEFORE:')`
`pprint.pprint(glob.glob('/tmp/example/*'))`

`shutil.rmtree('/tmp/example')`

`print('\nAFTER:')`
`pprint.pprint(glob.glob('/tmp/example/*'))`

### Automation Ideas
3. Explain one automation idea from the assigned material and describe how it can be implemented using Python’s regular expressions and shutil libraries.

Oh boy--this was tough. 

For the first idea: import the libraries, define the source and destination directories, created regular expressions to match the files extensions. 

Finally--loop through the source directory and move the files to new directories!

We start with 50 seconds of running thru the woods.

1. Automatically moving files (might be helpful with downloads)
2. Automatically moving files and renaming them
3. Open YouTube when your fav youtuber uploads a new video, potential for stock trading
4. Calculate compounding interest

### Automating Your Browswer and Desktop Apps

Assigned for later, a 40 minute watch

### Watchdog

A python library that monitors file system events, and allows you to trigger actions in response to those changes. 





