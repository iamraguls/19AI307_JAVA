# Ex.No:8(E) READING DATA FROM CONSOLE USING InputStreamReader AND BufferedReader

## AIM:
To write a Java program for reading data from the console using `InputStreamReader` and `BufferedReader`.

## ALGORITHM:
1. Import necessary classes: `InputStreamReader`, `BufferedReader`, and `IOException`.
2. Create an `InputStreamReader` object that reads from `System.in` (console input).
3. Create a `BufferedReader` object that uses the `InputStreamReader` object.
4. Read the input data using `readLine()` method of `BufferedReader`.
5. Display the input data with a prefix "Welcome: " to the user.

## PROGRAM:
```
/*
Program to read data from the console using InputStreamReader and BufferedReader.
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 8E_READING_DATA_FROM_CONSOLE.JAVA:
```java
import java.io.*;

public class ConsoleInputExample {
    public static void main(String[] args) throws IOException {
        InputStreamReader r = new InputStreamReader(System.in);
        BufferedReader br = new BufferedReader(r);
        String name = br.readLine();
        System.out.println("Welcome: " + name);
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/aa078aec-84f4-49b1-b5b8-adbbf8f6ed73)


## RESULT:
The Java program for reading data from the console using `InputStreamReader` and `BufferedReader` was successfully executed.
