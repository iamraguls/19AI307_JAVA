# Ex.No:3(D) PROGRAM TO PRINT OUTPUT UPTO SEPARATOR SYMBOL USING STRING TOKENIZER

## AIM:
To write a Java program that prints the first token from the input string up to the separator symbol (`,`) using the `nextToken` method of the `StringTokenizer` class.

## ALGORITHM :
1. Start the program.
2. Read the input string using `Scanner`.
3. Create an instance of `StringTokenizer` using the input string and the separator `,`.
4. Check if there are more tokens available using `hasMoreTokens()`.
5. If a token is available, retrieve it using `nextToken()` and print it.
6. If no tokens are found, print a message indicating no token was found.
7. End.

## PROGRAM:
```
/*
Program to print output up to separator symbol (,) using StringTokenizer in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 3D_TOKEN_EXAMPLE.JAVA:
```java
import java.util.*;

public class TokenExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine();
        StringTokenizer tokenizer = new StringTokenizer(input, ",");
        
        if (tokenizer.hasMoreTokens()) {
            String token = tokenizer.nextToken();
            System.out.println("Next token is : " + token);
        } else {
            System.out.println("No token found.");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/dec8f1c3-f150-4bd9-b9e8-31e1989d26ae)


## RESULT:
Thus, the Java program to print the output up to the separator symbol (`,`) using the `StringTokenizer` class was successfully implemented and executed.
