# Ex.No:9(C) PROGRAM TO PRINT STRING USING StringWriter

## AIM:
To write a Java program that reads a string from the user and prints it using `StringWriter`.

## ALGORITHM:
1. Start the program.
2. Create a `Scanner` object to read input from the user.
3. Create a `StringWriter` object to store the string.
4. Read a string value from the user using `nextLine()` method.
5. Write the string to the `StringWriter` object.
6. Display the string content stored in the `StringWriter` using `toString()`.
7. Close the `StringWriter`.
8. End.

## PROGRAM:
```
/*
Program to print the string using StringWriter
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 9C_PRINT_STRING_USING_STRINGWRITER.JAVA:
```java
import java.io.StringWriter;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String data = sc.nextLine();
        try {
            StringWriter writer = new StringWriter();
            writer.write(data);
            System.out.println("Data in the StringWriter: " + writer.toString());
            writer.close();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/1a5e46f8-25ac-4f27-abaf-ba8465bfe600)


## RESULT:
Thus, the Java program that reads a string from the user and prints it using `StringWriter` was successfully implemented and executed.
