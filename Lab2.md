# Lab 2


## In this lab please write a simple character, word, and line count function and test it on a couple of files


## Some useful background material:

The <a href="https://the-examples-book.com/book/introduction" target="_blank">Purdue Data Mine Examples Book</a> contains many useful chapters on data science. While they have not been directly designed for this class, they may be useful. You will not need to use scholar to perform the exercises of this class so don't worry about that part. Here is a direct link to the <a href="https://the-examples-book.com/book/python/introduction" target="_blank">Python chapter.</a>


Additional useful links for Python include:

<a href="https://docs.python.org/3/" target="_blank">Python 3.9.4 documentation</a>

The <a href="https://pypi.org/" target="_blank">Python Package Index</a> (This contains many of the useful Python "add-on" packages such as the math package)

The <a href="https://numpy.org/" target="_blank">Numpy Package</a> (This contains specialized array (vector and matrix) routines. Numpy stands for "Numerical Python")

United States Department of Agriculture: <a href="https://quickstats.nass.usda.gov/" target="_blank">Quick Stats</a> (The USDA's National Ag Statistics Service -- go here and familiarize yourself with the available data)


```python
# Import packages ...
import numpy as np
import matplotlib as mpl
import matplotlib.pyplot as plt
```

## A Python Function to count characters, words, and lines in a file

Takes a file located in the current working directory. Reads it. And counts these items printing the numbers to standard output ...


```python
# Skeleton of the function to write ...

def PoorMansWordCount(file_name):
    
    fin = open(file_name, 'r') # open the given file name for reading only
    
    # initialize three variables to zero for holding the numbers of characters, words, and lines
    print(file_name) 
    
    Nchar = 0
    Nsentences = 0
    Nword = 0
    Nlines = 0
    
    for line in fin:
        Nlines += 1# Everytime we read a line, we count it ...
        Nsentences += len(line.split('.'))
        Nchar += len(line)                 # increment by the length of the line you just read ...
        Nword += len(line.split())         # increment of the length of the list you get by splitting the line on whitespace
        
        # print(line)
        # print()
    print(f'Number of lines in {file_name} is {Nlines}.')  
    print(f'Number of sentences in {file_name} is {Nsentences}.') 
    print(f'Number of words in {file_name} is {Nword}.')     
    print(f'Number of characters in {file_name} is {Nchar}.')     
   
    return None
```


```python
# Test your solution on the PLimerick file ...

PoorMansWordCount('Data/PLimerick')
```

    Data/PLimerick
    Number of lines in Data/PLimerick is 8.
    Number of sentences in Data/PLimerick is 9.
    Number of words in Data/PLimerick is 42.
    Number of characters in Data/PLimerick is 191.



```python
# Test your solution on President Obama's First Inagural Speech

PoorMansWordCount('Data/ObamaFirstInagural.tex')
```

    Data/ObamaFirstInagural.tex
    Number of lines in Data/ObamaFirstInagural.tex is 183.
    Number of sentences in Data/ObamaFirstInagural.tex is 296.
    Number of words in Data/ObamaFirstInagural.tex is 2423.
    Number of characters in Data/ObamaFirstInagural.tex is 13548.



```python

```


```python

```
