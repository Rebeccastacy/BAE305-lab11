# BAE305 Lab 11 - Data Informatics Part 2

Rebecca Stacy

March 27th, 2024

## Summary

The goal of this lab was to further familiarize student with Python. This was achieved by following the instructions for writing a function that would count characters, words, and lines in a file and print the results. We were also allowed to use Anaconda Assistant for this lab, so learning how AI can be used for coding was another purpose of this lab. To complete these objectives we used the limerick file from Lab 10, and a file containing Barack Obama's inagural adress. 

## Code

[Lab 11 Code](https://github.com/Rebeccastacy/BAE305-lab11/blob/main/Lab2.md)    

## Conclusion 

From this lab, I became more comfortable with python and with using AI to help me code. A skeleton of the function was provided, so I wrote the code for opening the file and printing the file name, and worte a line to count each of the assigned variables. We were also asked to see if the program could read the number of sentences in the file, which we initally tried by splitting the lines at each period. However, we realized that that does not give an accurate count because, as in the first line of the poem, the author's name has a period within it, so the program said the poem had 9 sentences when it really has 8. We then did some research to find that we needed a more advanced package to accurately read teh number of sentences. However, I was able to fill in the rest of the code to sucessfully read both the poem and the innagural adress and return the correct number of characters, word, and lines in each file which was the original goal of the lab. 
