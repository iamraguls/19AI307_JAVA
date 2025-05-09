# Ex.No:8(C) FILE OPERATION - FILTERINPUTSTREAM

## AIM:
To write a Java program to get the actual number of available bytes in the file using FilterInputStream.

## ALGORITHM:
1. Import `java.io.*` and `java.util.*`.
2. Use `FileInputStream` to read from `"sample.txt"`.
3. Wrap it with `BufferedInputStream` (a subclass of `FilterInputStream`).
4. Use `available()` to check available bytes.
5. Use `skip()` to move ahead in the stream.
6. Again, use `available()` to display remaining bytes.

## PROGRAM:
```
/*
Program to find available bytes in a file using FilterInputStream
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 8C_FILTERINPUTSTREAM.JAVA:
```java
import java.io.*;
import java.util.*;

public class Main {
    public static void main(String[] args) {
        try {
            FileInputStream fin = new FileInputStream("sample.txt");
            FilterInputStream f = new BufferedInputStream(fin);
            Scanner sc = new Scanner(System.in);
            int sk = sc.nextInt();

            System.out.println("Available bytes in the file: " + f.available());
            f.skip(sk);
            System.out.println("Available bytes in the file: " + f.available());

            fin.close();
            f.close();
        } catch (IOException e) {
            System.out.println("An error occurred.");
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/63882158-5025-4366-8d92-93cdb06432a6)


## RESULT:
Thus, the Java program to get the number of available bytes in a file using FilterInputStream was successfully written and executed.
