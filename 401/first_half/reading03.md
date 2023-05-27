## FileIO & Exceptions

#### Things I Want to Know More About
FYI, the video assigned is paywalled, so I followed [Corey Schafer's tutorial](https://www.youtube.com/watch?v=Uh2ebFW8OYM)

### Read & Write Files

A file is continguous set of bytes used to store data.

There are three main parts: 
1. Header (metadata about the contents of the file)
2. Data (content)
3. End of file (special char indicating end of the file)

Type of file specified by the extension after the file name.

Paths: file path is a string that represents the location of a file.
--includes folder path, file name, and extension

Line endings: when working with file data, you will need to specify the line ending, which uses a specific pro-sign to communicate the end of a transmission.

In Windows you must use both Carriage return is \r and Line feed is \n. 

Windows and Unix will treat the line endings differently. 

You can parse a file incorrectly if you do not know if the character encoding is ASCII or UNICODE. 

Step 1: Open a file, using the built in open function. 

`file = open('dog_breeds.txt')`

Final Step: Close the file to avoid unexpected behavior, generally should use the `try-finally` block, but highly recommend the `with` further use `r` so that the file will open as a read-only.

`finally:`

   `file.close()`

`with open('dog_breeds.txt','r') as reader:`

Different types of options for modes include 'r', 'w', 'rb' (binary mode)

There are 3 different types of file objects, including txt, buffered binary files, raw binary files. 

`open()` returns a TextIOWrapper file object. 

Now you'll want to read and write to the file. 

`.read(size=-1)` reads from the file based on the # of size bytes. if no, none or -1 is passed the whole file is read. 

`.readlines()` reads as a list

`.readline(size=-1)` reads at most size number of char from the line, continues and wraps back around, same as above for no, none, and -1

`.read()` returns file as a single string

use this method to iterate over the file object itself:

`with open('dog_breeds.txt','r') as reader:`

    `for line in reader:`

    `print(line, end='')`

`.(write)string` writes the str to the file.

`.writelines(seq)` writes the seq to the file. no line endings, and you will add them. 

__file__  allows for the pathname of the file from which the module was loaded

use `'a'` to append to a file

You can combine read/write in instances of creating a new file. 

__enter__ __exit__ to create context manager

There are special libraries to manage many different file types.

There are special modules for CSV and JSON.


### Exceptions 

There are built in python exceptions, and you can create self defined exceptions. 

[exceptions](https://docs.python.org/3/library/exceptions.html)

You can assert exceptions for specific conditions, ex `assert('linux' in sys.platform)`

`raise` allows you to throw an exception at any time. 

You can use a try/except block to run code.

The code block will only run up to when the first exception is encountered. 

The except clause determine what will happen with the exception, you can anticipate multiple exceptions.

Else helps w/ multiple exceptions. 

Finally, allows you to implement an action to clean up after executing your code and it will always run.

### Read & Write Videos

Covers the read & write article using video, but they are paywalled after the intro and the open/close. 

with is a context manager

Paths are covered so closely in the reading because you may have to use the path to read/write the file.

covers printing the name of the file to ensure you are opening the correct file

`print(f.name)`

`print(f.mode)`  will tell you how you are opening the file 

`print(f.closed)` you still have access to the f variable, even though you have closed it with the context manager.

`.readline` singular reads one line and then continues on each time it is run.

The for loop allows you not to add everything into the memory!!! Aha.

Can use seek to set it back to the beginning. 

Demos how to read a file and then write a copy, which is pretty dang cool. 

Demos how to copy a picture and pictures in sizes. 

OHHH--that's why you would use binary mode, for pictures.


