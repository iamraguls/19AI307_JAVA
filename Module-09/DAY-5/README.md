# Ex.No:9(E) DISPLAY NUMBER OF BYTES AFTER SKIP FUNCTION USING BYTEARRAYINPUTSTREAM

## AIM:
To demonstrate the use of the `skip()` function in `ByteArrayInputStream` to skip a specific number of bytes and display the remaining byte values.

## ALGORITHM :
1. Initialize a byte array with values `{1, 2, 3, 4}`.
2. Create a `ByteArrayInputStream` object using the byte array.
3. Use the `skip()` method to skip 1 byte.
4. Read and display the remaining byte values using the `read()` method.
5. End.

## PROGRAM:
```
/*
Program to display the number of bytes after skipping using ByteArrayInputStream in Java
Developed by: Ragul S
RegisterNumber: 212222060184
*/
```

## 9E_SKIP_FUNCTION_BYTEARRAYINPUTSTREAM.JAVA:
```java
import java.io.ByteArrayInputStream;

public class Main {
  public static void main(String[] args) {
      byte[] array = {1, 2, 3, 4};
      try {
          ByteArrayInputStream by = new ByteArrayInputStream(array);
          by.skip(1); // Skip 1 byte
          System.out.print("Input stream after skipping 1 bytes: ");
          int data;
          while ((data = by.read()) != -1) {
              System.out.print(data + ", ");
          }
      } catch (Exception e) {
          e.printStackTrace();
      }
  }
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/fc123186-337f-48f4-9104-09d51788b577)


## RESULT:
Thus, the Java program to display the number of bytes after using the `skip()` function in `ByteArrayInputStream` was implemented and executed successfully.
