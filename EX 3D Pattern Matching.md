# EX 3D Pattern Matching
## DATE:
## AIM:
To write a python program to implement pattern matching on the given string using Brute Force algorithm.



## Algorithm
1. Read the text (s1) and the pattern (s2).
  
2. Determine lengths of both strings.

3. Slide the pattern over the text from index 0 to len(text) - len(pattern).

4. At each position, compare characters of the pattern with the corresponding substring in the 
   text.

5.If all characters match, return the current index.

6.If no match is found after full traversal, return -1.

## Program:
```
Program to implement the Pattern Matching.
Developed by: Nivetha A
Register Number: 212222230101 
```
```
def BF(s1,s2):
    len_s1 = len(s1)
    len_s2 = len(s2)
    for i in range(len_s1 - len_s2 + 1):
        j = 0
        while j < len_s2 and s1[i + j] == s2[j]:
            j += 1
        if j == len_s2:
            return i
    return -1
if __name__ == "__main__":
    a1=input() 
    a2=input() 
    b=BF(a1,a2)
    print(b)
```
## Output:
![438918884-d15a7adb-a1de-4a0b-88f3-91956c5c15af](https://github.com/user-attachments/assets/51039062-c9e7-41c9-81c5-02c618ce54b9)

## Result:
The brute force substring search program executed successfully and returned the starting index of the match or 0 if no match was found.
