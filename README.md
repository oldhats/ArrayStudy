# ArrayStudy Program

## Description

The `ArrayStudy` program performs a series of manipulations on a 2D array of double values. It includes steps to extract rows based on the fraction of negative values, replace negative values with the column average of non-negative values, and print the resulting array.

## Table of Contents

- [Usage](#usage)
- [Implementation Details](#implementation-details)
- [Example](#example)

## Usage

To use the program, create an instance of the `ArrayStudy` class and call the `manipulate` method, passing the 2D array and the fraction as parameters. The method will perform the specified manipulations and return the resulting array.

```java
public static void main(String[] args) {
    double[][] a = {{-1, 4, 3, 2, -3, 2}, {-2, 3, 5, -4, 0, 1}, {-1, -3, -4, 1, -1, 0}, {-1, 2, -
            3, 6, 5, 3}, {-3, 2, -3, -5, 0, 0}}; // A 5 x 6 Dimension;
    
    System.out.println("Printing input array...");
    printArray(a);
    
    double[][] b = manipulate(a, 0.5);
    
    System.out.println("Printing manipulated array...");
    printArray(b);
}
```
## Implementation Details
The program consists of the following key methods:

manipulate(double[][] a, double fraction): This method performs the extraction and replacement steps on the input array a based on the specified fraction.

extract(double[][] a, double fraction): Extracts rows from the input array based on the fraction of negative values in each row.

replace(double[][] b): Replaces negative values in each column of the input array with the column average of non-negative values.

printArray(double[][] a): Prints the content of a 2D array.

## Example

```java
Copy code
double[][] a = {{-1, 4, 3, 2, -3, 2}, {-2, 3, 5, -4, 0, 1}, {-1, -3, -4, 1, -1, 0}, {-1, 2, -
        3, 6, 5, 3}, {-3, 2, -3, -5, 0, 0}}; // A 5 x 6 Dimension;

System.out.println("Printing input array...");
printArray(a);

double[][] b = manipulate(a, 0.5);

System.out.println("Printing manipulated array...");
printArray(b);
```
This example demonstrates how to use the program to manipulate a 2D array with a specified fraction. The input array is printed before and after the manipulation.
