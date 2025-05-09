# Ex.No:7(B) TRY-CATCH-FINALLY CLAUSE WITH NullPointerException

## AIM:
To write a Java program to demonstrate the control flow of try-catch-finally clause when `NullPointerException` occurs.

## ALGORITHM:
1. Start the program.
2. Create a string variable and assign it null.
3. Try accessing the length of the null string inside try block.
4. Catch the `NullPointerException` and print the exception message.
5. Use finally block to print a statement indicating it was executed.
6. Print a statement outside try-catch-finally to indicate normal flow.

## PROGRAM:
```
/*
Program to demonstrate control flow of try-catch-finally clause.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 6E_TRY_CATCH_FINALLY.JAVA:
```java
public class TryCatchFinallyDemo {
    public static void main(String[] args) {
        try {
            String str = null;
            System.out.println(str.length()); 
        } catch (NullPointerException e) {
            System.out.println("Exception: " + e);
        } finally {
            System.out.println("Finally block executed");
        }
        System.out.println("Outside try-catch-finally clause");
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/dc20ab68-ffbb-49c4-abc6-d477a1350647)


## RESULT:
Thus, the Java program demonstrating control flow of try-catch-finally with `NullPointerException` was successfully implemented and verified.
