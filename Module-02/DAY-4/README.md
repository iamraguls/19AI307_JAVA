# Ex.No:2(D) MULTIDIMENSIONAL ARRAY TO READ AND DISPLAY VALUES ROW BY ROW

## AIM:
To write a Java program to read values for a multidimensional array and display the values row by row.

## ALGORITHM :
1. Start the program.
2. Read the number of rows and columns for the multidimensional array.
3. Create a 2D array with the given rows and columns.
4. Use nested `for` loops to read values into the array.
5. Print the array elements row by row using nested loops.
6. End.

## PROGRAM:
```
/*
Program to read values into a multidimensional array and display them row by row in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 2D_MULTIDIMENSIONAL_ARRAY_READ_DISPLAY.JAVA:
```java
import java.util.Scanner;

public class MultiDimensionalArray {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int rows = scanner.nextInt();
        int cols = scanner.nextInt();
        int[][] arr = new int[rows][cols];
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                arr[i][j] = scanner.nextInt();
            }
        }

        System.out.println("Printing array elements row by row:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(arr[i][j] + " ");
            }
            System.out.println();
        }

        scanner.close();
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/630d57b8-0312-4626-91a1-c153e7ef8e83)




## RESULT:
Thus, the Java program to read values into a multidimensional array and display them row by row was implemented and executed successfully.
