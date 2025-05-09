# Ex.No:9(A) PROGRAM TO DISPLAY NUMBER OF BYTES AND READ INTEGER AND CHARACTER DATA FROM A FILE USING DataInputStream

## AIM:
To write a Java program that displays the number of bytes in a file and reads the integer and character data using `DataInputStream` from the file "OutputFile.txt".

## ALGORITHM :
1. Start the program.
2. Create a `DataInputStream` object named `di` using `FileInputStream` to read from the file "OutputFile.txt".
3. Use the `available()` method of `DataInputStream` to check the number of bytes available for reading and print it.
4. Read a UTF string using `readUTF()` and print the result.
5. Read an integer using `readInt()` and print the result.
6. Read a character using `readChar()` and print the result.
7. Close the `DataInputStream` object.
8. End.

## PROGRAM:
```
/*
Program to display number of bytes and read integer and character data from a file using DataInputStream
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 9A_DISPLAY_BYTES_READ_FROM_FILE.JAVA:
```java
import java.io.*;

public class Main {
    public static void main(String[] args) {
        DataInputStream di = null;
        try {
            di = new DataInputStream(new FileInputStream("OutputFile.txt"));

            int availableBytes = di.available();
            System.out.println("Available number of bytes to read: " + availableBytes);

            String utfString = di.readUTF();
            System.out.println("Read UTF: " + utfString);

            int intValue = di.readInt();
            System.out.println("Read int: " + intValue);

            char charValue = (char) di.readChar();
            System.out.println("Read char: " + charValue);
            
        } catch (IOException e) {
            System.out.println("Exception: " + e);
        } finally {
            try {
                if (di != null) {
                    di.close();
                }
            } catch (IOException e) {
                System.out.println("Exception while closing the stream: " + e);
            }
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/dc22903b-1f5e-4ab5-b99d-00c5ffce7b12)


## RESULT:
Thus, the Java program that displays the number of bytes and reads integer and character data from the file "OutputFile.txt" using `DataInputStream` was successfully implemented and executed.
