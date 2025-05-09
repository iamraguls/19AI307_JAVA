# Ex.No:8(A) FILE OPERATION - OUTPUTSTREAM

## AIM:
To write a Java program to append a string for specified bytes in a file "sample.txt" using OutputStream.

## ALGORITHM:
1. Import `java.io.*` and `java.util.*`.
2. Use `FileOutputStream` with append mode to open `sample.txt`.
3. Read index and length from user.
4. Convert the string `SAVEETHA` into byte array.
5. Use `write(byte[], offset, length)` method to write specific bytes.
6. Handle exceptions using try-catch.

## PROGRAM:
```
/*
Program to append string using OutputStream
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 8A_APPEND_BYTES_OUTPUTSTREAM.JAVA:
```java
import java.io.*;
import java.util.*;

public class Main {
    public static void main(String[] args) {
        try {
            FileOutputStream f = new FileOutputStream("sample.txt", true);
            Scanner sc = new Scanner(System.in);

            int n = sc.nextInt();
            int m = sc.nextInt();

            String a = "SAVEETHA";

            System.out.println("Successfully Completed");
            byte b[] = a.getBytes();
            f.write(b, n, m);
            f.close();
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/56887356-be90-43ad-a6af-2f4860ef93bd)


## RESULT:
Thus, the Java program to append a string for specified bytes in a file using OutputStream was successfully written and executed.
