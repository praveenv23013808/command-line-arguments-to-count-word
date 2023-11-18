##5b. command-line-arguments-to-count-word

Date: 10.10.2023

AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.

EQUIPEMENT'S REQUIRED:
PC Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:Import sys module to use command line arguments
### Step 2:Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument
### Step 3:Iterate the content of the file using for loop.
### Step 4:Split the contents into each line using .split() function.
### Step 5:Iterate the list of lines and increment the value of variable (word) each time.
### Step 6:Run the program by giving "python prgm.py EX12.txt" on the terminal. 
## PROGRAM:
```
#Developed By: Praveen v
#Register No: 212222233004
import sys
count = {}
with open('/content/COMMAND LINE COUNT WORD.txt', 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
print(count)
f.close()
```
### OUTPUT:
![280464334-8b3a4901-dcfe-4874-8936-4dfa0779bf19](https://github.com/praveenv23013808/command-line-arguments-to-count-word/assets/145824728/13b013eb-abc9-42d8-bd87-7568bb1e14ac)
## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
