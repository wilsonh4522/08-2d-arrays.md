## Name: Wilson Huang
## Course: APCSA
## Period: 7
## Concept: Unit 8

### Introduction
In APCSA (AP Computer Science A) we are curretly learning about 2-D arrays in Java. This unit has so far been challenging but after some background knowldege about arrays in Java unit 6 & 7 it was easy to understand but I didn't do to well in the unit 7 exam. Throughout this writeup I will take you through some of my challenges, thinkings, and questions I got wrong on the exam. 

### Challenge #1
One challenge I had in this unit is 

### Challenge #2

### Challenge #3
In this challenge I will take you through some of the questions I got wrong on the unit 8 exam.
#### Challenge #3.1
Consider the following method that is intended to return true if all the Strings in the 2-d array arr have length 3:

public static boolean rowOfLengthThreeStrings(String[][] a) 
{
  /* Missing Code */
}
Which of the following could replace /* Missing Code */ so that the method works as intended?
```Java
for (int j = 0; j < arr.length; j++) 
{
  for (int k = 0; k < arr[j].length; k++) 
  {
    if (arr[j][k].length() == 3) 
    {
      return true;
    }
  }
}
```
```Java
return false; 
for (int j = 0; j < arr.length; j++) 
{
  for (int k = 0; k < arr[j].length; k++) 
  {
    if (arr[j][k].length() != 3) 
    {
      return false;
    }
  }
}
return true;
```
```Java
boolean result = true;
for (int j = 0; j < arr.length; j++) 
{
  for (int k = 0; k < arr[j].length; k++) 
  {
    if (arr[j][k].length() != 3) 
    {
      result = false;
    }
  }
  return result;
}
```
For this question I chose one and two but this is wrong because the whole array list has to have a length of three so if the array has a list of `bye, hello, red`, it would return true because after going through `bye` it will return true. This is wrong because the `hello` is more than four letters. The first one is correct because it goes through each item in the array to check if it has a length of 3.
#### Challenge #3.2

#### Challenge #3.3

### Takeaways
* Plug in values for questions in the exam
