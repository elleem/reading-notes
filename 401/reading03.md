## FileIO & Exceptions

#### Things I Want to Know More About

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

use this method to iterate over the file object itself:

`with open('dog_breeds.txt','r') as reader:`

    `for line in reader:`

    `print(line, end='')`


### Exceptions 

### Read & Write Videos

