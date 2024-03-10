## Name: Wilson Huang
## Course: APCSA
## Period: 7
## Concept: Unit 8

### Introduction
In APCSA (AP Computer Science A) we are curretly learning about 2-D arrays in Java. This unit has so far been challenging but after some background knowldege about arrays in Java unit 6 & 7 it was easy to understand but I didn't do to well in the unit 7 exam. Throughout this writeup I will take you through some of my challenges, thinkings, and questions I got wrong on the exam. 

### Challenge #1
One challenges I had in this unit is simple misunderstandings I had when learning about 2-D arrays. For example 2-D arrays are row major order so we go `[row][column]`. I keep getting confused on what row and column is and it takes me a while to get used to it. I would sometimes confuse them with each other and get something wrong. Another misunderstading would be the numbers in the row and column like `[5,3]`; I would also get confused if the number meant that there would be 6 rows and 4 columns because I get confused if the numbers in the bracket start at 0 or 1. 
```java
int[][] testScores = new int[10][4]; \\ I might confuse myself if this might have 10 or 11 rows and 4 or 5 columns
```

### Challenge #2
Another challenge that I faced when learning on your unit 8 is trasversing through 2-D arrays. When I first learned about it it was confusing because there was a lot going on. Howver I watched this [video](https://www.youtube.com/watch?v=zZWZNSeys_4) to better understand the concept of trasversing though a 2-D array. After watching the video I finnaly understood how it worked. Trasversing through through 2-D arrays were basiccaly two for loops that represent the row and column. The row is the first for loop and the column represents the second for loop inside the first one. When trasversing though a 2-D array it will check every every element in the first row and then move to the next.
```java
for(int r = 0; r < arr.length; r++){ // Goes through all the rows inside the 2-D array but has to go thruogh every column in each row in order to move on to the next 
  for(int c = 0; c < arr.length; r++){ // Goes though each column in the row and moves to the next

  }
}

```
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
* Plug in values for questions in the exams to have a better chance to get the question correct
* Watch videos if you don't understand something beacuse there are a lot of resources online
* Always review the questions you got wrong on the test because thats how you learn
