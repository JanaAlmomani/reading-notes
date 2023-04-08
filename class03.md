Q1 :
### Using “with” statement to open and read a file

#### Algorithm (Steps)

* Use the open() function(opens a file and returns a file object as a result) to open the text file in read-only mode by passing the file name, and mode as arguments to it (Here “r” represents read-only mode).
with open(inputFile, 'r') 


* Using the readlines() function to obtain the list of lines of a given text file.
file.readlines(hint)

Q2 :
### Difference between the ‘read()’ and ‘readline()’ methods

The read() method reads the entire file and returns it as a string, while the readline() method reads one line at a time and returns it as a string.

- if you want to read the entire file into memory as a single string, use read().
```
with open('example.txt', 'r') as f:
    contents  = f.read()
    # do something with config

```
- if you want to read a file line by line, Use readline().

```
with open('example.data', 'r') as f:
    contents  = f.readline()
    for line in f:
        data = line.split(',')
        # do something with data
```
