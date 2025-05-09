# Ex.No:3(E) PROGRAM TO CONVERT STRING INTO CHARACTER ARRAY

## AIM:
To write a Java program that converts a string into a character array and displays the characters in the array in order.

## ALGORITHM :
1. Start the program.
2. Read a string from the user input.
3. Use the `toCharArray()` method to convert the string into a character array.
4. Print the characters of the array, separating them with commas.
5. End.

## PROGRAM:
```
/*
Program to convert String into a character array and display the characters in order in Java.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 3E_STRING_TO_CHAR_ARRAY.JAVA:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.nextLine();
        char[] arr = s.toCharArray();
        System.out.print('[');
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i]);
            if (i < arr.length - 1) {
                System.out.print(", ");
            }
        }
        System.out.print(']');
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5c7ecb54-e0ef-454c-a630-c2298593d807)


## RESULT:
Thus, the Java program to convert a string into a character array and display the characters in order was successfully implemented and executed.
