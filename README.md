# Java ArrayIndexOutOfBoundsException Bug

This repository contains a simple Java program that demonstrates an `ArrayIndexOutOfBoundsException`. The bug is caused by an off-by-one error in a loop that iterates over an array. The solution demonstrates how to correct the loop condition to prevent the exception.

## Bug Description

The `bug.java` file contains a program that attempts to access an array element that is beyond the bounds of the array.  The loop condition incorrectly includes the upper bound, leading to an attempt to access an element at index 5 in an array with a length of 5 (valid indices are 0 to 4).

## Solution

The `bugSolution.java` file provides the corrected code. The loop condition has been changed to 'i < arr.length', ensuring that only valid array indices are accessed. This prevents the `ArrayIndexOutOfBoundsException`.

## How to run the code

1. Save both `bug.java` and `bugSolution.java` files.
2. Compile and run each file using a Java compiler (like the one included in the JDK): 
   ```bash
   javac bug.java
   java bug
   javac bugSolution.java
   java bugSolution 
   ```