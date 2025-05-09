# Ex.No:9(B) PROGRAM TO WRITE COMMON DATA INTO TWO FILES USING ByteArrayOutputStream

## AIM:
To write a Java program that writes the multiplication of two integers into two files (F1.txt and F2.txt) using `ByteArrayOutputStream`.

## ALGORITHM :
1. Start the program.
2. Create two `FileOutputStream` objects `f1` and `f2` to write to the files "F1.txt" and "F2.txt", respectively.
3. Create a `ByteArrayOutputStream` object to store the multiplication result.
4. Read two integer values from the user.
5. Multiply the two integers and write the result into the `ByteArrayOutputStream`.
6. Write the contents of `ByteArrayOutputStream` to both files `F1.txt` and `F2.txt` using the `writeTo()` method.
7. Close all the streams (`ByteArrayOutputStream`, `FileOutputStream`).
8. End.

## PROGRAM:
```
/*
Program to write the multiplication of two integers into F1.txt and F2.txt using ByteArrayOutputStream
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 9B_WRITE_COMMON_DATA_TO_FILES.JAVA:
```java
import java.io.*;
import java.util.*;

public class Main {
    public static void main(String[] args) {
        FileOutputStream f1 = null;
        FileOutputStream f2 = null;
        ByteArrayOutputStream by = new ByteArrayOutputStream();
        Scanner s = new Scanner(System.in);
        
        try {
            f1 = new FileOutputStream("F1.txt");
            f2 = new FileOutputStream("F2.txt");
            
            System.out.println("Success...");
            int n1 = s.nextInt();
            int n2 = s.nextInt();
            
            int result = n1 * n2;
            
            // Writing the multiplication result to ByteArrayOutputStream
            by.write(Integer.toString(result).getBytes());
            
            // Writing the data in ByteArrayOutputStream to both files
            by.writeTo(f1);
            by.writeTo(f2);
            
        } catch (IOException e) {
            System.out.println("Exception: " + e);
        } finally {
            try {
                if (f1 != null) f1.close();
                if (f2 != null) f2.close();
                by.close();
            } catch (IOException e) {
                System.out.println("Exception while closing the streams: " + e);
            }
        }
    }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/d99a4e6c-d45c-4882-8a7d-1a6d2713ec64)


## RESULT:
Thus, the Java program that writes the multiplication of two integers into two files "F1.txt" and "F2.txt" using `ByteArrayOutputStream` was successfully implemented and executed.
