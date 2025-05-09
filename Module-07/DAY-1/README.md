# Ex.No:7(A) PROGRAM TO HANDLE DIVISION BY ZERO EXCEPTION

## AIM:
To write a Java program to handle `ArithmeticException` for division by zero using try-catch block.

## ALGORITHM:
1. Start the program.
2. Import `Scanner` class.
3. Create a scanner object to take user input.
4. Read two integers `num1` and `num2`.
5. Use try block to perform division.
6. Catch `ArithmeticException` to handle divide by zero error.
7. Print appropriate message based on whether exception occurred or not.
8. End.

## PROGRAM:
```
/*
Program to handle division by zero exception.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6D_DIVISION_EXCEPTION.JAVA:
```java
import java.util.Scanner;

public class DivisionByZeroException {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int num1 = scanner.nextInt();
        int num2 = scanner.nextInt();

        try {
            int result = num1 / num2;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("You Shouldn't divide a number by zero");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/0cdf6128-ffa2-4a8d-bf0c-034c992bcf8c)


## RESULT:
Thus, the Java program to handle division by zero exception using try-catch block was successfully implemented and verified.
