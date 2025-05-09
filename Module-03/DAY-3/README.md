# Ex.No:3(C) PROGRAM TO RETURN FIRST HALF OF STRING IF EVEN LENGTH

## AIM:
To write a Java program that returns the first half of a string if the string's length is even. If the string's length is odd, the program will return `null`.

## ALGORITHM :
1. Start the program.
2. Read a string from the user input.
3. Define a method `getFirstHalf` to check if the length of the string is even.
4. If the length is even, return the first half of the string.
5. If the length is odd, return `null`.
6. Print the result from the method call.
7. End.

## PROGRAM:
```
/*
Program to return the first half of a string if the length is even in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 3C_FIRST_HALF_STRING.JAVA:
```java
import java.util.*;

public class StringHalf {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine();
        String result = getFirstHalf(input);
        System.out.println(result);
    }

    public static String getFirstHalf(String str) {
        if (str.length() % 2 == 0) {
            return str.substring(0, str.length() / 2);
        } else {
            return null;
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/f81b0158-f6bd-4e0f-9336-58acf5b5de2c)



## RESULT:
Thus, the Java program to return the first half of a string if the length is even was successfully implemented and executed.
